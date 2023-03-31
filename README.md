![Nyuu][1]
++++++++++[>+++++++++++>++++++++++<<-]>--.+++++++++.>-.<++++.-----------.+++++++++++.----..
**c**, x86asm, c++, and sometimes pascal. Learning Rust 🦀

### Programming peaked at C99

This is the most useful program
```c
#include <stdio.h>
#include <stdlib.h>

struct number {
    int digit;
    struct number *next;
};

struct number *create_number(int value);
struct number *add_numbers(struct number *a, struct number *b);

int main() {
    struct number *num1, *num2, *sum, *counter1;
    int array1[10];

    num1 = create_number(1);
    num2 = create_number(1);
    counter1 = create_number(0);

    sum = add_numbers(num1, num2);
    
    struct number *current = sum;
    while (current != NULL) {
        array1[counter1->digit]=current->digit;
        current = current->next;
        counter1 = add_numbers(counter1, create_number(1));
    }

    printf("1 + 1 = ");
    struct number *i;
    for(i = create_number(counter1->digit-1);i->digit>=0;i=add_numbers(i, create_number(-1)))
        printf("%d", array1[i->digit]);
    free(i);
    printf("\n");

    free(num1);
    free(num2);
    free(counter1);
    free(sum);

    return 0;
}

struct number *create_number(int value) {
    struct number *num = (struct number *) malloc(sizeof(struct number));
    num->digit = value;
    num->next = NULL;
    return num;
}

struct number *add_numbers(struct number *a, struct number *b) {
    struct number *result = NULL;
    struct number *prev = NULL;
    int carry = 0;
    while (a != NULL || b != NULL || carry != 0) {
        int sum = carry;
        if (a != NULL) {
            sum += a->digit;
            a = a->next;
        }
        if (b != NULL) {
            sum += b->digit;
            b = b->next;
        }
        struct number *digit = create_number(sum % 10);
        carry = sum / 10;
        if (result == NULL)
            result = digit;
        else
            prev->next = digit;
        prev = digit;
    }
    return result;
}
```

[1]: https://cdn.discordapp.com/attachments/676226832856776714/1023823772140179516/Nyuu.png

<!--
**lucynyuu/lucynyuu** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
