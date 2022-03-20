# reverse.c
reverse the characters of the word using a pointer

#include<stdio.h>

#define MSG_len 80

int main(){
	
	char msg[MSG_len], *p;
	
	printf("enter a sentence: ");
	for(p=&msg[0]; p<&msg[MSG_len]; p++){
		*p = getchar();
		if(*p == '\n')
		break;
	}
	
	printf("reversal is: ");
	for(p--; p>=&msg[0]; p--)
	    putchar(*p);
	putchar('\n');    
	
	
	return 0;
}
