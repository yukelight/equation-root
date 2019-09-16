# equation-root
#include<iostream>
#include<cmath>
using namespace std;
int main()
{
	double a,b,c;
	double dela;
	double x1,x2,x3;
	cout<<"请依次输入方程的a,b,c"<<endl;
	cin>>a>>b>>c;
	if(a==0){
		if(b==0)
		  cout<<"方程无解";
		else{
	
		  x1=-c/b;
		  cout<<"方程的解x1="<<x1;
	        }
		}
	else
	{

	    dela=b*b-4*a*c;
	    if(dela>=0){
		  x1=(-b+sqrt(dela))/2/a;
	      x2=(-b-sqrt(dela))/2/a;
	      cout<<"方程的解x1="<<x1<<endl<<"方程的解x2="<<x2<<endl;
	    }
	    else
	    {
	      x1=-b/2*a;
		  x2=sqrt(-dela)/2*a;
		  cout<<"方程的解x1="<<x1<<"+"<<x2<<"i"<<endl;
		  cout<<"方程的解x2="<<x1<<"-"<<x2<<"i"<<endl;
	    }
	      
        
	} 
  return 0;
}
