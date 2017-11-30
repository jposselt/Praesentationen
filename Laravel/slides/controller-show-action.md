#Controller show action

- Um auf die Show Car Seite zuzugreifen muss dann Folgende URL zugegriffen werden: http://app.url/cars/{car}
- {car} ist die ID des Car Objekts in der Datenbank Beispielsweise: http://app.url/cars/1
- Damit das Model im Controller genutzt werden kann muss Folgendes 	&uuml;ber der Controller Klasse stehen:
```
use App\Car;
```
- Die show Funktion im Controller kann man dann so Implementieren:
```
public function show($id)
  {
    $car = Car::find($id);
    return view('cars.show', array('car' => $car));
  }
```
