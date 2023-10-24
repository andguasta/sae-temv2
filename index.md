Per i pdf e i video delle lezione potete accedere a questa cartella Google Drive:
`U2FsdGVkX1+jPp70nWnIBk9k91YIjpgOA7KM//tF6yQG7RbluhbXkjZphgGkeBk8\nlcQJbXI88A2OfbdjO7oqb89JwtBcpNuvmBdnPVW4iLuCCPS9T+kuDgQYDWScFRA9`
### Course Software
- Unity 2020.3 Lts
    - Visual Studio
    - Unity Hub
    - Mac Build
- Wwise 2019.2.15
- Git
- Sublime Text
- Sublime Merge

### Course Program
- Introduction to Programming
- Advanced Music
- Large Project Management
- Version Control
- Game Engine Integration
- Resources Optimisation

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
`echo "U2FsdGVkX1+jPp70nWnIBk9k91YIjpgOA7KM//tF6yQG7RbluhbXkjZphgGkeBk8\nlcQJbXI88A2OfbdjO7oqb89JwtBcpNuvmBdnPVW4iLuCCPS9T+kuDgQYDWScFRA9" | openssl enc -aes256 -a -d -pbkdf2 -pass pass:password`

`echo` è un comando che viene utilizzato per visualizzare una stringa nel terminale. Ad esempio: `echo "Hello, World!"`
Questo visualizzerà `"Hello, World!"` nel terminale.