# Verwendung in Angular, Ionic

```
import {Component, Input} from '@angular/core';
import {IonicPage, NavController, NavParams} from 'ionic-angular';
import {ApiProvider} from "../../providers/api";
import {Data} from "../../interface/data.interface";

@IonicPage()
@Component({
  selector: 'page-home',
  templateUrl: 'home.html',
})
export class HomePage {
  data: Data;

  constructor(public navCtrl: NavController, public navParams: NavParams, private api: ApiProvider) {
  }

  get(id: number) {
    this.api.getData(id)
      .subscribe(
        (data: Data) => this.data = data,
        (error: Response) => console.log(error)
      );
  }
}
```