# Simple-Game-in-C
 <i> a game that receives input from the user to make a pyramid </i>

<p>In this game, you'll be prompted for a number.
When you sucessfully respond with a positive integer, the code will output a pyramid with the equivalent number of rows to the number you provided.</p>


<b>This program includes libraries created by Harvard University's Intro To Comp Sci 50</b>

#include <cs50.h>
#include <stdio.h>


int main(void)
{
    int n;
    do
    {
    n = get_int("Height: ");
    }
    while (n < 1);


    for (int i = 0; i < n; i++) 
    {
        printf("\n");

            for (int j = 0; j < i + 1; j++) 
            {
            printf("|");
            }
    }

    printf("\n\n"); 
}
