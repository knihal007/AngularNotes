## EVENT BINDING

    export class TopnevComponent implements OnInit {
      constructor() { }
      ngOnInit(): void {           //write on ts
      }
       msg:string="";
      onAddCard(){
        this.msg="your item is successfully add to card";
      }
    }
    <button (click)="onAddCard()">AddToCart</button>//write on html
    <br><br>
    <p>{{msg}}</p>

## TARGET VALUE

    constructor() { }
      ngOnInit(): void {
       }
      onInputClick(event:any){
        console.log(event.target.value);
      }
    }
    <input type="text" value="myInputText" (click)="onInputClick($event)" />
