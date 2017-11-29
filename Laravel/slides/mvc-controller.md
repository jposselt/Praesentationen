# MVC (Controller)
- Implementiert die Anwendungslogik
- Verarbeitet Usereingaben, empfangene Daten mithilfe von Models
- Es gibt einen Hauptcontroller von dem alle anderen Controller erben
- Neuen Controller erstellen:
	```
	$ php artisan make:controller CarController 
	```
	der Befehl Erstellt einen Controller mit allen typischen CRUD Aktionen
- Jetzt müssen nur noch die Routes definiert werden um die URLs mit den Controller aktionen zu verbinden