# RisolutoreTetris
Risolutore automatico di tetris che, presi in input un immagine contenente uno schema, e un'immagine con dei tetramini, piazza i tetramini nel posto corrispondente.

Per il corretto funzionamento controllare la qualità delle immagini riportate in seguito.
Questo perché una loro compressione porterebbe a un cambiando del risultato della classificazione.

sfondo.jpg		5292 KB
tetramini.jpg 		441 KB


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
