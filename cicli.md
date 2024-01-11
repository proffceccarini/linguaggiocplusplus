### I Cicli
In informatica, un ciclo è una struttura di controllo che permette di eseguire ripetutamente un blocco di istruzioni finché una condizione 
specificata è vera. I cicli sono fondamentali per automatizzare e semplificare l'esecuzione di compiti ripetitivi.
In generale un ciclo è costituito da una condizione e da un blocco di istruzioni che saranno eseguite fino a quando la condizione è vera.

I cicli si distinguono in cicli pre e post condizionati e cicli definiti (o a conteggio) e indefiniti.

I termini "cicli pre-condizionati" e "cicli post-condizionati" si riferiscono al momento in cui la condizione di esecuzione di un ciclo viene valutata rispetto all'esecuzione del corpo del ciclo. 
Distinguiamo anche tra cicli "definiti" e "indefiniti" in base al fatto che il numero di iterazioni sia noto a priori o meno.

1. **Ciclo pre-condizionato**:
   - La condizione viene valutata prima dell'esecuzione del corpo del ciclo.
   - Se la condizione è falsa fin dall'inizio, il corpo del ciclo non viene eseguito nemmeno una volta.
   - Il ciclo `while` è un esempio di ciclo pre-condizionato.

   ```cpp
   while (condizione) {
       // Blocco di istruzioni
   }
   ```

2. **Ciclo post-condizionato**:
   - La condizione viene valutata dopo l'esecuzione del corpo del ciclo.
   - Il corpo del ciclo viene eseguito almeno una volta, indipendentemente dalla condizione.
   - Il ciclo `do-while` è un esempio di ciclo post-condizionato.

   ```cpp
   do {
       // Blocco di istruzioni
   } while (condizione);
   ```

3. **Ciclo definito**:
   - Il numero di iterazioni è noto a priori.
   - I cicli `for` sono spesso cicli definiti, poiché la condizione di terminazione è specificata all'interno dell'inizializzazione e dell'incremento/decremento.

   ```cpp
   for (inizializzazione; condizione; incremento/decremento) {
       // Blocco di istruzioni
   }
   ```

4. **Ciclo indefinito**:
   - Il numero di iterazioni non è noto a priori.
   - I cicli `while` e `do-while` possono essere cicli indefiniti, poiché il numero di iterazioni dipende dalla condizione.

   ```cpp
   while (condizione) {
       // Blocco di istruzioni
   }
   ```

   ```cpp
   do {
       // Blocco di istruzioni
   } while (condizione);
   ```

In sintesi, la distinzione tra pre-condizionato e post-condizionato riguarda il momento in cui la condizione è valutata rispetto all'esecuzione del corpo del ciclo, mentre la distinzione tra definito e indefinito riguarda il numero di iterazioni, se noto o meno a priori.

Esistono diverse tipologie di cicli, tra cui i più comuni sono il ciclo `for`, il ciclo `while` e il ciclo `do-while`. 

Ecco una breve spiegazione di ciascuno:

1. **Ciclo `for`**:
   Il ciclo `for` è spesso utilizzato quando il numero di iterazioni è conosciuto a priori. Si tratta di un ciclo pre-condizionato e definito.
   L'inizializzazione viene eseguita una sola volta all'inizio, la condizione è valutata prima di ogni iterazione, e l'incremento/decremento viene eseguito alla fine di ogni iterazione.

   ```cpp
   for (inizializzazione; condizione; incremento/decremento) {
       // Blocco di istruzioni
   }
   ```
  Ecco un esempio di ciclo `for` che stampa i numeri da 1 a 5:
  ```cpp
  #include <iostream>
  
  using namespace std;
  
  int main() {
      for (int i = 1; i <= 5; ++i) {
          cout << i << " ";
      }
  
      return 0;
  }
  ```
   
2. **Ciclo `while`**:
   Il ciclo `while` viene utilizzato quando la condizione di continuazione è verificata all'inizio di ogni iterazione.
   Si tratta di un ciclo pre-condizionato e indefinito.
   Se la condizione è vera, il blocco di istruzioni viene eseguito; altrimenti, l'esecuzione del ciclo termina.
   ```cpp
   while (condizione) {
       // Blocco di istruzioni
   }
   ```
Ecco un esempio di ciclo `while` in C++. 
In questo caso, il programma chiede all'utente di inserire un numero e continua a farlo finché l'utente non inserisce un numero pari.

```cpp
#include <iostream>

using namespace std;

int main() {
    int numero;

    cout << "Inserisci un numero positivo: ";
    cin >> numero;

    while (numero%2 == 1) {
        cout << "Il numero inserito non è pari. Riprova: ";
        cin >> numero;
    }

    cout << "Hai inserito un numero pari. Grazie!" << endl;

    return 0;
}
```
   

3. **Ciclo `do-while`**:  
 Il ciclo `do-while` è simile al ciclo `while`, ma garantisce che il blocco di istruzioni venga eseguito almeno una volta, indipendentemente dalla condizione.
 La condizione viene verificata alla fine di ogni iterazione. Si tratta di un ciclo post-condizionato indefinito.  
  
   ```cpp
   do {
       // Blocco di istruzioni
   } while (condizione);
   ```
Ecco un esempio di ciclo `do-while` in C++ chiede all'utente di inserire un numero e continua a farlo finché l'utente non inserisce un numero positivo. 
```cpp
#include <iostream>

using namespace std;

int main() {
    int numero;

    do {
        cout << "Inserisci un numero positivo: ";
        cin >> numero;
    } while (numero <= 0);

    cout << "Hai inserito un numero positivo. Grazie!" << endl;

    return 0;
}
```
