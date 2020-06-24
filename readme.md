## CodeCamp#6 Online

## Sompop Laya
<hr>

## Javascript Basic Part 1

### แบบฝึกหัด : การตั้งชื่อตัวแปรที่ดี

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

+ 1.ให้ระบุค่าของ a,b,c และ d หลังจบ statement ทั้งหมด

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
+ 2.จงหาผลลัพธ์ของ statement ดังต่อไปนี้

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

+ 1.จงหาค่าเปรียบเทียบต่อไปนี้

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
<hr>

### Homework

+ 1.จงคำนวนค่าด้านล่างต่อไปนี้ และ คอมเม้นตอบหลังคำถาม

```javascript
    5 + "34"                                            // 534
    5 ** 4                                              // 625
    5 - "4"                                             // 1
    10 % 5                                              // 0
    5 % 10                                              // 5
    (2 ** 5) % 2                                        // 0
    "Java" + "Script"                                   // JavaScript
    " " + " "                                           // " "
    " " + 0                                             // 0
    20 + 4 + "15"                                       // 2415
    true + true                                         // 2
    true + false                                        // 1
    false + true                                        // 1
    false - true                                        // -1
    false - true + false - true + false                 // -2
    (true + true) ** 4                                  // 16
    19 + true + "20"                                    // 2020
    3 - 4                                               // -1
    "Bob" - "bill"                                      // NaN
    "Code" + "Camp" + true + false + null + undefined   // CodeCamptruefalsenullundefined
```

+ 2.จงคำนวนค่าเปรียบเทียบต่อไปนี้ และคอมเม้นตอบด้านล่าง

```javascript
    5 >= 1                  //  true
    0 === 1                 //  false
    4 <= 1                  //  false
    1 != 1                  //  false
    1 == "1"                //  true
    1 === "1"               //  false
    "2" == "2"              //  true
    "2" === "2"             //  true
    "12" !== 12             //  true
    "15" != 15              //  false
    "A" > "B"               //  false
    "B" < "C"               //  true
    "a" > "A"               //  true
    "b" < "A"               //  false
    "bee" > "bbe"           //  true
    "BeE" < "Bee"           //  true
    "Sonter" > "Soncom"     //  true
    "circle" > "circles"    //  false
    "NaRuTo" < "nArUtO"     //  true
    true === false          //  false
    true != true            //  false
```

+ 3.สร้าง String ที่มีค่า "Hello, lt's me."Mario"."

```javascript
    let txt_string = `Hello, lt's me."Mario".`;
    console.log(txt_string);
```
<hr>

## Javascript Basic Part 2

### แบบฝึกหัด : ตัวดำเนินการแบบตรรกะ

+ 1.คำสั่งต่อไปนี้จะแสดงค่าเป็นอะไร

```javascript
    alert( null || 2 || undefined );        // 2
    alert( alert(1) || 2 || alert(3) );     // 1 และ 2
    alert( 1 && null && 2 );                // null
    alert( alert(1) && alert(2) );          // 1 และ undefined
    alert( null || 2 && 3 || 4 );           // 3
```
+ 2.เขียนคำสั่ง if ที่เช็คอายุว่าอยู่อยู่ระหว่าง 18 - 60

```javascript
    let myAge = 30;
    let beverAge = !!(myAge >=18 && myAge <=60);
    console.log(beverAge);
```

+ 3.เขียนคำสั่ง if ที่เช็คอายุว่าไม่อยุ่ระหว่าง 18 - 60

```javascript
    let myAge = 30;
    let beverAge = !!(myAge < 18 || myAge > 60);
    console.log(beverAge);
```

+ 4.คำสั่ง alert ไหนที่จะถูกรันบ้าง

```javascript
    if (-1 || 0) alert( 'first' );          // run alert ได้ค่า first
    if (-1 && 0) alert( 'second' );         // ไม่ run
    if (null || -1 && 0) alert( 'third' );  // ไม่ run
