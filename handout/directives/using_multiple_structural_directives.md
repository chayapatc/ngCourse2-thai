# การใช้งานไดเร็กทีฟแบบโครงสร้างหลายอันร่วมกัน

บางครั้งเราต้องการจะใช้ไดเร็กทีฟแบบโครงสร้างหลาย ๆ อันร่วมกัน เช่น การทำซ้ำด้วย `ngFor` แต่ต้องการเชคเงื่อนไขด้วย `ngIf` ว่าตรงกับเงื่อนไขที่กำหนดไว้หรือไม่ การใช้งานไดเร็กทีฟแบบโครงสร้างหลายอันร่วมกันสามารถสร้างผลลัพธ์ที่ไม่คาดคิดได้ อย่างไรก็ตาม Angular 2 ต้องการให้เทมเพลตสามารถผูกติดกับไดเร็กทีฟแค่อันเดียวเท่านั้น การที่จะใช้หลายไดเร็กทีฟเราจำเป็นจะต้องขยายซินแท็ก sugar หรือใช้แท็กเทมเพลตซ้อนกัน


```typescript
@Component({
  selector: 'app',
  template: `
    <template ngFor [ngForOf]="[1,2,3,4,5,6]" let-item>
      <div *ngIf="item > 3">
        {{item}}
      </div>
    </template>
  `
})
```
[ดูตัวอย่าง](https://plnkr.co/edit/3bJVnCs6n9HwA3GCh7IE?p=preview)