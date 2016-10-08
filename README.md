# IlPostSlidesKiller
#Cos'è?
IlPost sta piano piano trasformando metà dei suoi articoli in slides in cui devi continuare a cliccare per visualizzarne i contenuti.
Il seguente codice Javascript è fatto per essere inserito in una bookmarklet nei preferiti o da eseguire nella console del browser per
eliminare la slide e permettere di vedere tutto l'articolo in colonna.

#Come si fa?
Crea una bookmarklet nella tua barra dei preferiti del tuo browser, dalle il nome che preferisci (La mia si chiama FuckPostSlides) e
nel campo URL inserisci il seguente script:

javascript:var d=document.getElementsByClassName('swiper-wrapper');
var c=document.getElementsByClassName('swiper-container');var at=document.getElementsByClassName('art_tag');
var ct=document.getElementsByClassName('controlli');d[0].classList.remove('swiper-wrapper');
c[0].classList.remove('swiper-container');var n=document.getElementsByClassName('new-comments');
var f=document.getElementsByTagName('footer');n[0].setAttribute('style','position:absolute;left:-5000px');
f[0].setAttribute('style','position:absolute;left:-5000px');f[1].setAttribute('style','position:absolute;left:-5000px');
at[0].setAttribute('style','position:absolute;left:-5000px');ct[1].setAttribute('style','position:absolute;left:-5000px');
ct[0].setAttribute('style','position:absolute;left:-5000px');

Una volta creata la bookmarklet, vai sull'articolo incriminato e premila. Si trasformerà in un articolo in colonna senza noiosi bottoni.

Altrimenti puoi andare sull'articolo incriminato, premere f12. Ti si aprirà una finestra, clicca su "console" e copincolla il seguente script:

var d=document.getElementsByClassName('swiper-wrapper');var c=document.getElementsByClassName('swiper-container');
var at=document.getElementsByClassName('art_tag');var ct=document.getElementsByClassName('controlli');
d[0].classList.remove('swiper-wrapper');c[0].classList.remove('swiper-container');
var n=document.getElementsByClassName('new-comments');var f=document.getElementsByTagName('footer');
n[0].setAttribute('style','position:absolute;left:-5000px');f[0].setAttribute('style','position:absolute;left:-5000px');
f[1].setAttribute('style','position:absolute;left:-5000px');at[0].setAttribute('style','position:absolute;left:-5000px');
ct[1].setAttribute('style','position:absolute;left:-5000px');ct[0].setAttribute('style','position:absolute;left:-5000px');

Premi invio e il gioco è fatto.
Lo script non fa altro che togliere gli articoli dagli slide, metterli in colonna, eliminare la sezione commenti e i footer per permetterne la visualizzazione.
