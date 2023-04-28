# random-number-generation-in-c#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main()
{
    int lower = 100, upper = 200, count = 6;

    srand(time(0));

    for (int i = 0; i < count; i++) {
        int num = (rand() % (upper - lower + 1)) + lower;
        printf("the random numbers are %d\n", num);
    }

    return 0;
}
