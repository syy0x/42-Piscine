La fonction ft_print_alphabet itère à travers les lettres de l'alphabet et les affiche à l'aide de la fonction putchar. Ensuite, la fonction main appelle ft_print_alphabet pour effectuer cette tâche d'affichage.
Il y'a un executable ' a.exe ' qui est le code ft_print_alphabet.c compiler avec gcc.

```c
/* ************************************************************************** */
/*                                                                            */
/*                                                        :::      ::::::::   */
/*   ft_print_alphabet.c                                :+:      :+:    :+:   */
/*                                                    +:+ +:+         +:+     */
/*   By: ruda-sil <marvin@42.fr>                    +#+  +:+       +#+        */
/*                                                +#+#+#+#+#+   +#+           */
/*   Created: 2023/09/15 10:31:23 by ruda-sil          #+#    #+#             */
/*   Updated: 2023/09/15 10:34:38 by ruda-sil         ###   ########.fr       */
/*                                                                            */
/* ************************************************************************** */

#include <unistd.h>

void ft_print_alphabet(void) {
    char lettreA = 'a';

    while (lettreA <= 'z') {
        write(1, &lettreA, 1);
        lettreA++;
    }
}

int main() {
    ft_print_alphabet();
    return 0;
}
```
En résultat quand vous ouvrez un CMD et que vous écrivez "a.exe", il vous renverra "abcdefghijklmnopqrstuvwxyz"
