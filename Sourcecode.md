# C-mini-project-FUN-GAME-with-source-code
C mini project FUN GAME with source code
#include <stdio.h>
#include <stdlib.h>
#include<time.h>
void input();
void color();
void fun_games();
void jackpot();
void todayluck();
void red () {
  printf("\033[1;31m");
}

void yellow() {
  printf("\033[1;33m");
}

void reset () {
  printf("\033[0m");
}
void blue(){
    printf("\033[0;34m");
}
void green(){
    printf("\033[0;32m");
}
void Purple(){
    printf("\033[0;35m");
}
int main()
{
    printf("😍 WElCOME TO SUMMER GALATTA 🤩 ");
     printf("\nCheck your lucky day ");
     while(1){
     printf("\n\n\t 1-Color\t2-Fun Games");
     input();
     }
    return 0;
}
void input(){
    int input;
    printf(" \n\nclick the Option :");
    scanf("%d",&input);
     switch(input){
         case 1:
           color();
           break;
         case 2:
           fun_games();
           break;
         default:
           printf("\nPlease check the network connection");
           printf("\n Enter the vaid input");
     }

}
void color(){
    int i,n;
    int col_r;		 
		 
 srand ( time(NULL) );		 

 col_r = rand() % 10 + 1; 
 
    switch(col_r){
        case 1:
        yellow();
       printf(" \n\nToday your todaylucky color is Yellow");
       reset();
         break;
         case 2:
         printf("\n\n Today your todaylucky color is Orange");
         reset();
         break;
         case 3:
         green();
         printf(" \n\nToday your todaylucky color is Green");
         reset();
         break;
         case 4:
         blue();
         printf("\n\n Today your todaylucky color is BLue ");
          reset();
         break;
         case 5:
         red();
         printf(" \n\nToday your todaylucky color is Red ");
         reset();
         break;
         case 6:
         printf(" \n\nToday your todaylucky color is Violet");
         
         case 7:
         Purple();
         printf(" \n\nToday your todaylucky color is Purple");
         reset();
         break;
         case 8:
         printf(" \n\nToday your todaylucky color is Alice blue");
         break;
         case 9:
         printf(" \n\nToday your todaylucky color is Aqua");
         break;
         default:
         printf("\n\nToday your todaylucky color is White");
         break;
        
    }
}
  
void fun_games(){
    printf("\n\n Welcome to  SUMMER GALATTA Fun_Zone");
    printf("\n                😍  😍    ");
    printf("\n\n 1-Jackpot\t2-funny_face reaction *free 😍");
    int fun_in;
    printf("\n");
    scanf("%d",&fun_in);
    switch(fun_in){
        case 1:
         jackpot();
         break;
         case 2:
         todayluck();
         break;
         default:
         printf("\n\nSorry some thing went wrong \n try again");
         break;
    }
}
void jackpot(){
printf("\n\nJackpot 😍  Zone");
 printf("\n\nWelcome to jackzone");

 int jaz;
 Purple(); 
 printf("       \n\n            LEVEL-1                ");
 reset();
 int number,l2n;		 
 srand ( time(NULL) );		 
number = rand() % 10 + 1; 
 printf("\n\nEnter your lucky  number  and Spin the Wheel ");
 scanf("%d",&jaz);
   if(number==jaz);
   {
     printf("\nJackpot 🤩 for you 1000$ 🤩 ");
     green();
     printf("        \n\n           LEVEL-2                ");
     reset();
     printf("\nDo you want continue to LEVEL-2");
     printf("\n\nEnter 5 to LEVEL-2  :");
     scanf("%d",&l2n);
    }
 int l2ln;
 if(l2n==5){
     printf("\n\n 1-💥  Game over\t 2-4 You will win 1000 Rs\t 5-9 You will win 500 Rs");
     printf(" \n\n  Enter your lucky number and Spin the Wheel");
     int lr2;
     scanf("%d",&lr2);
     srand ( time(NULL) );		 
	 l2ln = rand() % 10 + 1; 
     printf("%d ", l2ln); 
      }   
      
      if(l2ln==1)
        {
         red();
         printf("\n\n                💥   Game over          ");
         reset();
       }
     else if(l2ln>=2&&l2ln<=4)
     {
          yellow();
         printf("\n\nYou won 1000 Rs");
         reset();
     }
     else{
         red();
         printf("\nBetterluck Nexttime");
          reset();
     }
     
     green();
     printf("        \n\n           LEVEL-3               ");
     reset();
     printf("\n\n Enter 5 to continue");
     int l3enter;
     scanf("%d",&l3enter);
     if(l3enter==5)
     {
         yellow();
         printf(" \n\nsorry LEVEL-3 is Premium user Only ");
         blue();
         printf(" \n\nReplay");
         reset();
     }
 
}
void todayluck(){
    printf("\n\nDo you want check the face_reaction");
    printf("\n\nThen Enter 5 to see it ");
    int factin;
    printf("\n");
    scanf("%d",&factin);
    if(factin==5){
        int facran;
        printf("\n\n Welcome to  SUMMER GALATTA funny_face ✨ ");
         printf("\n");
     scanf("%d",&facran);
     srand ( time(NULL) );		 
	 facran = rand() % 10 + 1; 
       switch(facran){
        case 1:
      
       printf("\n\n    🙄    ");
       
         break;
         case 2:
         printf("\n\n   😍  ");
         
         break;
         case 3:
         printf("\n\n     😅   ");
      
         break;
         case 4:
    
         printf("\n\n    😒    ");
      
         break;
         case 5:
    
         printf("\n\n    😒    ");
         
         break;
         case 6:
         printf("\n\n    😅   ");
         
         case 7:
        
         printf("\n\n    😎    ");
        
         break;
         case 8:
         printf("\n\n    😀    ");
         break;
         default:
         printf("\n\n    😛    ");
         break;
    }
    }
}
