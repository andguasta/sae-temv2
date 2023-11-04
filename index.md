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
U2FsdGVkX1+jPp70nWnIBk9k91YIjpgOA7KM//tF6yQG7RbluhbXkjZphgGkeBk8\nlcQJbXI88A2OfbdjO7oqb89JwtBcpNuvmBdnPVW4iLuCCPS9T+kuDgQYDWScFRA9
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
printf "Received String Here" | openssl enc -aes256 -a -d -pbkdf2 -pass pass:password
```


- **`printf`** è un comando che viene utilizzato per visualizzare una stringa nel terminale. Ad esempio: `printf "Hello, World!"`; Visualizzerà `"Hello, World!"` nel terminale.
- **`|`** è un operatore che viene utilizzato per prendere l'output di un comando e usarlo come input per un altro comando. Permette la concatenazione di comandi, dove l'output di un comando viene elaborato da un altro. Consente manipolazioni di dati complesse combinando comandi semplici senza la necessità di salvare risultati intermedi in un file.
- **`openssl`** è un toolkit open-source per SSL/TLS e crittografia. Offre funzionalità come comunicazione sicura, generazione di chiavi e gestione dei certificati.
- **`enc`** indica che si desidera cifrare o decifrare dei dati.
- **`-aes256`** Specifica l'algoritmo da utilizzare, in questo caso, AES con una chiave da 256 bit.
- **`-a`** Questa opzione indica a OpenSSL di codificare l'output in base64. È utile quando i dati devono essere memorizzati e trasferiti su supporti progettati per gestire il testo.
- **`-d`** Decifra i dati in input. Senza questo flag, l'operazione predefinita sarebbe quella di cifrare.
- **`pbkdf2`** PBKDF2 (Password-Based Key Derivation Function 2) è un metodo utilizzato per trasformare una password in una chiave più lunga e sicura. Lo fa mescolando e elaborando ripetutamente la password, rendendo più difficile per gli aggressori indovinare la password originale anche se hanno la chiave risultante.
- **`-pass pass:password:`** Questo è il modo in cui si specifica la passphrase utilizzata per la cifratura o decifrazione. In questo caso, la passphrase è "password".

- - -

## Lesson 1

Slides:
```
U2FsdGVkX1/RjAvgZs+jg+AVfLZPJEAkaCi3d/9X+5EZBEKcB7uRCRQ10wz21mRF\nPKi98zj3B5MIfm+a9cXVOLexamfkfXHIguLYSRaIJizZoAy7y4TbW/Zf+vXt4Hdh\nAjzsUVw8uScEErkx5AjZ2MD7cUnPPAn0ynRC3L8+3fy9tmbUR3Gi4HDBtMIijkGz\nlU9GPez/vsmFYSxyul6kTw8ckiunZMbMAN/nhjGH6vma0b0fWpXAq6etRvzdSuZA
```

**Practice Environments**: Per non dover necessariamente usare un compilatore è possibile usare degli environment nel browser che sono utili per testare velocemente i programmi. Selezionare **C** tra i linguaggi!
- **Wandbox**: [wandbox.org](https://wandbox.org/)
- **OnlineGDB**: [onlinegdb.com](https://www.onlinegdb.com/)

Libro su C: **Head First C** by David Griffiths
[link oreilly](https://www.oreilly.com/library/view/head-first-c/9781449335649/)

![CBook](assets/img/HeadFirstC.jpeg)

Articolo di Wired su **Dennis Ritchie**: [link](https://web.archive.org/web/20140702035255/https://www.wired.com/2011/10/thedennisritchieeffect/)

