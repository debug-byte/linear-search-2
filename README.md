# linear-search-2
#include <iostream>

using namespace std;

int linearSearch(int a[],int size,int searchValue)
{
	for(int i = 0; i < size ; i++)
	{
		if (searchValue == a[i])
		{
			return i;
		}
	}
	return -1;
}

int main(){
int searchValue;
	int i;
	int userValue;
{
	int a[]={47,54,87,69,14,58,25,78};
     cout << "Enter a value :" << endl;
     cin>>userValue;
	
	
	int result = linearSearch( a, 8, userValue);
	
	if(result>=0) 
	{
		cout <<"The number" << a[result] <<"was found at element with index"<< result << endl;
	}
	else
	{
		cout <<"INVALID INPUT"<< endl;
	}
}  
return 0;
}
