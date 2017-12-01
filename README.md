# Strcmp#include "txlib.h"

int my_strcmp (const char string1 [], const char string2 []);

int main ()

    {

    char data1 [] = "hello";
    char data2 [] = "hellou";
    printf ("%d", my_strcmp (data1, data2));

    }


int my_strcmp (const char string1 [], const char string2 [])

    {

    int result = 0;
    for (int i = 0; /*string1 [i] != 0 || string2 [i] != 0*/i >= 0; i ++)

        {

        if ( string1 [i] != string2 [i])

            {

            result = string1 [i] - string2 [i];
            break;

            }

        if (string1 [i] == 0 || string2 [i] == 0)

            {

            result = string1 [i] - string2 [i];
            break;

            }

        }

    return result;

    }
