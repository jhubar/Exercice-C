# Corrections — Exercices en C (Boucles et Suites)

---

## Correction Exercice 1 — Somme des N premiers entiers
```c
#include <stdio.h>

int main(void) {
    int N, i, S = 0;

    scanf("%d", &N);

    for (i = 1; i <= N; i++) {
        S += i;
    }

    printf("%d\n", S);
    return 0;
}
```

---

## Correction Exercice 2 — Produit des nombres impairs
```c
#include <stdio.h>

int main(void) {
    int N, i;
    int impair = 1;
    int P = 1;

    scanf("%d", &N);

    for (i = 1; i <= N; i++) {
        P *= impair;
        impair += 2;
    }

    printf("%d\n", P);
    return 0;
}
```

---

## Correction Exercice 3 — Factorielle
```c
#include <stdio.h>

int main(void) {
    int N, i, fact = 1;

    scanf("%d", &N);

    for (i = 2; i <= N; i++) {
        fact *= i;
    }

    printf("%d\n", fact);
    return 0;
}
```

---

## Correction Exercice 4 — Fibonacci
```c
#include <stdio.h>

int main(void) {
    int N, i;
    int a = 0, b = 1, c;

    scanf("%d", &N);

    for (i = 0; i < N; i++) {
        printf("%d ", a);
        c = a + b;
        a = b;
        b = c;
    }

    return 0;
}
```

---

## Correction Exercice 5 — Somme harmonique
```c
#include <stdio.h>

int main(void) {
    int N, i;
    double H = 0;

    scanf("%d", &N);

    for (i = 1; i <= N; i++) {
        H += 1.0 / i;
    }

    printf("%f\n", H);
    return 0;
}
```

---

## Correction Exercice 6 — Suite récurrente
```c
#include <stdio.h>

int main(void) {
    int N, i;
    int u = 2;

    scanf("%d", &N);

    for (i = 0; i <= N; i++) {
        printf("u%d = %d\n", i, u);
        u = 3 * u + 1;
    }

    return 0;
}
```

---

## Correction Exercice 7 — Somme des carrés
```c
#include <stdio.h>

int main(void) {
    int N, i, S = 0;

    scanf("%d", &N);

    for (i = 1; i <= N; i++) {
        S += i * i;
    }

    printf("%d\n", S);
    return 0;
}
```

---

## Correction Exercice 8 — Puissance
```c
#include <stdio.h>

int main(void) {
    int a, n, i;
    int p = 1;

    scanf("%d %d", &a, &n);

    for (i = 1; i <= n; i++) {
        p *= a;
    }

    printf("%d\n", p);
    return 0;
}
```

---

## Correction Exercice 9 — Syracuse
```c
#include <stdio.h>

int main(void) {
    int N, steps = 0;

    scanf("%d", &N);

    while (N != 1) {
        printf("%d ", N);

        if (N % 2 == 0)
            N = N / 2;
        else
            N = 3 * N + 1;

        steps++;
    }

    printf("1\n%d\n", steps);
    return 0;
}
```

---

## Correction Exercice 10 — Chaîne sans voyelles
```c
#include <stdio.h>

int main(void) {
    char s[200];
    int i = 0, count = 0;
    char c;

    fgets(s, 200, stdin);

    while (s[i] != '\0') {
        c = s[i];

        if (!(c=='a'||c=='e'||c=='i'||c=='o'||c=='u'||
              c=='A'||c=='E'||c=='I'||c=='O'||c=='U') &&
              c != '\n') {
            putchar(c);
            count++;
        }
        i++;
    }

    printf("\n%d\n", count);
    return 0;
}
```
