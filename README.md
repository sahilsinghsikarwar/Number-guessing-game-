# Number-guessing-game-
A number guessing game in C involves the program randomly selecting a number, and the player attempts to guess it. The game provides feedback on whether the guess is too high, too low, or correct.
#include <stdio.h>
#include<stdlib.h>
#include<math.h>
int main(){
    
    srand(time(0)) ;
    int random_number=(rand() % 100) + 1;
    int guessed_num;
    int no_of_guesses=0;
    

  do{ printf("enter the guessed number :");
  scanf("%d",&guessed_num);

    if(guessed_num>random_number){
        printf("please enter SMALL NUMBER \n");}

    else{printf("please ENTER LARGE NUMBER :\n");}

    no_of_guesses++;
    } while (guessed_num != random_number);
    printf(" you guessed the no. in %d guesses ", no_of_guesses);
    return 0;
}
