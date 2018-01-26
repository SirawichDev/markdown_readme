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

> **TIP 12:** ถ้าต้องการลบ branch นั้นออกใช้คำสั่ง `$ git branch -d [nameofbranch]` ต้องอย่าให้ branchปัจจุบันเป็น branch นั้นด้วย ถึงจะลบได้.

> **Tip 13** ถ้าต้องการ รวมไฟล์ที่อยุ่ใน branch dev มาใส่ใน branch master ย้ายไป masterก่อน แล้วใช้คำสั่ง
`$ git merge [nameofbranch] `

> **TIP 14:** ถ้าต้องการลบ branch ที่ remote  นั้นออกใช้คำสั่ง `$ git push origin --delete [nameofbranch]` 

> **TIP 15:** ลบuser ออกจากเครื่องนั้น กด start พิมพ์ credential manager -> เลือก window credential -> เลือก github.com -> remove

> **TIP 16:** ถ้าต้องการติด tag ให้ใช้คำสั่ง `$ git tag [nameoftag]` แล้วทำคสั่ง `$ git push --tags` 

> **TIP 17:** ถ้าต้องการย้อนกลับมา event ปัจจุบัน ใช้คำสั่ง `$ git checkout [namroftag]` มันจะอยู่กับ branch ปัจจุบัน 

> **TIP 18:** ถ้าต้องการลบ tags ใช้คำสั่ง `$ git tags -d ` แต่ที่ remote ยังไม่ถูกลบ ต้อง ใช้คำสั่ง `$ git push origin --delete [ชื่อของtag]`


 
<h2> Reference </h2>

* [DEVAHOY](https://devahoy.com/posts/introduction-to-git-and-github/)
* [guides.github](https://guides.github.com/features/mastering-markdown/)


* [Git Merge --on-ff อธิบาย 1](http://www.artit-k.com/how-to-git-config-merge-no-fast-forward/)
* [Git Merge --no-ff อธิบาย 2](https://sites.google.com/site/chanwit/blogs/git-explained-branch-and-merge)
* [สำหรับคนที่อยาก Push แบบไม่ต้องใส่รหัสซ้ำๆ (rsa key)](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)

* [อันนี้ Mediumของอาจาร์ย วโรดมเกี่ยวกับ git (เข้าใจง่ายมาก)](https://werapun.com/git-review-8ecb03b7c8cc)

<h2> HOMEWORK </h2>
Create 2 new branches (dev, feature)
dev: dev.md (lisyt command you have learn)

feature: feature.md (list features in your project)

merge master

`git merge --no-ff dev`

`git merge --no-ff feature`

<h2>Update HomeWorks</h2>

> **ทำไมถึงใช้?** : `git merge --no-ff [branchname]` ทำเมื่อ branch หลายๆ branch เวลา merge จะไปอยู่เส้นเดียวทำให้ดูยากมาก การแก้ปัญหาจึงนำ --no-ff มาใช้เพื่อทำให้ branch ที่สร้างขึ้นมาให้ แตกกิ่งก้านออกไป
> **ADDED** : ถ้าทำการ merge แบบไม่ --no-ff แล้วจะทำให้ branch นั้นหายไป
> **วิธีทำ(short)** : ทำการสร้าง branch ใหม่แล้วย้ายไป push เมื่อทำเสร็จแล้วให้ทำการกลับมายัง branch หลักแล้วทำการ merge แบบ no ff (no fast forward)แล้วเมื่อ แน่ใจจริงๆ ว่า branch นั้นเสร็จแล้วให้ทำการ push แล้วกลับมา merge ผลลัพธ์จะได้ network ของ branch ที่ดูง่ายสวยงาม **สามารถดูวิธีทำเพิ่มเติมได้ที่ Reference ที่อัพเดตให้**

<h2>ถ้ามี Error Conflict</h2>

> **วิธีแแก้** 

* `git add -A`
* `git commit -m "massage"`
* `git push --force`
* [ตามลิ้งค์นี้](https://githowto.com/resolving_conflicts)
 
 ### เพิ่มเติมแก้ปัญหา  conflict

* `$ git stash` : คือการเซฟและซ่อนโปรเจ็คของเราไว้ สามารถที่จะ restore กลับได้ทุกเมื่อ
* `$ git merge conflict` คือ เกิดกรณีที่มีการแก้ไขไฟล์เดียวกัน เวลาเดียวกัน Git จะไม่รู้ว่าเราควรจะใช้ไฟล์ไหนดี

### ISSUE(ประเด็น)
