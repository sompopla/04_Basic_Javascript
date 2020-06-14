## CodeCamp#6 Online

## Sompop Laya
<hr>

### Lab 1 : การตั้งชื่อตัวแปรที่ดี

+ Lab 1
    + ให้ประกาศชื่อตัวแปร human และ name
    + ใส่ชื่อตัวเองลงบนตัวแปร name
    + นำค่าที่อยู่ในตัวแปร name ไปใส่ให้ human
    + เมื่อ console.log(human) ออกมาเป็นชื่อตัวเอง

```javascript
    let myHuman;
    let myName;
    name = "Sompop";
    human = name;
    console.log(human); 
```
<hr>

### Lab 2 : การตั้งชื่อตัวแปรที่ดี
    
 + Lab 2
    + ตั้งชื่อตัวแปรที่ใช้เก็บจำนวนเงินในกระเป๋าของคุณ
    + ตั้งชื่อตัวแปรที่ใช้เก็บชื่อของ พ่อและแม่ของคุณ
    + ตั้งชื่อตัวแปรเก็บที่อยู่ของคุณ
    + ตั้งชื่อตัวแปรที่ใช้เก็บอายุจักรวาล

```javascript
    let myWallet;
    let myFather;
    let myMother;
    let myAddress;
    let ageUniverse;
```
<hr>

### Exercise 1 : ตัวแปรและประเภทของข้อมูล

+ ผลลัพธทั้ง console.log ทั้งสามคืออะไร ?
    

```javascript
    let name = "Codecamp";
    console.log(`hello ${1}`); // 1
    console.log(`hello ${"name"}`); // name
    console.log(`hello ${name}`); // Codecamp
```
<hr>

### Exercise 2 : ตัวแปรและประเภทของข้อมูล

+ 2.1 กำหนดตัวแปรสำหรับเก็บชื่อ และกำหนดค่าเริ่มต้นเป็นชื่อของผู้เรียน
+ 2.2 กำหนดตัวแปรสำหรับเก็บอายุ และกำหนดค่าเริ่มต้นเป็นอายุของผู้เรียน
+ 2.3 กำหนดตัวแปรสำหรับเก็บที่อยู่ และกำหนดค่าเริ่มต้นเป็นที่อยู่ของผู้เรียน
+ 2.4 กำหนดตัวแปรสำหรับเก็บประวัติของนักเรียนโดยใช้ตัวแปรทั้ง 3 ตัวด้านบนประกอบการเขียนประวัตินี้ด้วย

```javascript
    const myName = "Sompop Laya";
    const myAge = "300";
    const myAddress = "Nonthaburi";
    const myProfile = myName + myAge "ปี" + myAddress;
```
<hr>

### แบบฝึกหัด : การดำเนินการเบื้องต้น

+ ให้ระบุค่าของ a,b,c และ d หลังจบ statement ทั้งหมด

```javascript
    let a = 1, b = 1;
    let c = ++a;
    let d = b++;

    ตอบ.
    a = 1;
    b = 1;
    c = 2;
    d = 1;
```
+ จงหาผลลัพธ์ของ statement ดังต่อไปนี้

```javascript
    1. "" + 1 + 0;      // 10
    2. "" - 1 + 0;      // -1
    3. true + false;    // 1
    4. 6 / "3";         // 2
    5. "2" * "3";       // 6
    6. 4 + 5 + "px";    // "9px"
    7. "$" + 4 + 5;     // "$45"
    8. "4" - 2;         // 2
    9. "4px" - 2;       // NaN
    10. 7 / 0           // Infinity
    11. " -9 " + 5;     // " -9 5"
    12. " -9 " - 5;     // -14
    13. null + 1;       // 1
    14. undefined + 1;  // NaN
    15. " \t \n" - 2;   // -2
```

<hr>

### แบบฝึกหัด : การเปรียบเทียบ

+ จงหาค่าเปรียบเทียบต่อไปนี้

```javascript
    - 5 > 4                     // true
    - "apple" > "pineapple"     // false
    - "2" > "12"                // true
    - undefined == null         // true
    - undefined === null        // false
    - "bee" < "be"              // flase
    - "bee" > "Bee"             // true
    - "Bee" < "be"              // true
```

<hr>

### แบบฝึกหัด : การเขียนเงื่อนไข

+ 1.Browser จะโชว์ข้อความ "Hello Codecamp #5" ไหม

```javascript
    ตอบ. แสดง "Hello Codecamp #5"
```

+ 2.ใช้ if else ในการเขียนถามชื่อของคุณ
    + ถ้าตอบถูกให้แสดงคำว่า "เก่งมาก"
    + ถ้าตอบผิดให้แสดงคำว่า "คุณไม่รู้จักชื่อฉัน"

```javascirpt
    let myName = prompt("ชื่อคุณคืออะไร ?","tum");
    if(myName == "tum") {
        alert("เก่งมาก");
    }else{
        alert("คุณไม่รู้จักชื่อฉัน") 
    }
```

+ 3.ใช้ prompt ในการรับคะแนนมาคำนวนเกรด
    + ถ้าคะแนน มากกว่าเท่ากับ 80 ได้ A
    + ถ้าคะแนน อยู่ระหว่าง 70 - 79 	ได้ B
    + ถ้าคะแนน อยู่ระหว่าง 60 - 69 	ได้ C
    + ถ้าคะแนน อยู่ระหว่าง 50 - 59 	ได้ D
    + ถ้าคะแนน น้อยกว่า 50 ได้ F

```javascript
    let myScore = prompt("คุณได้คะแนนสอบเท่าไร ?","77");
    if(myScore < 50) {
        alert("คุณได้เกรด F");
    }else if(myScore <= 59) {
        alert("คุณได้เกรด  D");
    }else if(myScore <= 69) {
        alert("คุณได้เกรด  C");
    }else if(myScore <= 79) {
        alert("คุณได้เกรด  B");
    }
        alert("คุณได้เกรด A");
```

+ 4.เปลี่ยน if-else ข้างล่างในอยู่ในรูปของ Ternary Operators

```javascript
    let age = prompt('How old are you ?');
    let price;
    if(age < 18) {
        price = 2000;
    }else{
        price = 3500;
    }

    //Ternary Operators
    price = (age < 18) ? price = 2000 : price = 3500;

    alert(price);
```