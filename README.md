# bubble-sort
#include<iostream.h>
#include<conio.h>
class arr
{
	int a[10],n,m;
	public:
	void get();
	void sort();
	void display();
	
};
void arr::get()
{
	cout<<"enter size of array"<<endl;
	cin>>n;
	cout<<"enter array elements "<<endl;
	for(int i=0;i<=n;i++)
	{
		cin>>a[i];
	}
	cout<<"Elements are"<<endl;
	for(int j=0;j<=n;j++)
	{
		cout<<a[j]<<"  "<<endl;
	}
	cout<<endl;
}
void arr::sort()
{
	for(int i=0;i<=n;i++)
	{
		for(int j=0;j<=n-i;j++)
		{
			if(a[j]>a[j+1])
			{
				m=a[j+1];
				a[j+1]=a[j];
				a[j]=m;
			}
		}
	
	}
}
void arr::display()
{
	cout <<"Sorted Element List ...\n";
for(int i = 0; i<=n; i++) 
{
   cout <<a[i]<<endl;
}

}


void main()
{
	clrscr();
	arr a;
	a.get();
	a.sort();
	a.display();
	getch();
}
Algorithm:
1.	Repeat For J = 1 to N
2.	Repeat For K = 1 to N-J
3.	If (A[K] > A[K+1]) Then
4.	Interchange A[K] and A[K+1]
5.	[End of If]
6.	[End of Step 2 For Loop]
7.	[End of Step 1 For Loop]
8.	Exit

