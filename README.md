<h1>MARKDOWN: First Push Project </h1>
<h2> By Mr.Sirawich Vounchuy </h2>

----------

> **$ git init** คำสั่ง git init เอาไว้เพื่อสร้าง git repository เปล่าๆขึ้นมา โดย Git จะทำการสร้างโฟลเดอร์  .git ขึ้นมาภายในโปรเจ็คของเรา (Hidden ไว้อยู่)

> **$ git add .** track ทุกไฟล์ที่อยู่ในโฟลเดอร์ 

> **$ git commit -m "Hello it's my first project commit"** คือการสร้าง snapshot ให้กับ repository ทำให้เราสามารถย้อนกลับมาดูว่าเราเปลี่ยนหรือแก้ไขโค๊ดอะไรไปบ้างได้
> **$ git remote add origin git@github.com:SirawichDev/markdown_readme.git** เพิ่ม url ของ remote (Server) เพื่อให้รู้ว่าเราจะฝากโค๊ดไว้ที่ใด

> **$ git push -u origin master** ต่อมาเราจะทำการส่งโค๊ดจากเครื่อง local ไปที่ Github ด้วยคำสั่ง
 
> **Tip:**  ถ้าต้องการ track ไฟล์หรือโฟลเดอร์ทั้งหมดที่อยู่ในโฟลเดอร์โปรเจคเดียวสามารถใช้  `$ git add .` แทนที่ จะ add ไปทีละตัว .

<h2> Reference </h2>

* [DEVAHOY](https://devahoy.com/posts/introduction-to-git-and-github/)


