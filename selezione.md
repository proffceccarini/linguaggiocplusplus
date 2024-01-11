### La selezione (IF)

La selezione, nota in C++ come istruzione `if` in C++, è utilizzata per eseguire un blocco di codice se una condizione è vera. La sintassi generale è la seguente:

```cpp
if (condizione) {
    // Blocco di codice da eseguire se la condizione è vera
}
```

Se la condizione tra parentesi tonde è valutata come `true` (vero), il blocco di codice all'interno delle parentesi graffe viene eseguito. 
Altrimenti, se la condizione è `false` (falsa), il blocco di codice viene saltato e l'esecuzione continua con le istruzioni successive.

Ecco un esempio semplice:

```cpp
#include <iostream>

using namespace std;

int main() {
    int numero;

    cout << "Inserisci un numero: ";
    cin >> numero;

    // Istruzione di selezione
    if (numero > 0) {
        cout << "Il numero inserito è positivo." << endl;
    }

    return 0;
}
```

In questo esempio, se l'utente inserisce un numero positivo, il programma stampa un messaggio indicando che il numero è positivo. Se l'utente inserisce un numero non positivo (zero o negativo), il blocco di codice all'interno dell'istruzione `if` viene ignorato.

È anche possibile utilizzare l'istruzione `else` per specificare un blocco di codice da eseguire quando la condizione dell'`if` è falsa. Ecco un esempio:

```cpp
#include <iostream>

using namespace std;

int main() {
    int numero;

    cout << "Inserisci un numero: ";
    cin >> numero;

    // Istruzione di selezione con ramo else
    if (numero > 0) {
        cout << "Il numero inserito è positivo." << endl;
    } else {
        cout << "Il numero inserito non è positivo." << endl;
    }

    return 0;
}
```

In questo caso, se il numero è maggiore di zero, viene eseguito il blocco di codice nell'`if`. Altrimenti, viene eseguito il blocco di codice nell'`else`. Questo consente di gestire più scenari in base al risultato della condizione.
