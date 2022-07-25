# (OOP School) library for learn oop by Tun Kedsaro

Python OOP+วิธีสร้าง library เป็นของตัวเอง + Upload package ไปยัง PyPI.org
PyPI: https://pypi.org/project/unclechat/

This program use for learn how to upload PyPi credit uncle engineer.

ปล. เวอร์ชั่นนี้ยังไม่สมบูรณ์ (เขียนแบบรีบๆ 55) ลุงเขียนขึ้นมาเพื่อประยุกต์นำ Python + Socket Library สร้างเป็นโปรแกรมแชทตัวอย่าง สำหรับนักพัฒนาสามารถนำ Source Code ไปพัฒนาต่อได้เต็มที่

### วิธีติดตั้ง

เปิด CMD / Terminal

```python
pip install oopzchool
```

### วิธีใช้

### วิธีการใช้งาน
- เปิด IDLE ขึ้นมาแล้วพิมพ์...

```python
from oopzchool.school import Student,Tesla,SpecialStudent,Teacher
#Day 0
print("----day 0----")
allstudent=[]
teacher1 = Teacher('Ada lovelace')
teacher2 = Teacher('Bill Gates')
print(teacher1.students)

#Day 1
print("----day 1----")
st1 = Student('Albert','Einstein')
allstudent.append(st1)
teacher2.AddStudent(st1)
print(st1.fullname)

#Day 2
print("----day 2----")
st2 = Student('Steve','Jobs')
allstudent.append(st2)
teacher2.AddStudent(st2)
print(st2.fullname)

#Day 3
print("----day 3----")
for i in range(3):
    st1.Coding()
st2.Coding()
st1.ShowEXP()
st2.ShowEXP()

#Day 4
print("----day 4----")

stp1 = SpecialStudent('Thomas','Edison','Hitler')
allstudent.append(stp1)
teacher1.AddStudent(stp1)
print(stp1.fullname)
print("Teasher give me 20 point")
stp1.exp = 20
stp1.Coding()
stp1.ShowEXP()

#Day 5
print("----day 5----")
print("Hey student How do you go to your home?")
print(allstudent)
for st in allstudent:
    print("I : {} back home with {}".format(st.name,st.vehicle))
    #check ว่า object นี้เป็น class อะไร
    if isinstance(st,SpecialStudent):
        st.vehicle.SelfDriving(st)

#Day 6
print("----day 6----")
teacher1.CheckStudent()
teacher2.CheckStudent()
print('Sum exp',st1+st2)

หากต้องการสร้างห้องใหม่
- กด New Room
- โปรแกรมจะสร้างห้องให้อัตโนมัติ (จำเลขห้องไว้ส่งให้เพื่อน)
- กด Enter Chatroom เพื่อเริ่มแชท

[STEP 3]
- ใช้งานได้เลยจ้าาา หากมีการกดปิดโปรแกรมระบบจะแจ้งให้สมาชิกท่านอื่นทราบว่าผู้ใช้ได้ออกจากกลุ่มแล้ว

พัฒนาโดย: ลุงวิศวกร สอนคำนวณ
FB: https://www.facebook.com/UncleEngineer
YouTube: https://www.youtube.com/UncleEngineer
