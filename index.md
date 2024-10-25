---
title: TeMV2 - Material Page
subtitle: "Pagina di supporto al corso Tecniche e Metodologie dei Videogiochi 2. Docente: Andrea Guastadisegni"
thumbnail-img: https://andguasta.github.io/sae-temv2/assets/img/CourseImage.png
cover-img: https://andguasta.github.io/sae-temv2/assets/img/Animal_Header1.png
---
| *Course* Software | Course Program              |
| ----------------- | --------------------------- |
| Unity 2020.3 Lts  | Introduction to Programming |
| - Visual Studio   | Advanced Music              |
| - Mac Buils       | Large Project Management    |
| Wwise 2022.1      | Version Control             |
| Git               | Game Engine Integration     |
| Sublime Text      | Resources Optimisation      |
| Sublime Merge     |                             |

- - -

Per i **Video** delle lezione e alcuni **Pdf** utili potete accedere a questa cartella Google Drive:
```
U2FsdGVkX19s1UUZgkZ1ENbJqFhjzFvtWuvTDRp9/FDp1EROba7csviILxIlZULT\nVLyDjl+k1HPSDoNUxXYlCvo8Brm7zUweopDCPBKBWIWSSuXqCFfYlwt7e7D9sN0m\nqsixT1C+El057EoCe0PkWQ==
```
---

## Books
### Technical Books
- **Code: The Hidden Language of Computer Hardware and Software** by Charles Petzold [link goodreads](https://www.goodreads.com/book/show/44882.Code)
    - Come funzionano i computer partendo dai componenti
- **Designing Sound** by Andy Farnell [link mitpress](https://mitpress.mit.edu/books/designing-sound)
    - Procedural Audio and Synthesis
    - Accessibile come studenti SAE nella e-library
- **The Audio Programming Book** by Richard Boulanger and Victor Lazzarini [link mitpress](https://mitpress.mit.edu/9780262014465/the-audio-programming-book/)
    - Come si utilizza C nell'audio e come si implementano effetti e sintesi.
- **Microsound** By Curtis Roads [link mitpress](https://mitpress.mit.edu/9780262681544/microsound/)
    - Sulla sintesi Granulare
    - Accessibile come studenti SAE nella e-library
- **The Computer Music Tutorial** By Curtis Roads [link mitpress](https://mitpress.mit.edu/9780262680820/the-computer-music-tutorial/)
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
printf "Received string here" | openssl enc -aes-256-cbc -md sha256 -pbkdf2 -a -d -pass pass:password
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