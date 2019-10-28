#include <unistd.h>

char top_left           = '/';
char top_right          = '\\';
char middle             = '*';
char sides              = '*';
char space              = ' ';
char bottom_left        = '\\';
char bottom_right       = '/';

void print(char a, char b, char d, char x)
{
    int c;
    c = 2;
    write(1,&a,1);
    if (x >= 2)
    {
        while (c < x)
        {
            write(1, &b, 1);
            c++;
        }
        write(1, &d, 1);
    }
    write(1, "\n", 1);
}

void rush(int x, int y)
{
    int c;
    c = 2;
    print(top_left, middle, top_right, x);
    while(c < y)
    {
        print(sides, space, sides, x);
        c++;
    }
    print(bottom_left, middle, bottom_right, x);
}

int main ()
{
  rush (10, 10);
  return 0;
}
