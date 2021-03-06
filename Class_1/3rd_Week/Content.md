#คาบที่ 3 เริ่มเขียน Javascript กัน


##เนื้อหา

1. แนะนำเครื่องมือที่ใช้
2. เขียนโปรแกรมภาษา Javascript  
  - คำสั่ง / Statement
  - ชนิดข้อมูล / Data Type
  - การดำเนินการทางคณิตศาสตร์ / Operator
  - ตัวแปร / Variable
  
##เครื่องมือที่เราจะใช้

ในการเรียนวิชานี้เโปรแกรมหลักๆ อยู่ 3 ตัวด้่วยกัน

1. โปรแกรมสำหรับเปิดเว็บไซต์ / Web Browser โดยเราจะใช้ [Google Chrome](https://www.google.com/chrome/) กัน

2. เครื่องมือพัฒนาโปรแกรมของ Google Chrome / [Chrome Developer Tools](https://developer.chrome.com/devtools)

  - [เรียนรู้การใช้งาน Chrome Developer Tools](http://pstudiodev.blogspot.my/2012/09/chrome-developer-tools.html)
  - [รู้จักกับ Inspector เครื่องมือช่วยคนทำเว็บ](http://jirayu.in.th/2013/07/%E0%B8%A3%E0%B8%B9%E0%B9%89%E0%B8%88%E0%B8%B1%E0%B8%81%E0%B8%81%E0%B8%B1%E0%B8%9A-inspector-%E0%B9%80%E0%B8%84%E0%B8%A3%E0%B8%B7%E0%B9%88%E0%B8%AD%E0%B8%87%E0%B8%A1%E0%B8%B7%E0%B8%AD%E0%B8%8A%E0%B9%88/)
  
3. โปรแกรมสำหรับแก้ไขไฟล์ข้อความ / Code Editor ซึ่งเราจะใช้ [Sublime Text 2](http://www.sublimetext.com/2)
  - [Sublime Text2 มันเจ๋งยังไง](http://nicha.in.th/2012/11/sublime-text2-%E0%B8%A1%E0%B8%B1%E0%B8%99%E0%B9%80%E0%B8%88%E0%B9%8B%E0%B8%87%E0%B8%A2%E0%B8%B1%E0%B8%87%E0%B9%84%E0%B8%87/)

เขียนโปรแกรมภาษา Javascript
--------------------------
เริ่มต้นลองเขียนโปรแกรมกัน โดยในการเขียนโปรแกรมเราจะมาใช้ภาษาที่ชื่อว่า Javascript กัน อันดับแรกที่เราจะต้องทำคือเปิด Google Chrome ขึ้นมาแล้วกดปุ่ม F12 ที่อยู่ด้านบนของคีย์บอร์ด หรือถ้าไม่ได้ก็กด Ctrl+Shift+I
พอกดแล้วเราจะเจอหน้าต่าง หรือแถบหน้าตาดูน่ากลัวขึ้นมา ไม่ต้องตกใจไปให้กดไปที่แถบที่เขียนว่า Console เราจะเจอกับหน้าต่างที่ให้พิมพ์ข้อความลงไปได้ แล้วก็มีเครื่องหมาย
**>** อยู่

สิ่งแรกที่อยากให้ลองทำคือพิมพ์คำสั่งด้านล่างลงไป (ใช้คีย์บอร์ดภาษาอังกฤษตลอดน้า อย่าเปลี่ยนเป็นภาษาไทย เช่นปุ่ม ( ใช้ตรงตัว เลข 9 หรือ ต ไม่ใช่ที่ปุ่ม Z หรือ ผ น้า)

```javascript
console.log("Sawasdee krub");
```

เสร็จแล้วกด Enter
เราจะเห็นมันขึ้นมาว่า

```
   Sawasdee krub
<- undefined
```

จะเห็นว่าบรรทัดแรกมันแสดงข้อความที่เราใส่เข้าไปใน ```console.log("Sawasdee krub");```

*สำหรับบรรทัดที่สองเรายังไม่ต้องสนใจมันในตอนนี้

###แบบฝึกหัดที่ 1
ลองเปลี่ยนข้อความในเครื่องหมายคำพูดอื่นๆ เช่นชื่อเล่นของเราดู เช่น ```console.log("Boat");``` เกิดอะไรขึ้นบ้าง
คำถามคือ เราได้รับอะไรกลับมา

เราจะเห็นว่าตำสัง ```console.log();``` เป็นคำสั่งที่ให้เราสั่งในคอมพิวเตอร์แสดงผลอะไรก็ตามที่อยู่ในวงเล็บออกมาให้เราดู

###แบบฝึกหัดที่ 2
ลองพิมพ์คำสั่งต่อไปนี้ดู
```Javascript
console.log("A");
console.log("Hello World");
console.log(1);
console.log(3.14159);
console.log();
```
แล้วลองตอบว่าเราเกิดอะไรขึ้นบ้าง

## คำสั่ง / Statement
สิ่งที่เราลองพิมพ์ไปเมื่อสักครู่เราเรียกว่า "คำสั่ง" คือเราพิมพ์คำสั่งเพื่อสั่งให้คอมพิวเตอร์ทำงานตามที่เราต้องการ

```Javascript
console.log("Sawasdee krub");
```

ส่วนประกอบของคำสั่งที่เราพิมพ์ไปมีอยู่ 3 ส่วนหลักๆ คือ

1. ตัวคำสั่ง ```console.log()``` เป็นชื่อคำสั่งที่เราต้องการที่จะสั่งให้คอมพิวเตอร์ทำ ในกรณีนี้คือการสั่งให้คอมพิวเตอร์แสดงผลข้อความออกมาทางหน้าจอภาพ
2. ข้อมูล ```"Sawasdee krub"``` เป็นข้อมูลที่เราส่งไปพร้อมกับคำสั่งเพื่อให้คอมพิวเตอร์รู้ว่าเราอยากให้ทำคำสั่งนั้นอย่างไร ในกรณีนี้คือบอกไปว่าต้องการที่จะให้แสดงข้อความนี้ออกมาทางจอภาพ
3. เครื่องหมาย ```;``` เป็นสัญลักษณ์ที่บ่งบอกจุดที่สิ้นสุดคำสั่งของเรา

เดี่ยวเราจะกลับมาดูคำสั่งอื่นๆ อีกครั้ง ตอนนี้เรามาดูเรื่องต่อไปกันก่อน

## ชนิดข้อมูล / Data Type
ในการเขียนโปรแกรม เราจะมีการแบ่งข้อมูลออกเป็นชนิดต่างๆ เพื่อให้ทั่งเราและคอมพิวเตอร์เข้าใจว่าเรากำลังใช้ข้อมูลอะไรอยู่มากขึ้น

###ตัวเลข / number
คือตัวเลขทั่งจำนวนเต็ม และจำนวนทศนิยม ทั่งจำนวนบวก จำนวนลบ และศูนย์
```Javascript
0
1
102
3.14159
-21
0.3448
```
นอกจากนี้เรายังวิธีการเขียนแทนจำนวนมากๆ เช่น 100,000,000,000,000,000 ด้วยสัญลักษณ์ทางคณิตศาสตร์คือ
10 ยกกำลัง 17 เป็น หรือจำนวนทศนิยมน้อยๆ เช่น 0.000000000000123 เป็น 1.23 x 10 ยกกำลัง -13
```Javascript
10e+17
1.28e-15
4.3212e+11
```

###ข้อความ / string
ข้อความคือตัวอักษร สัญลักษณฺ์ คำ หรือประโยต หรือแม้แต่ตัวเลขที่อยู่ภายในเครื่องหมายคำพูด 
เช่น
```Javascript
"A"
"Boat"
"Sawasdee krub"
"10"
"3.14159"
"*^*"
"--+--+--+--"
```

###ค่าความจริง / boolean
คือค่าที่ใช้แทนค่าความจริงคือ จริง หรือ เท็จ ซึ่งเราจะได้เห็นประโยชน์ของค่าความจริงในเรื่อง คำสั่งเงื่อนไข ในคาบต่อๆ ไป
โดย true คือค่าแทน จริง และ false แทนค่า เท็จ
```Javascript
true
false
```

###ไม่ใช่ตัวเลข / NaN
เราจะเจอ NaN (Not a number) เมื่อเราใช้การดำเนินการทางคณิตศาสตร์ บวก ลบ คูณ หาร แบบที่ไม่ปกติ
เช่นการเอาจำนวนใดๆ มาหารด้วย 0 เป็นต้น ซึ่งเราไม่สามารถหารอะไรด้วย 0 ได้ คอมพิวเตอร์จึงใช้ NaN เป็นเพื่อเป็นผลลัพธ์แทน

###ไม่นิยาม / Undefined
เมื่อเราประกาศตัวแปร (ดูในหัวข้อ ตัวแปร / variable) โดยที่ยังไม่ให้ค่าลงไป ตัวแปรเหล่านั้นจะมีค่าเริ่มต้นเป็น undefined คือเรายังไม่นิยามความหมายของตัวแปร

###ไม่มีค่า / null
เราจะได้เจอ null ในภายหลังซึ่งจะอธิบายอีกครั้งหนุึ่ง

##การดำเนินการทางคณิตศาสตร์ / Operator

เราสามารถใช้การดำเนินการทางคณิตศาสตร์ได้ เช่น การบวก การลบ การคูณ และการหาร เป็นต้น
ในการเขียนโปรแกรมเราจะแทนเครื่องหมายทางคณิตศาสตร์ต่างๆ ดังนี้

1. ```+``` แทนการบวก

2. ```-``` แทนการลบ

3. ```*``` แทนการคูณ

4. ```/``` แทนการหาร

###แบบฝึกหัดที่ 3
ลองเปิด Chrome Developer Tools ใน Google Chrome ขึ้นมาแล้วลองพิมพ์ประโยคสัญลักษ์ทางคณิตศาสตร์ด้านล่างลงไป
แล้วสังเกตดูผลลัพธ์ที่เกิดขึ้น

```Javascript
1+1
101+158
2*3
11*58
6/3
1/3
1000000000000*10000000000000
78-99
0.5/0.25
```

เราจะเห็นว่าเราสามารถให้คอมพิวเตอร์คำนวนค่าต่างๆ ให้เรากับเราได้

###แบบฝึกหัดที่ 4
ลองใช้ตัวดำเนินการทางคณิตศาสตร์ด้่านล่างแล้วสังเกตผลลัพธ์ที่เกิดขึ้น เครื่องหมายนี้เอาไว้ใช้ทำอะไร

```Javascript
6%3
7%3
11%5
99%33
5%3
```
ลองทดลองเปลี่ยนตัวเลข แล้วตอบดูว่าเครื่องหมายนี้เอาไว้ทำอะไร

##การเปรียบเทียบข้อมูล / Comparation

เราสามารถเปรียบเทียบข้อมูลได้ในลักษณะเดียวกับในคณิตศาสตร์ ทั้งเปรียบเทียบความเท่ากัน น้อยกว่า มากกว่า เป็นต้น
โดย
1. ```===``` แทน เท่ากับ หรือมีค่าเท่ากัน
2. ```!==``` แทน ไม่เท่ากับ
3. ```<``` แทน น้อยกว่า
4. ```>``` แทน มากกว่า
5. ```<=``` แทน น้อยกว่าหรือเท่ากับ
6. ```>=``` แทน มากกว่าหรือเท่ากับ

ค่าผลลัพธ์ของการเปรียบเทียบจะออกมาเป็นค่าความจริงคือ จริง หรือ เท็จ
เช่น
```Javascript
100 > 52
```
จะให้ค่าเป็น จริง
```Javascript
1 > 2
```
จะให้ค่าเป็น เท็จ เป็นต้น

###แบบฝึกหัดที่ 5
ลองทดลองใช้การเปรียบเทียบด้านล่างดู แล้วสังเกตดูผลลัพธ์ที่เกิดขึ้น
```Javascript
11 === 11
18 === 58
2 !== 2
38 !== 52
11 > 52
35 < 99
1.23 < 2.53
25 <= 25
98 >= 199
```

###แบบฝึกหัดที่ 6
เราลองทดลองคำสั่งด้านล่าง
```Javascript
1 === 1
1 === '1'
1 == 1
1 == '1'
```
ลองทดลองค่าต่างๆ แล้วหาความแตกต่างระหว่าง ```==``` กับ ```===``` ดู รวมถึงหาความแตกต่างระหว่าง ```!===``` กับ ```!=```

##ตัวแปร / Variable
ในการเขียนโปรแกรมเราจะสามารถสร้างตัวแปรได้ ซึ่งตัวแปรเป็นเหมือนการที่เรามีกล่องเพื่อเก็บข้อมูลอยู่แล้วเราตั้งชื่อให้กับมันเพื่อให้เราสามารถเรียนใช้ได้ง่ายขึ้น
การสร้างตัวแปรทำได้โดยใช้คำสั่ง
```Javascript
var x;
```
ซึ่งจะทำให้เรามีตัวแปรชื่อ ```x``` ขึ้นมาซึ่งเริ่มต้นมาถ้าเราถามหาค่าของ x ผ่านคำสั่ง ```console.log(x);``` เราจะได้ค่า undefined กลับมา
ซึ่งก็คือการที่เรายังไม่่ได้บอกคอมพิมเตอร์ว่าค่าของ ```x``` คืออะไรนั้นเอง การให้ค่ากับ ```x``` สามารถให้ได้โดยใช้เครื่องหมาย ```=```
```Javascript
x = 10;

console.log(x);
```
ค่าของตัวแปรสามารถเปลี่ยนแปลงได้ตลอดเวลาขึ้นกับว่าเราจะให้ความมันเป็นอะไร
```
x = 12;
console.log(x);

x = 20;
console.log(x);
```

##ข้อกำหนดของการตั้งชื่อตัวแปร
ชื่อของตัวแปรสามารถตั้งโดยประกอบด้วยตัวอักษรได้ 4 ประเภทคือ ตัวอักษรภาษาอังกฤษตัวพิมพ์ใหญ่ พิมพ์เล็ก ตัวเลข และเครื่องหมาย underscore _ (ขีดล่าง)
```Javascript
var a;
var hello;
var goodBoy;
var big_foot;
var strong_machine_1;
```
แต่เราไม่สามารถใช้ตัวเลขขึ้นหน้าได้
```Javascript
var 1toy; 	// error
```
เราสามารถใช้เครื่องหมายอื่นๆ บางเครื่องหมายและภาษาไทยได้ด้วย แต่เราไม่ควรใช้เพราะมีโอกาสเกิดปัญหาอื่นๆ ได้ ใช้แค่ 4 ประเภทนี้ปลอดภัยกว่า

##คำสั่งรับข้อมูลจากผู้ใช้
ลองพิมพ์คำสั่งด้านล่างดู
```Javascript
var data = prompt("Give me a number");
console.log(data);
```
เราจะเห็นว่าบน Google Chrome จะขึ้นหน้าให้พิมพ์ข้อความให้กับเรา และเมื่อเราพิมพ์ข้อความลงไป
มันก็จะถูกส่งไปเก็บที่ตัวแปรชื่อว่า data ต่อไป ด้วยเครื่องหมาย ```=```

##การเขียนโปรแกรมในไฟล์
ก่อนหน้านี้เราเขียนคำสั่งลงใน Chrome Developer Tools ซึ่งเราจะพิมพ์ที่ละคำสั่ง แล้วให้คอมพิวเตอร์ทำงานเมื่อเรากดปุ่ม Enter
ซึ่งใช้ในลักษณะนี้มีประโยชนตอนที่เราเรียนรู้คำสั่ง แต่เมื่อเราต้องเขียนออกมาเป็นโปรแกรมที่ทำงานหลายขั้นตอนต่อเนื่องกัน เราจะเอาไปเขียนไปใส่ในไฟล์เอกสารแทน

ให้เราเปิดโปรแกรม Sublime Text 2 ขึ้นมา แล้วลองคัดลอกข้อความข้างล่างลงไป (copy and paste)

###โปรแกรม 1: แสดงประโยคคำพูด
```html
<!DOCTYPE html>
<html>
	<body>
		<script type="text/javascript">
			// This program write Hello to the website
			document.write("Sawasdee Krub");
		</script>
	</body>
</html>
```

เสร็จแล้วก็ save as ไฟล์เป็นชื่อ hello.html จากนั้นเราเปิดไฟล์นี้ด้่วย Google Chrome เราจะเห็นข้อความ Sawasdee Krub อยู่บนหน้าเว็บไซต์
ซึ่งถ้าเรามาดูสิ่งที่เราเขียนลงไป ไฟล์ที่เราเขียนเรียกว่าไฟล์ HTML เป็นไฟล์เว็บไซต์แบบเดียวกับที่เราเห็นเวลาเปิดใช้งานเว็บไซต์ต่างๆ

ที่บรรทัดที่ 4 เราจะเห็น ```<script type="text/javascript">``` ส่วนนี้เป็นส่วนที่เราจะเขียน Javascript ลงไปในไฟล์ HTML 
ในวิชานี้เราจะใช้งานส่วนนี้เป็นหลัก

ที่บรรทัดที่ 5 เราจะเห็น ```// input your code here``` ส่วนนี้เรียกว่า comment หรือเป็นที่ๆ เราไว้ใช้เขียนคำอธิบายลงไป โดยไม่มีผลต่อการทำงานของโปรแกรม
เราใช้สำหรับไว้เขียนอธิบายเพื่อให้คนมาอ่านเอกสารของเราเข้าใจการทำงานของโปรแกรมได้ง่ายมากขึ้น ซึ่งการเขียน comment จะทำได้โดยเริ่มต้นด้วยเครื่องหมาย ```//``` แล้วในบรรทัดเดียวกัน
หลังจากเครื่องหมายนี้ จะเป็นส่วนที่เราพิมพ์คำอธิบายลงไป ```//``` จะมีผลเฉพาะบรรทัดนั้นๆ เท่านั้น

ที่บรรทัดที่ 6 เราจะเห็น ```document.write("Sawasdee Krub");``` คำสั่งนึ้เป็นคำสั่งในลักษณะคล้ายๆ กับ ```console.log();``` 
คือทำหน้าที่คล้ายๆ แสดงผลแต่ ```document.write()``` ทำหน้าที่เขียนข้อความของเราลงไปในเว็บไซต์แทน ในขณะที่ ```console.log();``` 
ใช้สำหรับแสดงผลข้อความในส่วน console ของ Chorme Developer Tools

ที่บรรทัดที่ 7 เราจะเห็น ```</script>``` ตรงนี้เป็นจุดที่กำหนดขอบเขตสิ้นสุดที่เราจะเขียน Javascript ลงไป ฉะนั้นเวลาเราเขียนโปรแกรมให้เขียนเฉพาะในขอบเขตนี้

###โปรแกรม 2: แสดงประโยคทักทายผู้ใช้
สร้างไฟล์เอกสารขึ้นมาใหม่ในโปรแกรมแล้วคัดลอกโปรแกรมด้านล่างลงไป
```html
<!DOCTYPE html>
<html>
	<body>
		<script type="text/javascript">
			// This program will say Hello to user
			var name = prompt("What is your name?");
			document.write("Hello " + name);
		</script>
	</body>
</html>
```
Save เป็นชื่ออะไรก็ได้ แล้วลงท้ายด้วย .html จากนั้นใช้ Google Chrome เปิดดู จะเห็นว่าจะมีกล่องให้ใส่ข้อความในลักษณะเดียวกับที่เราเคยใช้ใน ```propmt()``` ขึ้นมาให้เราพิมพ์ข้อความ
แล้วถ้าเราพิมพ์ข้อความลงไปแล้ว มันก็จะแสดง Hello ตามด้วยข้อความที่เราพิมพ์ลงไป ถ้ากลับไปดูโปรแกรมของเรา เราจะเห็นว่ามีคำสั่งอยู่ 2 บรรทัดด้วยกัน

บรรทัดแรก ```var name = prompt("What is your name?");``` จะเริ่มทำงานจาก ```prompt("What is your name?")``` เพื่อให้มีกล่องให้ใส่ข้อความขี้นมา
จากนั้นข้อความจะคืนกลับไปใส่ไว้ในตัวแปร ```name``` เนื่องจากเราใส่เครื่องหมาย ```=``` เอาไว้

บรรทัดที่ 2 ```document.write("Hello " + name);``` จะเป็นการเอาข้อความของเรามาเขียนลงไปบนหน้าเว็บไซต์

เราจะเห็นความีเครื่องหมาย + อยู่ระหว่าง ```"Hello " + name``` ซึ่งการใช้ + กับข้อความจะได้ผลลัทธ์เป็นการเอาข้อความมาต่อกัน

ลองพิมพ์คำสั่งข้างลงไปใน Chrome Developer Tools
```Javascript
"Hello" + "World"
"Sawasdee " + "krub"
"1" + " " + "Week"
"Blue " + "Rainy " + "Sky"
```
แล้วสั่งเกตดูผลลัพธ์ที่เกิดขึ้น

###โปรแกรม 3: รับค่าผู้ใช้ 2 ค่าเข้ามา แล้วหาผลบวก
โปรแกรมที่ 3 จะทำงานโดยการมีกล่องข้อความขึ้นมาให้ผู้ใช้ใส่ข้อความลงไป 2 ครั้ง แล้วเอาข้อความมาต่อกัน แล้วแสดงผลข้อความนั้น

```html
<!DOCTYPE html>
<html>
	<body>
		<script type="text/javascript">
			// This program will put two text together
			var text1 = prompt("Please input text 1");
			var text2 = prompt("Please input text 2");
			var text3 = text1 + text2;
			document.write(text3);
		</script>
	</body>
</html>
```

###โปรแกรม 4: รับค่าผู้ใช้เป็นตัวเลขเข้ามาแล้วแสดงผล
โปรแกรมที่ 3 จะทำงานโดยรับข้อความเข้ามา โดยคาดหวังให้ผู้ใช้พิมพ์ตัวเลขเข้ามา เมื่อเราได้มาแล้วใส่ไว้ในตัวแปร ```text``` แต่เเนื่องจาก
การรับเข้ามาแบบนี้จะได้ข้อมูลเป็นประเภทข้อความ ไม่ใช่ตัวเลข เช่นถ้าผู้ใช้พิมพ์ 3 เข้ามา เราจะได้ ```"3"``` ไม่ใช่ ```3``` ซึ่งไม่เหมือนกัน
เราจะเอามาทำการตำนวนเลขต่อไป เช่นการบวก ลบ คูณ หาร ไม่ได้ เราจึงจะใช้คำสั่งในบรรทัดที่ 2 ```parseInt(text)``` เพื่อแปลงข้อความที่เป็นตัวเลขอย่าง ```"3"``` 
ให้กลายเป็น ```3``` ก่อน แล้วเก็บไว้ในตัวแปรซื่อ ```num``` ต่อไป

```html
<!DOCTYPE html>
<html>
	<body>
		<script type="text/javascript">
			// This program will convert string (text) to number
			var text = prompt("Please input a number");
			var num = parseInt(text);
			document.write(num);
		</script>
	</body>
</html>
```

###โปรแกรม 5: แสดงผลการบวกเลข
จากที่เราเคยใช้คำนวนเลข บวก ลบ คูณ หาร ไปแล้ว เรามาลองใช้มันอีกครั้งนึง แล้วสังเกตผลลัพธ์ที่เกิดขึ้นดู

```html
<!DOCTYPE html>
<html>
	<body>
		<script type="text/javascript">
			// This program show you how to calculate basic math
			var result1 = 22+35;
			document.write(result1);
			var result2 = 22-35;
			document.write(result2);
			var result3 = 22*35;
			document.write(result3);
			var result4 = 22/35;
			document.write(result4);
			
			document.write(99+85);
			document.write(99-85);
			document.write(99*85);
			document.write(99/85);
		</script>
	</body>
</html>
```

###แบบฝึกหัดที่ 7 โปรแกรมคำนวณเลข 1
ในแบบฝึกหัดนี้จะให้เราลองเขียนโปรแกรมรับค่าตัวเลขมา 2 ตัว จากนั้นให้แสดงผลบวกของตัวเลขทั้งสองออกทางหน้าจอ

```html
<!DOCTYPE html>
<html>
	<body>
		<script type="text/javascript">
			// input your code here

		</script>
	</body>
</html>
```

###แบบฝึกหัดที่ 8 โปรแกรมตำนวณเลข 2
ในแบบฝึกหัดนี้จะให้เราลองเขียนโปรแกรมรับค่าตัวเลขมา 2 ตัว จากนั้นให้แสดงผลบวก ลบ คูณ หารของตัวเลขทั้งสองออกทางหน้าจอ

```html
<!DOCTYPE html>
<html>
	<body>
		<script type="text/javascript">
			// input your code here

		</script>
	</body>
</html>
```
