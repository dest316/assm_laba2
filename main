#include <stdio.h>
#include<iostream>
//Вариант 20
// y = {2 * x, x < 5
//	   {|a| + x, x >= 5
int main()
{
	
	
	short int x;
	short int a;
	_asm
	{
		mov x, -4;
		mov a, -10;
		cmp x, 5;
		jl link3;
		//jae link;		
	link:
		cmp a, 0;
		jl link2;
		link4:
		mov bx, x;
		add bx, a;
		mov x, bx;	
		jmp link5;
	link2:
		xor eax, eax;
		mov ax, a;
		sub a, ax;
		sub a, ax;
		//mov a, ax;
		jmp link4;
		
	link3:
		mov bl, 2;
		mov ax, x;
		imul bl;
		mov x, ax;
	link5:

	}
	printf("%d", x);
	//std::cout << b;
}
