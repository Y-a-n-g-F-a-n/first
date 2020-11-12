#include <stdio.h>
#include <windows.h>

//函数的声明与定义
int MyAdd() //形参
{
	//if (){

	//}
	//for (){

	//}
	//printf("after：_a: %d, _b: %d\n", _a, _b);
	//printf("after：_a: %p, _b: %p\n", &_a, &_b);

	//int _res = _a + _b; //局部变量->作用域&&生命周期~
	//return _res;
	return 0;
}
#pragma warning(disable:4996)

int MyMax(int x, int y)
{
	return x > y ? x : y;

	//int max = x > y ? x : y; //三目运算符
	//return max;
	//if (x > y){
	//	return x;
	//}
	//return y;
}

void show(){
	//static修饰局部变量的时候，有如下两个作用：
	//1. 作用域：在本代码块内有效~，用static修饰，这个作用不变
	//2. 生命周期：临时性，static修饰，则该变量的生命周期变成全局属性
	//3. 注意事项：int i = 0; 初始化，任何一个变量都只会初始化一次！！！

	static int i = 0; //临时变量具有临时性
	++i;
	printf("i : %d\n", i);
}

int main()
{
	for (int j = 0; j < 10; j++){
		show();
	}


	//printf("%d\n", -10 % -3);
	//printf("%d\n", !10);
	//printf("%d\n", !11);
	//printf("%d\n", !12);
	//printf("%d\n", !100);
	//printf("%d\n", !1000);
	//int x = 0;
	//int y = 0;
	//printf("Please Enter Two Data# ");
	//scanf("%d %d", &x, &y);
	//printf("Max: %d\n", MyMax(x, y));
	//int a = 10;
	//int b = 20;
	//if ((a == 20) || (b == 10)){
	//	printf("yes!\n");
	//}
	//else{
	//	printf("no!\n");
	//}
	//printf("%d\n", (1 == 2) && (2 == 2)); //&
	//10 != 20 //1
 //   10 == 20 //0
	//int a = 10;
	////++a; //++前置：先自增，在使用
	////a++; //后置++：先使用，在自增
	////--a;
	////a--;
	//int b = a++;
	//printf("%d\n", b); 
	//printf("%d\n", a);
	//int a = 1;         //0000 0000 0000 0000 0000 0000 0000 0001
	//printf("%u\n", ~a);//1111 1111 1111 1111 1111 1111 1111 1110
	//                   //1111 1111 1111 1111 1111 1111 1111 1110
	////int a = -10;
	////printf("%d\n", sizeof(a) ); //sizeof 是函数吗？?
	////strlen 是函数
	//int b = a;
	//printf("b = %d\n", b);
	/*printf("%d\n", 10 == 10);
	printf("%d\n", !(10 == 10));*/
	//int x = 100;
	//if (!(100 == x)){
	//	printf("yes x is 100!\n");
	//}
	//else{
	//	printf("no!\n");
	//}






	//int a = 10;
	//a = 20;
	//a += 5; //a = a + 5;
	//a -= 5; //a = a + 5;
	//a *= 5; //a = a + 5;
	//a /= 5; //a = a + 5;
	//a %= 5; //a = a + 5;
	//a &= 5; //a = a + 5;
	//a |= 5; //a = a + 5;
	//a ^= 5; //a = a + 5;






	//& ^ |
	//& 按位与
	// 1 ^ 1 = 0
	//1010
	//1100 ^
	//------
	//0110
	//6
	//printf("%d\n", 10 ^ 12); //8 + 4 
	//int a = 10;
	//printf("%d\n", a << 1); // 1010 << 1 == 10100
	////10
	//a >> 1 == a / 2; //5
	//a << 1 == a * 2; //20
	//1 ->   1
	//2 ->   10
	//4 ->   100
	//8 ->   1000
	//2^n -> 1...n个0
	//10 -> 1010 -> 1000 + 0010 -> 2^3 + 2^1
	//17 -> 16 + 1 -> 2^4 + 2^0 -> 10000 + 1 -> 10001
	//37 -> 32 + 4 + 1 -> 2^5 + 2^2 + 2^0 = 100101 vs 100101
	//10 / 3 = 3 ... 1
	//printf("%d\n", 10 / 3);
	//printf("%d\n", 10 % 3);
	//int a = 0;
	//int b = 0;
	//int c = a + b;
	////定义与初始化
	//int arr[] = { 11, 22, 33, 44, 55, 66,33,55,0};
	//printf("%d\n", sizeof(arr)); //求数组的总大小
	//printf("%d\n", sizeof(arr[0])); //求数组的一个元素的大小
	////动态的求出数组的个数
	//int num = sizeof(arr) / sizeof(arr[0]);
	//printf("num: %d\n", num);
	//char arr[] = "hello world";
	////数组的遍历
	//for (int i = 0; i < SIZE; i++){
	//	printf("arr[%d]: %d\n", i, arr[i]);
	//}
	//int a = 10;
	//int b = 20;
	//printf("before：a: %d, b: %d\n", a, b);
	//printf("before：a: %p, b: %p\n", &a, &b);
	//int result = MyAdd(); //实参 -》	
	//printf("result:%d\n", result);
	system("pause");
	return 0;
}
