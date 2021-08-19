# RisolutoreTetris
Risolutore automatico di tetris che, presi in input un immagine contenente uno schema, e un'immagine con dei tetramini, colloca i tetramini nel posto corrispondente.

![Schema+Scena](https://user-images.githubusercontent.com/65859032/130081496-35ea9c32-afc7-4777-9c64-42564fdd8d8d.png)

Come strumento ho utilizzato **MATLAB** con un tool per l'**image processing**
(in modo da poter riconoscere nelle immagini i tetramini e lo schema)


Con delle tecniche di elaborazione delle immagini é stato **riconosciuto** e **etichettato** singolarmente **ogni tetramino** all'interno della scena
Ed é stato poi **riconosciuto** e **etichettato** lo **schema** dove collocare gli oggetti


Successivamente é stato scritto un algoritmo che calcola la correlazione per ogni coppia tetraminoScena-tetraminoSchema e l'angolo di rotazione per ogni oggetto


Infine, se é stata trovata una **corrispondenza**, l'oggetto viene **applicato nello schema** producendo il **risultato finale**



Per il corretto funzionamento controllare la qualità delle immagini riportate in seguito.
Questo perché una loro compressione porterebbe a un cambiando del risultato della classificazione.

sfondo.jpg (5292 KB), tetramini.jpg (441 KB)


## Descrizione delle classi

main.m                 -->	main semplice del programma - creato per l'utente finale 
                            (selezione di 1 immagine di scena e 1 immagine di schema a scelta)

main_batch.m	         -->	main creato per sviluppatori, usato per testare il programma su più immagini (più settaggi disponibili)
                            per come é settato adesso considera le prime 10 scene e il primo schema
                            file usato per un controllo più dettagliato

sauvola.m	             --> 	script con implementazione dell'algoritmo di Sauvola
                            fornito dal prof. Ciocca durante le lezioni di laboratorio

quality_control.m
clicksubplot.m		     --> 	File usati per effettuare il test di accuratezza finale
analysis.mat

## Alcuni risultati ottenuti
![RisultatiOttenuti](https://user-images.githubusercontent.com/65859032/130080909-de263043-d41b-4dbb-a156-ed43cdaaf476.png)
