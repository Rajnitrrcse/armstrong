#include<iostream>
#include<cmath>
using namespace std;
int main(){
     int num;
    cout<<"enter the number : \n";
    cin>>num;
    int numcpy=num;
    int numcpy_1=num;
    int digCount=0;
    for(int i=0;numcpy_1!=0;i++){
     digCount++;
    numcpy_1/=10;
   }
   int sum=0;
   for(int i=0;num!=0;i++){
    sum+=pow((num%10),digCount);
    num/=10;
   }
   cout<<sum<<endl;
   if(sum==numcpy){
    cout<<"given number is Armstrong number.";
   }else{
    cout<<"no! given number is not armstrong number";
   }
    return  0;
}
