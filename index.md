---
title: TeMV2 - Material Page
subtitle: "Pagina di supporto al corso Tecniche e Metodologie dei Videogiochi 2. Docente: Andrea Guastadisegni"
cover-img: https://andguasta.github.io/sae-temv2/assets/img/oldtree_bw.png
---
[Wwise and Rclone](Wwise-Rclone.md)

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
U2FsdGVkX1/L55dQKmB7VpwFYgn4pxw/4EeoUvJPJNVvBXjDvHXQXwpC4JncLcdYMcmWdTGSugcjIdZnzix3ZoB3qgugmttniruWiF0DOxP2eeIo+W2pZymAkhXb0/jxj6sXli7L5ewHZC91SCFzvQ==\n
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
printf "password_here" | openssl enc -aes-256-cbc -a -d -pbkdf2 -pass pass:password
```
- **`printf`** è un comando che viene utilizzato per visualizzare una stringa nel terminale. Ad esempio: `printf "Hello, World!"`; Visualizzerà `"Hello, World!"` nel terminale.
- **`|`** è un operatore che viene utilizzato per prendere l'output di un comando e usarlo come input per un altro comando. Permette la concatenazione di comandi, dove l'output di un comando viene elaborato da un altro. Consente manipolazioni di dati complesse combinando comandi semplici senza la necessità di salvare risultati intermedi in un file.
- **`openssl`** è un toolkit open-source per SSL/TLS e crittografia. Offre funzionalità come comunicazione sicura, generazione di chiavi e gestione dei certificati.
- **`enc`** indica che si desidera cifrare o decifrare dei dati.
- **`-aes-256-cbc`** Specifica l'algoritmo da utilizzare, in questo caso, AES con una chiave da 256 bit con opzione **`-pbkdf2`** per usare Password-Based Key Derivation Function 2
- **`-a`** Questa opzione indica a OpenSSL di codificare l'output in base64. È utile quando i dati devono essere memorizzati e trasferiti su supporti progettati per gestire il testo.
- **`-d`** Decifra i dati in input. Senza questo flag, l'operazione predefinita sarebbe quella di cifrare.
- **`-pass pass:password`** Questo è il modo in cui si specifica la passphrase utilizzata per la cifratura o decifrazione. In questo caso, la passphrase è "password".

- - -

## Programming

Da dove viene la parola Algoritmo? - [video youtube](https://www.youtube.com/watch?v=oRkNaF0QvnI)
The Elegance of the ASCII Table - [Link](https://danq.me/2024/07/21/ascii/)

**Practice Environments**: Per non dover necessariamente usare un compilatore è possibile usare degli environment nel browser che sono utili per testare velocemente i programmi. Selezionare **C** tra i linguaggi!
- **Wandbox**: [wandbox.org](https://wandbox.org/)
- **OnlineGDB**: [onlinegdb.com](https://www.onlinegdb.com/)

Articolo di Wired su **Dennis Ritchie**: [link](https://web.archive.org/web/20140702035255/https://www.wired.com/2011/10/thedennisritchieeffect/)

Libro su C: **Head First C** by David Griffiths [link oreilly](https://www.oreilly.com/library/view/head-first-c/9781449335649/)
![CBook](assets/img/HeadFirstC.jpeg)
#### Esercizio da Fare per la lezione 3: Mario
![MarioBlocks](SAE/SAE_Websites/sae-temv2/assets/img/SuperMarioBlocks.jpeg)

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

**Game on Programming: Human Resource Machine** - [link](https://tomorrowcorporation.com/humanresourcemachine)
> _Human Resource Machine is a puzzle game. In each level, your boss gives you a job. Automate it by programming your little office worker! Don't worry if you've never programmed before - programming is just puzzle solving. If you strip away all the 1's and 0's and scary squiggly brackets, programming is actually simple, logical, beautiful, and something that anyone can understand and have fun with!_

#### Talk da Guardare:
> The Art of Code - Dylan Beattie  
> Software and technology has changed every aspect of the world we live in. At one extreme are the 'mission critical' applications - the code that runs our banks, our hospitals, our airports and phone networks. Then there's the code we all use every day to browse the web, watch movies, create spreadsheets...  
> [https://www.youtube.com/watch?v=6avJHaC3C2U](https://www.youtube.com/watch?v=6avJHaC3C2U)  

---
### MIDI Lesson

Consultare Capitolo 4 da **Audio Engineer's Reference Book** by **Michael Talbot-Smith** su Material Page

Video su come funzionano i numeri **Binari**
- Representing Numbers and Letters with Binary: Crash Course Computer Science [https://www.youtube.com/watch?v=1GSjbWt0c9M](https://www.youtube.com/watch?v=1GSjbWt0c9M)  

Video su cosa sono le **Logic Units**
- How Computers Calculate - the ALU: Crash Course Computer Science [https://www.youtube.com/watch?v=1I5ZMmrOfnA](https://www.youtube.com/watch?v=1I5ZMmrOfnA)  

Come costruire un **Logic Gate** con i **Transistors**
- Making logic gates from transistors [https://www.youtube.com/watch?v=sTu3LwpF6XI](https://www.youtube.com/watch?v=sTu3LwpF6XI)  

**Layers** in Protocols
- OSI model [https://en.wikipedia.org/wiki/OSI_model](https://en.wikipedia.org/wiki/OSI_model)  

**Midi Files Structure** from Stanford
- [https://ccrma.stanford.edu/~craig/14q/midifile/MidiFileFormat.html](https://ccrma.stanford.edu/~craig/14q/midifile/MidiFileFormat.html)  

More on **Midi Files** and **Midi**
- Musical Instrument Digital Interface (MIDI) [https://www.recordingblogs.com/wiki/musical-instrument-digital-interface-midi](https://www.recordingblogs.com/wiki/musical-instrument-digital-interface-midi)
- Standard MIDI file format [http://www.music.mcgill.ca/~ich/classes/mumt306/StandardMIDIfileformat.html](http://www.music.mcgill.ca/~ich/classes/mumt306/StandardMIDIfileformat.html)

- - -
### 5.Bash & Bash Tools

![NeverSpend](SAE/SAE_Websites/sae-temv2/assets/img/NeverSpend5minuts.jpeg)
**The Linux Command Line: A Complete Introduction Book by William E. Shotts**
Online Edition:
> [!info] LinuxCommand.org: Learning the shell.  
> Why do you need to learn the command line anyway? Well, let me tell you a story. Many years ago we had a problem where I worked. There was a shared drive on one of our file servers that kept getting full. I won't mention that this legacy operating system did not support user quotas; that's another story.  
> [https://linuxcommand.org/lc3_learning_the_shell.php](https://linuxcommand.org/lc3_learning_the_shell.php)  

Free PDF Download: [https://sourceforge.net/projects/linuxcommand/](https://sourceforge.net/projects/linuxcommand/)  

**SOX - The Swiss Army knife of sound processing programs**
> _SoX is a cross-platform (Windows, Linux, MacOS X, etc.) command line utility that can convert various formats of computer audio files in to other formats. It can also apply various effects to these sound files, and, as an added bonus, SoX can play and record audio files on most platform_

[http://sox.sourceforge.net/](http://sox.sourceforge.net/)  

**youtube-dl**

> _Command-line program to download videos from YouTube.com and other video sites_
[https://github.com/ytdl-org/youtube-dl/](https://github.com/ytdl-org/youtube-dl/)  

**FFmpeg**
> _A complete, cross-platform solution to record, convert and stream audio and video._
[https://www.ffmpeg.org/download.html](https://www.ffmpeg.org/download.html)  

- - -
### 6.Markup Languages

From Material Folder:
- Consult: Chapter 1 di **XML in a Nutshell**
- Consult: Chapter 12 from **How Computer Really Work**

**Sublime Text Editor** [https://www.sublimetext.com/](https://www.sublimetext.com/)  

**GUID Generator **[https://www.guidgenerator.com/](https://www.guidgenerator.com/)
> [!info] Universally unique identifier - Wikipedia  
> A universally unique identifier ( UUID) is a 128-bit label used for information in computer systems. The term globally unique identifier ( GUID) is also used, often in software created by Microsoft. When generated according to the standard methods, UUIDs are, for practical purposes, unique.  
> [https://en.wikipedia.org/wiki/Universally_unique_identifier](https://en.wikipedia.org/wiki/Universally_unique_identifier)  

> [!info] Pigeonhole principle - Wikipedia  
> In mathematics, the pigeonhole principle states that if items are put into containers, with , then at least one container must contain more than one item.[1] For example, if one has three gloves (and none is ambidextrous/reversible), then there must be at least two right-handed gloves, or at least two left-handed gloves, because there are three objects, but only two categories of handedness to put them into.  
> [https://en.wikipedia.org/wiki/Pigeonhole_principle](https://en.wikipedia.org/wiki/Pigeonhole_principle)  

**History of XML** [https://www.youtube.com/watch?v=RH0o-QjnwDg](https://www.youtube.com/watch?v=RH0o-QjnwDg)  

**XML Specification** [https://www.xml.com/axml/axml.html](https://www.xml.com/axml/axml.html)  

- - -
### Files and Files System

Video ben fatto su come funzionano i **File e i File Systems**  https://youtu.be/KN8YgJnShPM  

**Wav Header**

> [!info] WAV - Waveform Audio File Format  
> WAV, known for WAVE (Waveform Audio File Format), is a subset of Microsoft's Resource Interchange File Format (RIFF) specification for storing digital audio files. The format doesn't apply any compression to the bitstream and stores the audio recordings with different sampling rates and bitrates.  
> [https://docs.fileformat.com/audio/wav/](https://docs.fileformat.com/audio/wav/)  

> [!info] Microsoft WAVE soundfile format  
> The WAVE file format is a subset of Microsoft's RIFF specification for the storage of multimedia files. A RIFF file starts out with a file header followed by a sequence of data chunks.  
> [http://soundfile.sapp.org/doc/WaveFormat/](http://soundfile.sapp.org/doc/WaveFormat/)  

- - -
## Git

[**Learn Git Branching**](https://learngitbranching.js.org/) - Sito interattivo per imparare i comandi git

[**Ry’s Git Tutorial**](https://johnmathews.is/rys-git-tutorial.html) - Libro facile e gratuito su git

[**Pro Git Book**](https://git-scm.com/book/en/v2) - uno dei libri più completi su git disponibile gratuitamente

[**Lezione del MIT**](https://missing.csail.mit.edu/2020/version-control/) sul Version Control

[**Git Cheat Sheets 1**](https://education.github.com/git-cheat-sheet-education.pdf) - [**Git Cheat Sheets 2**](https://about.gitlab.com/images/press/git-cheat-sheet.pdf)

Come Costruire un file **.gitignore** - [Atlassian](https://www.atlassian.com/git/tutorials/saving-changes/gitignore)
```
#Questo è un esempio di gitignore che si può usare in un progetto Wwise
*.prof
*.akd
*.validationcache
GeneratedSoundBanks
.cache
.backup
*.crossover.wsettings
AutoDetectedSampleRates.cache
.DS_Store
```

I commit git hanno un numero esadecimale che li identifica in maniera univoca. Quel numero è un hash del contenuto del commit. Sul concetto di hash nel contesto delle password c’è questo video interessante: [How NOT to Store Passwords! - Computerphile](https://www.youtube.com/watch?v=8ZtInClXe1Q)

Come gestire i branch: [**A successful Git branching model**](https://nvie.com/posts/a-successful-git-branching-model/)

- - -
### Unity Material
Questo è del materiale aggiuntivo utile per approfondire Unity:
**Unity Essentials - Corso Introduttivo Ufficiale di Unity**  
[https://learn.unity.com/pathway/unity-essentials](https://learn.unity.com/pathway/unity-essentials)  
**Junior Programmer - Corso Ufficiale sullo scripting ed altro**  
[https://learn.unity.com/pathway/junior-programmer](https://learn.unity.com/pathway/junior-programmer)  
**Complete C# Unity Game Developer 3D - Corso ben fatto e a poco prezzo su Udemy**  
[https://www.udemy.com/course/unitycourse2/](https://www.udemy.com/course/unitycourse2/)

**Script Lifecycle** flowchart
- Order of execution for event functions [https://docs.unity3d.com/Manual/ExecutionOrder.html](https://docs.unity3d.com/Manual/ExecutionOrder.html)

- - -