# c-Pattern-Programs-using-Matrix

#include<bits/stdc++.h>
using namespace std;

int main()
{
	int n;
	cin>>n;
int k=2*n-1;
int low=0,high=k-1;
int val =n;


int a[k][k];
	

for(int i=0;i<k;i++)
{
for(int h=low;h<=high;h++)
	{
		a[i][h]=val;
		a[h][i]=val;
		a[high][h]=val;
		a[h][high]=val;

	}
	

	low++;
	high--;
	val--;
}

for(int i=0;i<k;i++)
{

	for(int j=0;j<k;++j)
	{
		cout<<a[i][j]<<"\t";

	}

	cout<<"\n";

}

}
