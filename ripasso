Gradino 1 · Leggi il codice (1 punto ciascuno)
1. Più classi. Per ogni paragrafo scrivi di che colore è e se è in grassetto.
<p class="nota">A</p>
<p class="nota importante">B</p>
<p class="importante">C</p>
<p id="nota">D</p>

.nota { color: green; }
.importante { font-weight: bold; }
RISPOSTE:
primo paragrafo: colore verde no grassetto
secondo paragrafo: verde e in grassetto
terzo paragrafo: non colorato ma in grassetto
quarto paragrafo: nessuno dei due (l'id non è stato detto nel css)


2. Il colore dei link. Di che colore sono il link e la scritta Testo?
<nav><a href="chi-sono.html">Chi sono</a> <span>Testo</span></nav>

nav { color: white; background: #003366; }
RISPOSTE:
Il link è di colore blu
Testo è di colore bianco


3. Il tipo del commit. Scegli tra feat, fix, style e docs, e scrivi il messaggio completo:
   a) hai cambiato il colore di sfondo della testata;
   b) hai sistemato i rientri di stile.css, e a schermo non cambia niente;
   c) hai corretto un link che portava a una pagina che non esiste;
   d) hai aggiunto un paragrafo al README.
RISPOSTE
a)feat
b)style
c)fix
d)docs

4. Markdown. Che cosa producono queste righe in un file .md?
# Missione
## Obiettivi
- prima voce
**importante**
  RISPOSTE:
  # Missione = titolo
  ## Obbiettivi = sottotitolo
  - prima voce = inzio di un elenco puntato con scritto prima voce
  **importante** = importante scritto in grassetto

5. Colori. Che colore è #00ffff? Quali componenti (rosso, verde, blu) sono al massimo?
componenti al massimo : verde e blu
colore: ciano



6. Commit senza add. Hai modificato stile.css e scrivi subito git commit -m "feat: testo rosso", senza git add.
 Che cosa risponde Git? Il commit contiene la modifica?
risponde che non esiste un file per attribuire la modifica, quindi il commit non viene fatto.
Logicamente quindi il commit non contiene la modifica.


Gradino 2 · Spiega in breve (2 punti ciascuno)


7. Due errori. Il paragrafo è nero, normale e non in corsivo. Trova i due errori, spiega perché ognuno impedisce la regola, e correggili.


<p class="nota importante">Avviso</p>

nota { color: green }
.importante { font-weight: bold font-style: italic; }

CORREZIONE:

primo errore: .nota (va messo il . prima di nota essendo una classe, viene definita così in css, sennò html cerca il tag nota inesistente)
secondo errore: il punto e virgola dopo green e dopo bold (perché così dividi le istruzioni, se non li mettessi html leggerebbe tutto in uno, e quindi non viene data alcuna istruzione)

CODICE CORRETTO:
<p class="nota importante">Avviso</p>

.nota { color: green; }
.importante { 
  font-weight: bold; 
  font-style: italic; 
  }

8. Mostrare il codice. In una pagina vuoi mostrare, come testo, il codice <a href="x.html">link</a>.
   Scrivi l'HTML e spiega perché serve.
   Che cosa mostra il browser se scrivi &amp;lt;?

  RISPOSTE:
  codice scritto:
  %lta href="x.html"%gtlink&lt/a&gt
  serve per far in modo che non diventi un link cliccabile, ma solo un qualcosa da vedere nel sito.
  se scrivessi &amp;lt; verrebbe vuori solo &lt.

9. add, poi ancora una modifica. Modifichi stile.css, scrivi git add stile.css, poi modifichi di nuovo stile.css e scrivi git commit -m "feat: testo rosso".
    Che cosa c'è nel commit? Che cosa mostra dopo git status? Che cosa devi fare per registrare anche la seconda modifica?
Nel commit c'è solo la prima modifica.
dopo il git status viene scritto che non si hanno elementi necessari per fare il commit.
per registrare anche la seconda modifica bisogna ripetere il processo (quindi rifare git add e poi il commit)

Gradino 3 · Ragiona (4 punti ciascuno)
10. Due cartelle più giù. Nessuno dei quattro riferimenti di pagine/progetti/robot.html funziona. 
Per ognuno scrivi quale file cerca il browser, perché non c'è, e la correzione. Poi scrivi la regola che usi per contare i ../.
sito/
├── index.html
├── stile.css
├── img/logo.png
└── pagine/
    ├── chi-sono.html
    └── progetti/robot.html

<!-- pagine/progetti/robot.html -->
<link rel="stylesheet" href="../stile.css">
<img src="../img/logo.png" alt="Logo">
<a href="index.html">Home</a>
<a href="chi-sono.html">Chi sono</a>

CORREZIONE:

<!-- pagine/progetti/robot.html -->
<link rel="stylesheet" href="../../stile.css">
<img src="../../img/logo.png" alt="Logo">
<a href="../../index.html">Home</a>
<a href="../chi-sono.html">Chi sono</a>

REGOLA:
ogni ../ fa arrivare alla casella precedente, quindi, se io mi trovo in robot.html (che è dentro progeti/) con un ../ arriverò in pagine/ e con un altro arriverò in sito/.

11. Un nav leggibile. In pagine/chi-sono.html il nav ha lo sfondo #003366. 
I link devono essere grigio chiaro e senza sottolineatura; quello della pagina in cui ti trovi, bianco e sottolineato. 
