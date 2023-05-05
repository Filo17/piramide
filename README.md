# Piramide
Piramide è un esercizio che permette di calcolare il numero di blocchi di cemento necessari alla costruzione di una piramide

## Descrizione del progretto

Realizzazione di un programma in console che permette di: dato un numero di mattoni, di calcolare quanti piani di una piramide possono essere costruiti e anche quanti mattoni avanzano. <br>

**Ipotizzando che:**

- i piani della piramide siano quadrati
- la piramide da costruire sia compatta, cioè non ci siano cavità al suo interno. 
- ogni piano è quadrato, con una lunghezza laterale inferiore di due rispetto a quella sottostante.
- il primo piano è sempre di un mattone <br>

**Ad esempio:**
- il primo piano ha un mattone, il secondo 9 mattoni, il terzo 25 e così via
- con 1 mattone la piramide è alta 1 piano
- con 84 mattoni la piramide è alta 4 piani

## Come funziona?
  
<details>
<summary>Controllo mattoni</summary>

```c#
    if(mattoni<1){
        return 0;
    }
```

Questo pezzo di codice serve per controllare che il numero di mattoni non sia minore di 1, In quel caso non ci sarebbe alcun piano.
</details>

  
<details>
<summary>Calcolo piani</summary>

```c#
 while (mattoni > tot)
            {
                num = System.Math.Pow(counter, 2);
                counter += 2;
                tot = tot + num;
                if (mattoni<tot)
                {   
                    eccesso = tot-mattoni; //non funziona bene
                    break;
                }     
                piani ++;
            }
            return piani;
```

Questo pezzo di codice calcola il numero di piani della piramide
</details>
  
<details>
<summary>Calcolo eccesso</summary>

```c#
    //codice assente
```

Questo pezzo di codice calcola il numero di mattoni in eccesso.
</details>
  

  
  
  
