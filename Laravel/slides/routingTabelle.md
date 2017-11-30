# Routes

In der Konfigurationsdatei **app/Http/routes.php** muss folgendes hinzugefügt werden:
```
Route::resource('cars', 'CarController');
```
Diese eine Zeile reicht aus um alle routes der Car resource zu definieren

| Request Type | Path             | Action  | Route Name   |
|--------------|------------------|---------|--------------|
| GET          | /cars            | index   | cars.index   |
| GET          | /cars/create     | create  | cars.create  |
| POST         | /cars            | store   | cars.store   |
| GET          | /cars/{car}      | show    | cars.show    |
| GET          | /cars/{car}/edit | edit    | cars.edit    |
| PUT/PATCH    | /cars/{car}      | update  | cars.update  |
| DELETE       | /cars/{car}      | destroy | cars.destroy |

