Un programma in linguaggio C++ ha una struttura generale che comprende diverse sezioni. 
Ecco una panoramica della struttura di base di un programma C++:

```cpp
#include <iostream> // Dichiarazione della libreria necessaria per utilizzare gli operatori di input e output

using namespace std; // Dichiarazione dello spazio dei nomi standard

int main() {
    // Corpo principale del programma

    // Dichiarazione e inizializzazione di variabili 
    // ...

    // Operazioni e istruzioni 
    // ...

    // Istruzione di ritorno
    return 0;
}
```

Ora spieghiamo le parti principali della struttura:

1. **Direttiva `#include`**: Questa parte del codice include le librerie necessarie per il programma. Nel caso sopra, stiamo includendo la libreria `<iostream>`, che è fondamentale per le operazioni di input/output.

2. **Dichiarazione `using namespace std`**: Questa dichiarazione semplifica l'utilizzo di oggetti e funzioni definiti nello spazio dei nomi standard (`std`). Ad esempio, permette di scrivere `cout` invece di `std::cout`.

3. **Funzione `main`**: La funzione `main` è il punto di ingresso del programma. L'esecuzione del programma inizia dalla prima istruzione all'interno della funzione `main`. La sua dichiarazione è obbligatoria e deve restituire un valore intero (`int`).

4. **Corpo della funzione `main`**: Questa sezione contiene le istruzioni effettive del programma. Qui vengono dichiarate e inizializzate le variabili, eseguite le operazioni desiderate e utilizzate le funzioni definite nel programma.

5. **Istruzione di ritorno**: La funzione `main` deve restituire un valore intero. Tipicamente, si utilizza `return 0;` per indicare che il programma è stato eseguito correttamente. Un valore diverso da zero può essere restituito per indicare un errore o un'altra condizione particolare.

Ecco un esempio più dettagliato:

```cpp
#include <iostream>

using namespace std;

int main() {
    // Dichiarazione e inizializzazione di variabili
    int numero;

    // Input da console
    cout << "Inserisci un numero: ";
    cin >> numero;

    // Elaborazione
    int doppio = numero * 2;

    // Output su console
    cout << "Il doppio del numero inserito è: " << doppio << endl;

    // Istruzione di ritorno
    return 0;
}
```

Questo è solo un esempio di base. La struttura specifica di un programma C++ può variare in base alle esigenze del progetto.
