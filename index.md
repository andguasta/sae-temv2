---
title: TeMV2 - Material Page
subtitle: "Pagina di supporto al corso Tecniche e Metodologie dei Videogiochi 2. Docente: Andrea Guastadisegni"
thumbnail-img: https://andguasta.github.io/sae-temv2/assets/img/CourseImage.png
cover-img: https://andguasta.github.io/sae-temv2/assets/img/Animal_Header1.png
---
| Course Software  | Course Program              |
| ---------------- | --------------------------- |
| Unity 2020.3 Lts | Introduction to Programming |
| - Visual Studio  | Advanced Music              |
| - Mac Buils      | Large Project Management    |
| Wwise 2019.2.15  | Version Control             |
| Git              | Game Engine Integration     |
| Sublime Text     | Resources Optimisation      |
| Sublime Merge    |                             |

- - -

Per i **Video** delle lezione e alcuni **Pdf** utili potete accedere a questa cartella Google Drive:
```
U2FsdGVkX19fYOVSoEE/ilXJRPfEQt1v7Y0PYIAsc67H6cfXnCo40nrycJed1yfl\nipD4hp5UROFb3WYrtcGCAJTk5eHePxc/F/Z86lQbCB7relwCtc/06tYjGc9TRjSE
```
---

## Books
### Technical Books
- **Code: The Hidden Language of Computer Hardware and Software** by Charles Petzold [link goodreads](https://www.goodreads.com/book/show/44882.Code)
    - Come funzionano i computer partendo dai componenti
- **Designing Sound** by Andy Farnell [link mitpress](https://mitpress.mit.edu/books/designing-sound)
    - Procedural Audio and Synthesis
    - Accessibile come studenti SAE nella e-library
- **The Audio Programming Book** by Richard Boulanger and Victor Lazzarini [link mitpress](https://mitpress.mit.edu/books/audio-programming-book)
    - Come si utilizza C nell'audio e come si implementano effetti e sintesi.
- **Microsound** By Curtis Roads [link mitpress](https://mitpress.mit.edu/books/microsound)
    - Sulla sintesi Granulare
    - Accessibile come studenti SAE nella e-library
- **The Computer Music Tutorial** By Curtis Roads [link mitpress](https://mitpress.mit.edu/books/computer-music-tutorial)
    - Copre tantissime tecniche di sintesi e di DSP. Libro molto importante per chi è interessato all'aspetto tecnico del sound design
- **Audio Engineer's Reference Book** by Michael Talbot-Smith [link routledge](https://www.routledge.com/Audio-Engineers-Reference-Book/Talbot-Smith/p/book/9780240516851)
    - Accessibile come studenti SAE nella e-library

### Non Audio Related Books
- **What If? Serious Scientific Answers to Absurd Hypothetical Questions** by Randall Munroe
[link goodreads](https://www.goodreads.com/book/show/21413662-what-if-serious-scientific-answers-to-absurd-hypothetical-questions)
    - Libro di xkcd che risponde in maniera scientifica a domande assurde
- **Deep Work: Rules for Focused Success in a Distracted World** by Cal Newport [link goodreads](https://www.goodreads.com/book/show/25744928-deep-work?ac=1&from_search=true&qid=3YjAFmWm5O&rank=1)
    - Lettura molto interessante su come gestire il tempo per riuscire a produrre lavori di qualità
- **Four Thousand Weeks: Time Management for Mortals** by Oliver Burkeman [link goodreads](https://www.goodreads.com/book/show/54785515-four-thousand-weeks)
    - Con il tempo limitato che abbiamo quanto possiamo fare veramente?

---

## Lessons
#### How to decode the Google Drive string
Il link è cryptato usando openssl. Potete decifrarlo usando il terminale:

```bash
printf "Received string here" | openssl enc -aes-256-cbc -md sha256 -a -d -pass pass:password
```


- **`printf`** è un comando che viene utilizzato per visualizzare una stringa nel terminale. Ad esempio: `printf "Hello, World!"`; Visualizzerà `"Hello, World!"` nel terminale.
- **`|`** è un operatore che viene utilizzato per prendere l'output di un comando e usarlo come input per un altro comando. Permette la concatenazione di comandi, dove l'output di un comando viene elaborato da un altro. Consente manipolazioni di dati complesse combinando comandi semplici senza la necessità di salvare risultati intermedi in un file.
- **`openssl`** è un toolkit open-source per SSL/TLS e crittografia. Offre funzionalità come comunicazione sicura, generazione di chiavi e gestione dei certificati.
- **`enc`** indica che si desidera cifrare o decifrare dei dati.
- **`-aes-256-cbc`** Specifica l'algoritmo da utilizzare, in questo caso, AES con una chiave da 256 bit.
- **`-md sha256`**:  Specifica di utilizzare un algoritmo di hashing che produce un valore hash di 256 bit.
- **`-a`** Questa opzione indica a OpenSSL di codificare l'output in base64. È utile quando i dati devono essere memorizzati e trasferiti su supporti progettati per gestire il testo.
- **`-d`** Decifra i dati in input. Senza questo flag, l'operazione predefinita sarebbe quella di cifrare.
- **`-pass pass:password`** Questo è il modo in cui si specifica la passphrase utilizzata per la cifratura o decifrazione. In questo caso, la passphrase è "password".

- - -

## Programming

Slides:
```
U2FsdGVkX1/Ay6JI9p3pJTr0MgTu4yvh2xTMtI7FAsmhDRDbgh5s5l1mdkubAhmQ\nnlzTAVYgcShtI40zXGguvA7HEAgUlkknPSfZmrU41r4+SY2Na6eqb1h+KgOw+jvN\nD28PA+0TkBXHjoC7+HpryhpdNs0SOnyGoAQToWciBRRwCWKzRcWjToi48B1dwq+c\nAgQGoOryuufI3tZY99yP4DmAq02R7JP6l1G6Sm6obVpB6ZrwB8H2enfVKpWZOph5
```

**Practice Environments**: Per non dover necessariamente usare un compilatore è possibile usare degli environment nel browser che sono utili per testare velocemente i programmi. Selezionare **C** tra i linguaggi!
- **Wandbox**: [wandbox.org](https://wandbox.org/)
- **OnlineGDB**: [onlinegdb.com](https://www.onlinegdb.com/)

Articolo di Wired su **Dennis Ritchie**: [link](https://web.archive.org/web/20140702035255/https://www.wired.com/2011/10/thedennisritchieeffect/)

Libro su C: **Head First C** by David Griffiths [link oreilly](https://www.oreilly.com/library/view/head-first-c/9781449335649/)

![CBook](assets/img/HeadFirstC.jpeg)

**Recursion:** Bella Talk sulla Recursion: [Link Youtube](https://www.youtube.com/watch?v=tAKfA3Lfvi0)

Fare pratica su sololearn di quello che è stato fatto in classe con i primi due moduli di questo corso: **Basic Concepts + Conditionals and Loops + moduli 15.1 e 16.1 sulle Funzioni**
[Link Sololearn](https://www.sololearn.com/learn/courses/c-introduction)
#### Esercizio da Fare per la lezione 3: Mario
![MarioBlocks](assets/img/SuperMarioBlocks.jpeg)

Fare un programma che chiede all’utente un’altezza e restituisce una piramide ostacolo simile a quella che si trova in Super Mario. (La piramide deve essere simmetrica verticalmente) La massima altezza possibile deve essere 10.
```
//">:" Rappresenta del testo stampato dal programma 
//"<:" Rappresenta l'input dell'utente 
>: Height: 
><: -1 
>>: Height: 
<: 0 
>: Height: 
<: 90 
>: Height: 
<: 43 
>: Height: 
<: 4 
>: 
   # # 
  ## ## 
 ### ### 
#### ####
```
#### Esercizio da Fare per la lezione 4: Fibonacci Numbers
Fare un Programma che stampa un numero di fibonacci specifico
> [!info] The magic of Fibonacci numbers | Arthur Benjamin  
> [https://www.youtube.com/watch?v=SjSHVDfXHQ4](https://www.youtube.com/watch?v=SjSHVDfXHQ4)  

> [!info] The Fibonacci Sequence: Nature's Code    
> [https://www.youtube.com/watch?v=wTlw7fNcO-0](https://www.youtube.com/watch?v=wTlw7fNcO-0)  

```
//">:" Rappresenta del testo stampato dal programma
//"<:" Rappresenta l'input dell'utente
>: Find the nth fibonacci number:
<: 8
>: The 8th fibonacci number is: 21
>: Do you want to enter another number?
<: y
>: Find the nth fibonacci number:
<: 18
>: The 18th fibonacci number is: 2584
>: Do you want to enter another number?
<: N
>: Bye
```

**Game on Programming: Human Resource Machine** - [link](https://tomorrowcorporation.com/humanresourcemachine)
> _Human Resource Machine is a puzzle game. In each level, your boss gives you a job. Automate it by programming your little office worker! Don't worry if you've never programmed before - programming is just puzzle solving. If you strip away all the 1's and 0's and scary squiggly brackets, programming is actually simple, logical, beautiful, and something that anyone can understand and have fun with!_

- - -

## Git

[**Learn Git Branching**](https://learngitbranching.js.org/) - Sito interattivo per imparare i comandi git
[**Ry’s Git Tutorial**](https://johnmathews.is/rys-git-tutorial.html) - Libro facile e gratuito su git
[**Pro Git Book**](https://git-scm.com/book/en/v2) - uno dei libri più completi su git disponibile gratuitamente
[**Lezione del MIT**](https://missing.csail.mit.edu/2020/version-control/) sul Version Control
[**Git Cheat Sheets 1**](https://education.github.com/git-cheat-sheet-education.pdf) - [**Git Cheat Sheets 2**](https://about.gitlab.com/images/press/git-cheat-sheet.pdf)
Come Costruire un file **.gitignore** - [Atlassian](https://www.atlassian.com/git/tutorials/saving-changes/gitignore)
