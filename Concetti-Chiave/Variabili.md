1. Le variabili in javascript sono delle entità che servono a memorizzare dati che possono essere riutilizzati nel codice.

2. le variabili vanno dicchiarate così:
   tipo di variabile + nome della variabile = tipo di dato da memorizzare

   es: const Numero = 5

3. esistono tre parole chiave per definire le variabili : var, let e const.
   var:
    - era l'unico modo di dichiarare delle variabili all'interno di js prima dell'introduzione di let e const
    - ha scope globale quindi vuol dire che la variabile è accessibile dappertutto all'interno di una funzione in cui sono state dichiarate
    - il suo valore è modificabile.
   let: 
    - è stato aggiunto con ES6 (aggiornamento di js del 2015).
    - a differenza di var il suo valore è legibile solo nella parte di codice in cui è dichiarato (Block Scope).
    - il suo valore è modificabile come per var
   const:
    - è stato aggiunto con ES6 come nel caso di let.
    - il suo scope è sul blocco di codice in cui viene dichiarata (Block Scope).
    - il suo valore è immutabile e rimane costante., anche se è possibile cambiarene il valore al suo interno come nel caso degli oggetti o degli array.
     es 1:
     const person = {
     name: 'Alice',
     age: 30
     };

     // Possiamo modificare le proprietà dell'oggetto
     person.age = 31;

     console.log(person); // Output: { name: 'Alice', age: 31 }
    
     es 2: 
     const numbers = [1, 2, 3, 4, 5];

     // Aggiungiamo direttamente un nuovo numero all'array numbers
     numbers.push(6);

     console.log(numbers); // Output: [1, 2, 3, 4, 5, 6]
    