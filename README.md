
Progetto HTML/VueJS
Repo proj-html-vuejs
Cosa fare
Riprodurre il layout proposto solo in versione Desktop
Tecnologie da utilizzare
● HTML
● CSS / Scss
● VueJs / Vite
Requisiti tecnici minimi
Creare un progetto con Vite, strutturando il layout in almeno 3 macro-componenti: Header, Main e Footer.
Popolare le voci di menù di Header e Footer dinamicamente, tramite delle props, creando una struttura dati idonea.



###linea guida step by step del mio procedimento.

1. Visualizzo consegna grafica e tutti gli elementi necessari per riprodurre il disegno grafico in codice.
2. Posiziono l'immagine. ricevuta dal grafico su figma per ricrearmi una struttura di partenza.
quindi individuerò come struttturare L'header e la navigation bar,
le parti main del sito per poi finire con il footer.
3. creo il progetto su vue/vite e creo lo scaffolding, quindi andrò a installarele dipendenze:
fontawesome, bootstrap , scss.
4. github publish ok.
5. Elimino i file superflui
6. creo i Componenti principali che mi servono per ricreare la pagina.
Creo :
un footer.vue
un main.vue
un footer.vue
7 Popolare le voci di menù di Header e Footer dinamicamente, tramite delle props, creando una struttura dati idonea.
7.1  nello script e template di appvue collego con import header, main e footer.
7.2  nel script dei singoli file collego con export default
7.3  collego header ad figlio NavItems 
7.4  creo data e inserisco un array di oggetti che fa riferimento alla nav
7.5  nel template inserisco le parti necessarie come logo / nav items / il bottone da cliccare/ il testo statico
7.6  inserisco dello stile per il logo, il bg header, metto tutta section in display flex.
7.7  collego navitems tramite props nello script
7.8  nel template di navitems costruisco la lista di items e il button da cliccare
7.9  aggiungo dello stile sempre a navitems

8. creo dei componenti figli di Main.vue
8.1 creo la welcome section
8.2 apporto una modifica alle main section per tenere tutto in ordine creo delle cartelle per header, main e footer per tenere tutto in ordine
8.3 nella Welcome section creo un array dati
8.4 creo altre due componenti sotto main da collegare welcome section
WelcomeTitle.vue e WelcomeCard.vue







