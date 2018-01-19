<h1>MARKDOWN: First Push Project </h1>
<h2> By Mr.Sirawich Vounchuy </h2>

----------

> `$ git init` คำสั่ง git init เอาไว้เพื่อสร้าง git repository เปล่าๆขึ้นมา โดย Git จะทำการสร้างโฟลเดอร์  .git ขึ้นมาภายในโปรเจ็คของเรา (Hidden ไว้อยู่)

> `$ git add .` track ทุกไฟล์ที่อยู่ในโฟลเดอร์ 

> `$ git commit -m "Hello it's my first project commit"` คือการสร้าง snapshot ให้กับ repository ทำให้เราสามารถย้อนกลับมาดูว่าเราเปลี่ยนหรือแก้ไขโค๊ดอะไรไปบ้างได้

> `$ git remote add origin git@github.com:SirawichDev/markdown_readme.git` เพิ่ม url ของ remote (Server) เพื่อให้รู้ว่าเราจะฝากโค๊ดไว้ที่ใด

> `$ git push -u origin master` ต่อมาเราจะทำการส่งโค๊ดจากเครื่อง local ไปที่ Github ด้วยคำสั่ง
 
> **Tip 1:**  ถ้าต้องการ track ไฟล์หรือโฟลเดอร์ทั้งหมดที่อยู่ในโฟลเดอร์โปรเจคเดียวสามารถใช้  `$ git add .` แทนที่ จะ add ไปทีละตัว.

> **Tip 2:** เมื่อ ทำ `$ git push -u origin master` ไปครั้งแรกแล้วครั้งอื่นๆสามารถทำ `$ git push` อย่าได้เลยโดย ตัด ~~-u origin master~~ ออกโดยbranch ที่push เข้าไปจะเป็น branchล่าสุด

> **Tip 3:** เมื่อมีปัญหา ไฟล์ในdesktop กับ ในเซิฟเวอร์ไม่ตรงกัน ให้ใช้คำสั่ง  `$ git pull` โดย  `$ git pull` = `$ git fetch` + `$ git merge`

> **Tip 4:** เมื่ออยาก undo ไฟล์ ที่เราต้องการที่อยู่ในเซิฟเวอร์ `$ git checkout -- [Filename]`

> **Tip 5:** เมื่อ Addไปแล้วต้องการ ที่จะuntrack ให้ใช่คำสั่ง `$ git reset HEAD [Filename]`

> **Tip 6:** เช็คว่าเราทำอะไรไปบ้าง ให้ใช้ `$ git log` 

> **Tip 7:** ถอด commit ออก ใช้คำสั่ง `$ git reset --soft "HEAD^"`

> **TIP 8:** `$ git branch -a` ดูว่ามี branch อะไรบ้าง

> **TIP 9:** `$ git branch (nameofbranch)` สร้าง branch ขึ้นมาใหม่

> **TIP 10:** เปลี่ยน branch ใช้คำสั่ง `$ git checkout [nameofbranch]` 

> **TIP 11:** ถ้าต้องการ สร้าง branch พร้อม switch ไปที่ branch นั้นเลย ใช้คำสั่ง `$ git checkout -b [nameofbranch]`     

<h2> Reference </h2>

* [DEVAHOY](https://devahoy.com/posts/introduction-to-git-and-github/)
* [guides.github](https://guides.github.com/features/mastering-markdown/)

