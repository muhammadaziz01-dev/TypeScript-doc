#      TypeScript

### - **TypeScript - *2012 yilda Microsoft tomonidan taqdim etilgan dasturlash tili va JavaScript imkoniyatlarini kengaytiruvchi veb-ilovalarni ishlab chiqish vositasi sifatida joylashtirilgan. TypeScript tilini ishlab chiqaruvchisi Anders Xeylsberg bo'lib, u ilgari Turbo Pascal, Delphi va C# tillarini yaratgan.***

![Alt Text](./imgs/WHATS-TYPESCRIPT_.png)

### - **TypeScript, JavaScriptga qaraganda, dasturchilarga dasturlarini qisqa va ishonchliroq qilishda yordam beradi. Uning asosiy vazifalari quyidagilardir:**
 
  1. **Statik Tiplash: TypeScript, dasturchilarga dasturlarini yozishda xato qilish imkonini kamaytiradi. U, koding muammolarini vaqtli ravishda aniqlab beradi. Statik tiplash, dasturda aniqlik va barqarorlikni oshiradi.**

  2. **Kode Kengaytirilganligi: TypScript, dasturchilarga ob'ektlar, funksiyalar va interfeyslar kabi qo'shimcha tayplar yaratish imkonini beradi. Bu, kodni o'qish va tushuntirishni osonlashtiradi, shuningdek, tarkibiy tashqi kutubxonalarni yaratishni ham osonlashtiradi.**

  3. **ES6+ Kengaytirish: TypeScript, JavaScriptning keyingi versiyalarining ko'pini qo'llab-quvvatlaydi. Bu, dasturchilarga yangi tilda mavjud bo'lgan ko'plab imkoniyatlar, masalan, klasslar, lambda funktsiyalari, ko'p qatorli matnlar va boshqalar kabi, foydalanish imkonini beradi.**

  4. **Kode Ma'lumotlari Tizimi: TypeScript, dasturchilarga koddagi ma'lumotlarni to'g'ri ravishda ma'lumotlar tizimi sifatida qo'llash imkonini beradi. Bu, kodni nazorat qilishni osonlashtiradi va katta loyihalarda qolgan muammolarni kamaytiradi.**

  5. **Kattalashgan Proyektlar Uchun Oson To'g'ri Ishlash: TypeScript, katta qatlamli loyihalarda ishlovchi dasturchilarga yordam beradi. Katta tashqi kutubxonalarda, jamoatchilik yoki korxona muhitlarida oson tarkibiy bo'lib, kengaytirilgan ma'lumotlar modellashini yaratishga imkon beradi.**

  6. **Kodni Avtomatlashtirish: TypeScript, dasturchilarga kodni yozish va uni avtomatik ravishda ma'lumotlar tizimi sifatida foydalanish imkonini beradi. Bu, kodni yozish va uni qayta ishlashni osonlashtiradi va dasturchilarning samarali ishlashini oshiradi.**

<hr> 

###  ***TaypScript data types*** 

![Alt text](./imgs/ts-data-types.png)

 - **Boolean: true yoki false qiymatlarini qabul qiladi.**
 -  **Number: Butun sonlar va o'nlik sanoq sistemasidagi sonlar.**
 -  **String: Matnlar.**
 -  **Array: Massivlar.**
 -  **Tuple: Belgilangan tartibda bir xil tayplarga ega massivlar.**
 -  **Enum: O'zgaruvchilarni qiymatlarga murojaat qilish uchun bir** 
 -  **qisqa nom beradi.**
 -  **Any: Har qanday turdagi qiymatlarni qabul qiladi.**
 -  **Void: Agar bir funksiya hech qanday qiymat qaytarmasa.**
  -  **Null va Undefined: Bitta qiymatlar uchun.**
  -  **Never: Nimadir qaytarmaydigan funksiyalar uchun.**
  -  **Object: JS obyektlari uchun umumiy turi.**


1. **Boolean:** *Boshqa tillardagi booleantip, true yoki false qiymatlarini qabul qiladi.*

```
let isDone: boolean = false;
console.log(isDone); // false
```

2.  **Number:** *Butun va o'nlik sonlarni ifodalaydi. Masalan, 5, 10.5, -3.14 kabi.*

```
let decimal: number = 6;
let hex: number = 0xf00d;
let binary: number = 0b1010;
let octal: number = 0o744;
console.log(decimal, hex, binary, octal); // 6 61453 10 484
```

3. **String:** *Matnlar, qo'shimcha belgilar yoki satrlar. Misol uchun: "Salom", "TypScript", "123".*

```
let color: string = "blue";
color = 'red'; // Double quotes va single quotes ishlatish mumkin
console.log(color); // red
```
4. **Array:** *Massivlar, biror turdagi elementlarni o'z ichiga oladi. [1, 2, 3] yoki ['salom', 'dunyo'] kabi.*

```
let list: number[] = [1, 2, 3];
console.log(list); // [1, 2, 3]

let names: Array<string> = ['John', 'Doe'];
console.log(names); // ['John', 'Doe']
```

5. **Tuple:**  *Tartiblangan elementlarga ega massivlar. Misol uchun, [string, number] turidagi tartiblangan massivda birinchi element matn va ikkinchi element son bo'ladi.*

```
let x: [string, number];
x = ['hello', 10]; // To'g'ri
x = [10, 'hello']; // Xato
console.log(x[0].substring(1)); // ello
```
6. **Enum:** *O'zgaruvchilarni belgilash uchun ishlatiladi. Masalan, enum Color {Red, Green, Blue}. Bu, Color.Red, Color.Green, Color.Blue qiymatlariga ega bo'ladi.*

```
enum Color {Red, Green, Blue}
let c: Color = Color.Green;
console.log(c); // 1
```
7. **Any:** *Har qanday turdagi qiymatni qabul qiladi. Ammo, bu turdan foydalanish tilning dinamik xususiyatlariga qo'shimcha yuklanishga olib kelishi mumkin.*

```
let notSure: any = 4;
notSure = "maybe a string instead";
notSure = false; // Hech qanday tur qiymat qabul qiladi
console.log(notSure); // false
```

8. **Void:** *Agar funksiya hech qanday qiymat qaytarmasa, unda void turi ishlatiladi.*

```
function warnUser(): void {
    console.log("This is a warning message");
}
warnUser();
```

9. **Null va Undefined:** *Misol uchun, biror o'zgaruvchiga bosh qiymat berish uchun ishlatiladi.*

```
let u: undefined = undefined;
let n: null = null;
console.log(u, n); // undefined null
```

10. **Never:** *Ushbu turi asosan funksiyalarda ishlatiladi va u faqatgi funksiya yoki xatolikni aniqlash uchun ishlatiladi.*

```
function error(message: string): never {
    throw new Error(message);
}
error("Something went wrong");
```

11.  **Object:** *JS obyektlari uchun umumiy turi.*

```
let obj: object = {};
console.log(obj); // {}
```

12. **Symbol:** *Unikal belgilar yaratish uchun ishlatiladi.*

```
let sym1 = Symbol();
let sym2 = Symbol("key");
console.log(sym1, sym2); // Symbol() Symbol(key)
```

13. **BigInt:** *Katta butun sonlarni ifodalaydi.*

```
const bigNumber: bigint = BigInt(Number.MAX_SAFE_INTEGER) + BigInt(1);
console.log(bigNumber); // 9007199254740992n
```

