# Analytische Funktionen in Oracle

> **Hinweis:** Analytische Funktionen gibt es auch in anderen Datenbanksystemen. Die Anweisungen
> können also auch in SQLite oder SQL Server ausgeführt werden.

Eine Datenbank ist durch das Ausführen des Scripts [sportfest.sql](sportfest.sql) mit den Daten zu einem Sportfest zu befüllen.

Die Datenbank speichert die einzelnen Bewerbe nach Abteilung, Klasse, Geschlecht und Bewerb. Die
Anzahl der Datensätze gibt folgende Tabelle an:

| S_ABTEILUNG	| S_KLASSE	| S_GESCHL	| E_BEWERB 	| SCHUELER	| ROWS	| 
| -----------	| --------	| --------	| ---------	| ---	| ----	| 
| FIT        	| 1AFIT   	| m       	| 100m Lauf	| 3  	| 30  	| 
| FIT        	| 1AFIT   	| m       	| 400m Lauf	| 3  	| 24  	| 
| FIT        	| 1AFIT   	| m       	| 5km Lauf 	| 3  	| 37  	| 
| FIT        	| 1AFIT   	| w       	| 100m Lauf	| 2  	| 17  	| 
| FIT        	| 1AFIT   	| w       	| 400m Lauf	| 2  	| 18  	| 
| FIT        	| 1AFIT   	| w       	| 5km Lauf 	| 2  	| 16  	| 
| FIT        	| 1BFIT   	| m       	| 100m Lauf	| 3  	| 35  	| 
| FIT        	| 1BFIT   	| m       	| 400m Lauf	| 3  	| 28  	| 
| FIT        	| 1BFIT   	| m       	| 5km Lauf 	| 3  	| 30  	| 
| FIT        	| 1BFIT   	| w       	| 100m Lauf	| 2  	| 22  	| 
| FIT        	| 1BFIT   	| w       	| 400m Lauf	| 2  	| 18  	| 
| FIT        	| 1BFIT   	| w       	| 5km Lauf 	| 2  	| 18  	| 
| HIF        	| 1AHIF   	| m       	| 100m Lauf	| 3  	| 31  	| 
| HIF        	| 1AHIF   	| m       	| 400m Lauf	| 3  	| 36  	| 
| HIF        	| 1AHIF   	| m       	| 5km Lauf 	| 3  	| 35  	| 
| HIF        	| 1AHIF   	| w       	| 100m Lauf	| 2  	| 25  	| 
| HIF        	| 1AHIF   	| w       	| 400m Lauf	| 2  	| 20  	| 
| HIF        	| 1AHIF   	| w       	| 5km Lauf 	| 2  	| 12  	| 
| HIF        	| 1BHIF   	| m       	| 100m Lauf	| 3  	| 33  	| 
| HIF        	| 1BHIF   	| m       	| 400m Lauf	| 3  	| 36  	| 
| HIF        	| 1BHIF   	| m       	| 5km Lauf 	| 3  	| 31  	| 
| HIF        	| 1BHIF   	| w       	| 100m Lauf	| 2  	| 24  	| 
| HIF        	| 1BHIF   	| w       	| 400m Lauf	| 2  	| 19  	| 
| HIF        	| 1BHIF   	| w       	| 5km Lauf 	| 2  	| 18  	| 
