# InfoLing-SchenkKlitschkov
# Abschlussprojekt Cryptocurrency QA


Im Rahmen des Informations Linguistik haben wir uns für das Abschlussprojekt ein QA-System ausgesucht, dass dabei helfen soll, Fragen zum Thema Kryptowährung aus einer Sammlung von Wikipedia Beträgen, zu beantworten. 

## Information zu den Daten im Repository
Scrape_Articles enthält den Code der für das erstellen der Wissensbasis gebraucht wurde. Das Programm crawlt alle Wikipedia Artikel die im Artikel zu Bitcoin verlinkt sind und gibt sie als txt. Dateien zurück. Die Dateien sind bereits im repository, der Code muss also nicht ausgeführt werden.

Fixed_txt_files.zip enthält alle Dokumente die von Wikipedia gecrawled wurden und die Wissensbasis des QA Systems darstellen. Solange sie im gleichen Ordner wie das Notebook abgelegt sind, muss nichts weiter vorbereitet werden. Einige der txt. Dateien hatte Namen die zu Fehlern beim Einfügen in die ES Datenbank führen, diese wurden bereits manuell behoben.

Scrape_Questions ist der Code in dem eine beliebte online Q&A nach Fragen durchsurcht wird, und diese in einer txt. Datei abgespeichert werden. Diese Datei ist bereits im repository, unter dem namen questions.txt

Die answers.json Datei wird nur gebraucht falls man den Reader mit Annotierten Antworten trainiern will.


## Wie starte ich das Programm
Das Python-Script kann durch das Aufrufen des Links von Google Collab in der Datei Crypto_QA.ipynb gestartet werden. Es empfielt sich dieses nur in der Umgebung auszuführen und nicht auf Plattformen wie Jupiter Notebook, da dies mit fehlgeschlagenen Imports von Libraries einhergehen würde. 

## Mögliche Probleme und wie man diese behebt 
### Problem: Haystack Libraries 

Es ist möglich, dass es einen Error geworfen wird, wenn zum ersten Mal die Haystack Libraries importiert werden sollen(siehe Screenshot). Dieses lässt sich beheben nochmal der Code für den Import erneut ausführt. 
![problem_haystack_import](https://github.com/Thekowo/InfoLing-SchenkKlitschkov/blob/main/problem_haystack_import.PNG)
### Nicht importiertes Zip File 

Das FileNotFound Error welcher geworfen wird (wie im Screenshot), deutet darauf hin, dass noch kein zip-File mit den entsprechenden Daten importiert wurde. Das lässt mit dem Import des in github mitaufgeführten txt-files.zip per z.B  Drag and Drop und erneute ausführen des Codes beheben
![zip_file_problem](https://github.com/Thekowo/InfoLing-SchenkKlitschkov/blob/main/zip_file_problem.PNG)
