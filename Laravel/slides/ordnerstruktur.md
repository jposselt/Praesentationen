# Laravel Ordnerstruktur
- Der **app** Ordner enth&auml;lt den Hauptcode der Applikation
- Der **app/config** Ordner enth&auml;lt wie der Name schon sagt die Konfigurationsdateien der App
- Der **app/database** Ordner beinhaltet die Datenbank migration und seeds
- Der **public** Ordner enth&auml;lt die **index.php** welche der einstiegspunkt f&uuml;r alle Anfragen an die Applikation ist
 und Konfiguriert autloading. Dieser Ordner enth&auml;lt auch die Assets wie Bilder, JavaScript und CSS
- Der **resources** Ordner enth&auml;lt die Views sowie raw assets wie LESS, SASS oder JavaScript und alle Sprachdateien.
- Der **storage** Ordner enth&auml;lt den App Speicher sowie den cache und die von der Anwendung erzeugten Protokolle
- Der **test** Ordner enth&auml;lt die Testf&auml;lle
- Der **vendeor** Ordner enth&auml;lt die Composer Abh&auml;ngikeiten