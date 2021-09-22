# InfoLing-SchenkKlitschkov
Abschlussprojekt Cryptocurrency QA

Crawl_Wiki enthält den Code der für das erstellen der Wissensbasis gebraucht wurde. Das Programm crawlt alle Wikipedia Artikel die im Artikel zu Bitcoin verlinkt sind und gibt sie als txt. Dateien zurück. 

Einige der txt. Dateien hatte Namen die zu Fehlern beim Einfügen in die ES Datenbank führen, diese wurden manuell behoben. Die funktionierenden Dateien finden sich in fixed_txt_files.zip.

Fixed_txt_files.zip enthält alle Dokumente die von Wikipedia gecrawled wurden und die Wissensbasis des QA Systems darstellen. Solange sie im gleichen Ordner wie das Notebook abgelegt sind, muss nichts weiter vorbereitet werden.

Scrape_Questions ist der Code in dem eine beliebte online Q&A nach Fragen durchsurcht wird, und diese in einer txt. Datei abgespeichert wird. Diese datei ist bereits im repository, unter dem namen questions.txt
