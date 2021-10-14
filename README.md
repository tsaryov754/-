//СТАТИЧЕСКИЙ МАССИВ
const int SIZE=3;

Int main () 
{
int arr[SIZE]; // либо же сразу можем написать элементы массива: "={1,2,3}"
for(int=0;i<SIZE;i++) {
cout<<"arr["<<i<<"]=";
cin>>arr[i]; //внутри квадратных скобок - имя массива к которому мы обращаемся
}


//ДИНАМИЧЕСКИЙ МАССИВ
тип.эл.м. *имя.массива=new тип.эл.м.[переменная]
int n;
cin>>n;
int *arr = new int[n];
arr[0] = 100;
delete []arr;

// Вывод массива
for(int i=0; i<N; i++)
{
cout<<arr[i]<<" ";
}

// Заполнение динамического массива рандомными числами
#include<ctime>
#include<cstdlib>
using namespace std;

int main() {
srand(time(0));
int a, b;
Cout<<"enter a";
Cin>>a;
Cout<<"enter b";
Cin>>b;
Int n;
Cout<<"enter size of array";
Cin>>n;
Int *arr=new int[n];
For(int i=0; i<n; i++) {
Arr[i]=rand()%(b-a+1)+a;
}
Cout<<"result array";
For (int i=0; i<n; i++) {
Cout<<arr[i]<<" ";
}
Cout<<endl;
delete []arr;
return 0;
}

// Найти минимальный и максимальный элемент массива
int index_of_max=0;
for(int i=1; i<n; i++) {
if (arr[i]>arr[index_of_max]) {
Index_of_max=i; };
}
cout<<"Максимальный элемент массива = "<<arr[index_of_max]<<" и находится на позиции номер "<< index_of_max;

// Сортировка массива
for (int i=0; i<n-1; i++) {
Int indexOfMin=i;
For (int j=i+1; j<n; j++) {
If(arr[j]<arr[indexOfMin]) { indexOfMin = j }
}
If(indexOfMin != i) {swap(arr[i], arr[indexOfMin]);
}
