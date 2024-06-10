# Marco-C-
Este código en C++ solicita al usuario el tamaño, grosor y carácter para un marco, y luego imprime el marco con esas características.
#include<iostream>
using namespace std;
void marco(int nume, char mar);
int main(){
	
	int num=0,num1=0,i=0;
	char mar=' ';
	
	cout<<"INGRESA EL TAMANIO DEL MARCO: ";
	cin>>num;
	
	cout<<"INGRESA EL GROSOR DEL MARCO: ";
	cin>>num1;
	
	cout<<"INGRESA EL CARACTER DEL MARCO: ";
	cin>>mar;
	
	for(i=0;i<num1;i++){
		marco(num,mar);
	}
	
	for(i=0;i<num;i++){
		if(i==0||i==num-1){
			cout<<mar;
			continue;
		}
		cout<<" ";
	}
		cout<<endl;
	
	for(i=0;i<num1;i++){
	
		marco(num,mar);
	}
		
	
	return 0;
}

void marco(int num, char mar)
{
	for(int i=0;i<num;i++){
		cout<<mar;
	}
	cout<<endl;
	return;
}
