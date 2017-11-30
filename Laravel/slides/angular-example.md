# Verwendung in Angular, Ionic

```
import {Injectable} from '@angular/core';
import {Http, Response, Headers} from "@angular/http";
import 'rxjs/add/operator/map';
import {Observable} from "rxjs";

@Injectable()
export class ApiProvider {

  constructor(private http: Http) {

  }

  getData(id: number): Observable<any> {
    return this.http.get('https://restapi.url/api/data/' + id)
      .map(
        (response: Response) => {
          return response.json().data;
        }
      );
  }
}
```