```

+ 5.ให้เขียนระบบ login
    + ให้ใช้ prompt ในการถามใครเป็นคน login
    + ถ้าผู้ใช้กรอกว่า "Admin" ให้ใช้ prompt ถาม password
        + วิธีเช็ค Password
        + ถ้า string นั้นเป็น "codecamp#6" ให้ alert "ยินดีตอนรับ
        + ถ้า string เป็นอย่างอื่นให้ alert เป็น "Wrong Password"
        + ถ้าเป็น string ว่าง หรือกด cancel ให้ alert ว่า "ยกเลิก"
    + ถ้าผู้ใช้กรอกอย่างอื่นที่ไม่ใช่ "Admmin" ให้ alert ว่า "ผมไม่รู้จักคุณ"
    + ถ้าผู้ใช้กรอก input เป็น string ว่าง หรือกด Esc ให้ alert ว่า "ยกเลิก"

```javascript
    let chkUser = prompt('ใครเป็นคน Login');

        if (!!(chkUser)) {
            if(chkUser === 'admin') {
                let chkPassword = prompt('กรุณากรอก Password');
                if(!!(chkPassword)) {
                    if(chkPassword == 'codecamp#6') {
                        alert("ยินดีตอนรับ");
                        exit();
                    }
                        alert("Wrong Password");
                        exit();
                }
                    alert("ยกเลิก")
                    exit();
            }
                alert("ผมไม่รู้จักคุณ");
                exit();
         }
            alert("ยกเลิก");
```
<hr>

### แบบฝึกหัด : วงวน for และ while     

+ 1.เลขที่ถูก alert เป็นลำดับสุดท้ายคือเลขอะไร ?

```javascript
    let i = 3;

    while (i) {
        alert( i-- );
    }

    // ตอบ. เลขลำดับสุดท้ายคือ 1
```

+ 2.code ทั้งสองอันนี้จะแสดง alert ออกมาเหมือนกันทั้งหมดหรือไม่

```javascript
    // Ex 1.
    let i = 0;
    while (++i < 5) alert( i );

    // Ex 2.
    let i = 0;
    while (i++ < 5) alert( i );  

    // ตอบ. ไม่เหมือนกัน Ex 1 จะแสดงข้อมูล [1,2,3,4]  Ex 2 จะแสดงข้อมูล [1,2,3,4,5]
```

+ 3.code ทั้งสองอันนี้จะแสดง alert ออกมาเหมือนกันทั้งหมดหรือไม่ 

```javascript
    // Ex 1
    for (let i = 0; i < 5; i++) alert( i );

    // Ex 2
    for (let i = 0; i < 5; ++i) alert( i );

    // ตอบ. เหมือนกัน Ex 1 และ Ex 2 จะแสดงข้อมูล [0,1,2,3,4] 
```

+ 4.ให้เขียน loop ทั้งแสดงเลข 2 ถึง 10 ออกมา

```javascript
    for (let i = 2; i <= 10; i++) alert( i );
```

+ 5.เปลี่ยน code for loop ด้านล่างนี้ให้เป็น while loop โดยที่ผลลัพธ์ยังเหมือนเดิม

```javascript
    // loop for
    for (let i = 0; i < 3; i++) {
        alert(`number ${i}`);
    }

    //loop while
    let i = 0;
    while(i++ < 3) alert(`number ${i}`);
```
+ 6.ให้เขียนเกมส์ทายตัวเลขสำหรับเล่นสองคน โดย
    + ให้ผู้เล่นคนแรกพิมพ์เลขใส่ใน prompt ที่อยู่ระหว่าง 1 ถึง 100 โดยไม่ให้ผู้เล่นคนที่สองรู้ว่าตัวเลขเป็นอะไร
    + และให้ผู้เล่นคนที่สองทายเลข โดยการพิมพ์เลยใส่ใน prompt จนกว่าจะถูก ถ้าไม่ถูก จะต้องบอกด้วยว่าเลขที่ผู้เล่นคนที่สองพิมพ์เข้ามา มากกว่า หรือ น้อยกว่า คำตอบนั้น

```javascript
    let player1 = prompt('[ผู้เล่นคนที่ 1] กรุณาเลือกตัวเลขระหว่าง 1 ถึง 100', '');
    let player2 = '';
         while (player1 !== player2) {

            let player2 = prompt('[ผู้เล่นคนที่ 2] กรุณาทายเลขของผู้เล่นคนที่ 1', '');

            if(Number(player1) < Number(player2)) {
                alert("ตัวเลขที่คุณทาย มากกว่า");

            }else if (Number(player1) > Number(player2)) {
                alert("ตัวเลขที่คุณทาย น้อยกว่า");

            }else {
                alert("ยินดีด้วย คุณทายตัวเลขถูกต้อง");
                break;
            }
                continue;
        }
