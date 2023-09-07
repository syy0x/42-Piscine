Ce code définit une fonction ft_is_negative qui prend un entier en paramètre. Si l'entier est négatif, la fonction affiche 'N'. Si l'entier est positif ou nul, elle affiche 'P'.

```c
#include <unistd.h>

void ft_is_negative(int n) {
    if (n < 0) {
        write(1, "N", 1);
    } else {
        write(1, "P", 1);
    }
}

int main() {
    ft_is_negative(1);
    ft_is_negative(0);
    ft_is_negative(-1);
    return 0;
}
```