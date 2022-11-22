# text11
，

#include <iostream>//看不懂；
#include <cstring>
using namespace std; 

/* run this program using the console pauser or add your own getch, system("pause") or input loop */
void Hanoi(int n,char a,char b,char c){
    if(n==1){
        cout<<n<<":"<<a<<"move to"<<c<<endl;
    }else{
        Hanoi(n-1,a,c,b);
        cout<<n<<":"<<a<<"move to"<<c<<endl;
        Hanoi(n-1,b,a,c);
    }
}
int main(int argc, char** argv) {
    int n;
    char a,b,c;
    while(cin>>n>>a>>b>>c){
        Hanoi(n,a,b,c);
    }
    return 0;
}