```
<hr>

### แบบฝึกหักด : Swtich Cases

+ 1.แปลง Code ดังกล่าวเป็น if-else statement

```javascript
    // Switch case statement
    switch (bowser) {
        case 'Edge' :
            alert("You've got the Edge!");
            break;
        case 'Chrome':
        case 'Firefox':
        case 'Safari':
        case 'Opera':
            alert("Okay we support these browsers too");
            break;
        default:
            alert('We hope that this page looks ok!');      
    }

    // แปลงเป็น if - else statement
        if(bowser === 'Edge') {
            alert(("You've got the Edge!"); 
            exit();          
        } else if(bowser === 'Chrome') {

        } else if(bowser === 'Firefox') {

        } else if(bowser === 'Safari') {

        } else if(bowser === 'Opera') {
            alert('Okay we support these browsers too');
            exit(); 
        }
            alert('We hope that this page looks ok!');
```

+ 2.แปลง Code ดังกล่าวเป็น Switch cases

```javascript
    // if - else statement
    let a = +prompt('a?', '');

    if(a == 0) {
        alert( 0 );
    }
    if(a == 1) {
        alert( 1 );
    }
    if(a == 2 || a == 3) {
        alert( '2,3' );
    }

    // แปลงเป็น Switch Cases
    let a = +prompt('a?', '');

    switch (a) {
        case 0:
            alert( 0 );
            break;
        case 1:
            alert( 1 );
            break;
        case 2 || 3:
            alert( '2,3');
            break;
    }
```
<hr>

### แบบฝึกหัดพิเศษ : ฟังก์ชั่น

![image](https://i.ibb.co/5BKK9b5/1.jpg)

```javascript
        const method_Draw = (n) => String.prototype.padStart(n,'*');

        console.log(method_Draw(2));
        console.log(method_Draw(3));
        console.log(method_Draw(4));

```

![image](https://i.ibb.co/R0TPZSz/2.jpg)

```javascript
    function meThod_draw(n) {
        let result = '';
        for (let i = 0; i < n; i++) {
            for (let z = 0; x < n; z++) {
                result = result + '*';
            }
                result = result + '\n';
            }
        return result;
    }
    console.log(meThod_draw(2));
    console.log(meThod_draw(3));
    console.log(meThod_draw(4));
```

![image](https://i.ibb.co/6R5gdLR/3.jpg)

```javascript
   function meThod_draw(n) {
        let result = '';
        for (let i = 1; i <= n; i++) {
            for (let z = 1; z <= n; z++) {
                result = result + z;
            }
                result = result + '\n';
        }
            return result;
        }
    console.log(meThod_draw(2));
    console.log(meThod_draw(3));
    console.log(meThod_draw(4));
```

![image](https://i.ibb.co/x74CbLR/4.jpg)

```javascript
    function meThod_draw(n) {
        let result = '';
        for (let i = 1; i <= n; i++) {
            for (let z = 1; z <= n; z++) {
                result = result + i;
            }
                result = result + '\n';
        }
        return result;
        }
    console.log(meThod_draw(2));
    console.log(meThod_draw(3));
    console.log(meThod_draw(4));
```

![image](https://i.ibb.co/7KL319W/5.jpg)

```javascript
    function meThod_draw(n) {
        let result = '';
            for (let i = n; i >= 1; i--) {
            for (let z = 1; z <= n; z++) {
                    result = result + i;
                }
                    result = result + '\n';
            }
                return result;
    }
    console.log(meThod_draw(2));
    console.log(meThod_draw(3));
    console.log(meThod_draw(4));
```
