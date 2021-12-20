# VuongT.Y Lab8b
На поле (к, I) расположен ферзь, ладья, слон или конь (должен ввести пользователь). Угрожает ли он полю (m, n)?
#include <stdio.h>
 
int main(int argc, char **argv)
{
    int k, l, m, n;
    printf("Enter the position of the queen:"); scanf("%i %i", &k, &l);
    printf("Enter the required field:"); scanf("%i %i", &m, &n);
    if ((k == m) || (l == n) || (k+l == m+n) || (k-m == l-n)) printf("The queen threatens the field %i %i", m, n);
    else printf("The queen does not threaten the field %i %i", m, n);
    return 0;
}
