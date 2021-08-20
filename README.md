# RisolutoreTetris
Risolutore automatico di tetris che, presi in input un immagine contenente uno schema, e un'immagine con dei tetramini, colloca i tetramini nel posto corrispondente.

![Schema+Scena](https://user-images.githubusercontent.com/65859032/130081496-35ea9c32-afc7-4777-9c64-42564fdd8d8d.png)

Come strumento ho utilizzato **MATLAB** con un tool per l'**image processing** <br/> 
(in modo da poter riconoscere nelle immagini i tetramini e lo schema)

Con delle tecniche di elaborazione delle immagini é stato **riconosciuto** e **etichettato** singolarmente **ogni tetramino** all'interno della scena <br/>
Ed é stato poi **riconosciuto** e **etichettato** lo **schema** dove collocare gli oggetti

Successivamente é stato scritto un algoritmo che calcola la correlazione per ogni coppia tetraminoScena-tetraminoSchema e l'angolo di rotazione per ogni oggetto

Infine, se é stata trovata una **corrispondenza**, l'oggetto viene **applicato nello schema** producendo il **risultato finale**


Per il corretto funzionamento controllare la qualità delle immagini riportate in seguito. <br/>
*Questo perché una loro compressione porterebbe a un cambiando del risultato della classificazione*

**sfondo.jpg (5292 KB), tetramini.jpg (441 KB)**


## Descrizione delle classi

main.m                 -->	main semplice del programma - creato per l'utente finale. 
                            *Selezione di 1 immagine di scena e 1 immagine di schema*

main_batch.m	         -->	main creato per sviluppatori, usato per testare il programma su più immagini (più settaggi disponibili).
                            *Per come é settato adesso considera le prime 10 scene e il primo schema*

sauvola.m	             --> 	script con implementazione dell'algoritmo di Sauvola

quality_control.m, clicksubplot.m, analysis.mat --> File usati per effettuare il test di accuratezza finale


## Alcuni risultati ottenuti
![RisultatiOttenuti](https://user-images.githubusercontent.com/65859032/130272557-262edda8-161f-484c-8896-70e816fcc0c7.png)
