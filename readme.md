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
    const myAge = "31";
    const myAddress = "Nonthaburi";
    const myProfile = myName + myAge "ปี" + myAddress;
```