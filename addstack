



#include<iostream>
#include<stack>
using namespace std;


class bin{

      public :
	   stack <int>stack1;
	   stack <int>stack2;
	   stack <int>stack3;
	   void read();
	   void add();
	   void display();



};
//===========================
void bin:: read()
{


     int i,n,j;
	int a[40],a1[40];
// n=20;

   cout<<"\n enter the length of first no:";
   cin>>n;
	 cout<<"\n enter the binari no1:";

	 for(i=0;i<n;i++)
	 {

	   cin>>a[i];

	     if(a[i]==1){
	     stack1.push(1);}
	     if (a[i]==0){
	     stack1.push(0);}

	 }

	cout<<"\n enter the length of second  no:";
	cin>>n;
	 cout<<"\n enter the binari no2:";
	for(i=0;i<n;i++)
{      cin>>a1[i];

	     if(a1[i]==1)
      {
	     stack2.push(1);
      }
	     if(a1[i]==0)
     {
	   stack2.push(0);
    }


}
}


//=======================================
void bin::add()
{
    int bit1,bit2;
    int cry=0;
    int rem;
    while(!stack1.empty()|| !stack2.empty())
    {
	bit1=bit2=0;

	if(!stack1.empty())
	{
	 bit1=stack1.top();
	 stack1.pop();
	}
	 if(!stack2.empty())
	{
	 bit2=stack2.top();
	 stack2.pop();
	}
	 rem=(bit1+bit2+cry)%2;
	 cry=(bit1+bit2+cry)/2;
	 stack3.push(rem);


    }
    if(cry==1)
    stack3.push(1);

}
//===============================
void bin:: display()
{

 /*  cout<<"\n first no is:";
     while(!stack1.empty())
    {
	cout<<stack1.top();
	stack1.pop();
    }
   cout<<"\n second  no is:";
     while(!stack2.empty())
    {
	cout<<stack2.top();
	stack2.pop();
    }*/
 cout<<"\n addition:\n";
    while(!stack3.empty())
    {
	cout<<stack3.top();
	stack3.pop();
    }




}
//===============================
int main()
{

    int ch;
    bin b1;
    b1.read();
  b1.add();
    b1.display();
       /* do{
	    cout<<"\n select option:";
	    cout<<"\n1) Read no:\n2)add no \n3)display addition :\n4)exit\n";
	    cin>>ch;
	    switch(ch)
	    {
		case 1 : b1.read();
			   break;
		case 2: b1.add();
                       break;
                case 3: b1.display();
                      break;
                default: cout<<"\n pla anter valid chioce :";
                
            }
        }while(ch!=4);*/
  return 0;
}

