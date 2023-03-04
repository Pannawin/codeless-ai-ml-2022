# codeless-ai-ml-2022


# Overview : 

Students Performance in Exams

About Dataset
This data set consists of the marks secured by the students in various subjects.

Example Research Questions:

How effective is the test preparation course?
Which major factors contribute to test outcomes?




![Screenshot 2023-03-02 093932](https://user-images.githubusercontent.com/96861429/222370068-3c1078e3-b38d-4ebe-ac45-8924ea2aa2d4.png)


ข้อมูลชุดนี้จะเเสดงให้เห็นถึง ผลคะเเนนของ การสอบทั้ง 3วิชา(Writing reading and Math) เเละข้อมุล ทั่วไป ปัจจัยอื่น เพศ การเข้าคอร์สเตรียมสอบ เชื้อชาติ การศึกษาของผู้ปกครอรอง



#ข้อมูลทั่วไปของ Data ชุดนี้ : 


   นักเรียนชายมีจำนวนทั้งหมด 517 นักเรียนหญิง 483 นักเรียนชาย นักเรียนมีจำนวนมากกว่านักเรียนหญิง 34 คน
![Screenshot 2023-03-02 152047](https://user-images.githubusercontent.com/96861429/222371680-f29c38f3-88e7-4132-8ed9-70f9432b25ae.png)



จำนวนผู้ไม่เข้าคอร์สเตรียมสอบ 665 คน  ส่วนคนที่เข้ามี 335 คน ต่างกัน 330 คน
![Screenshot 2023-03-02 100307](https://user-images.githubusercontent.com/96861429/222372078-230d2c7e-e55a-4f5e-91b0-8814a95c849e.png)





จำนวนเชื้อชาติต่างๆ
![Screenshot 2023-03-02 152751](https://user-images.githubusercontent.com/96861429/222373273-35de74ee-a2f4-4b27-9f34-4b575a0306cc.png)



# ภาพโปรเจคโดย ภาพรวม : 



![Screenshot 2023-03-02 153626](https://user-images.githubusercontent.com/96861429/222879549-36deeb86-c9d6-4456-878f-15878114bac8.png)





# การเตรียมข้อมูล : 





![Screenshot 2023-03-04 132659](https://user-images.githubusercontent.com/96861429/222879846-406bbb5f-db56-4991-a7d3-a74b729d2625.png)



ใช้ node math formula ทำการรวมคะเเนนทั้ง 3 วิชา เพื่อให้ได้ค่าคะเเนนรวม






![Screenshot 2023-03-04 132824](https://user-images.githubusercontent.com/96861429/222879913-28f75fdd-431a-4d98-bad1-5ff3027df028.png)

เปลี่ยนชุดข้อมูลตัวอักษรให้เป็นตัวเลข (เพศ เชื้อชาติ การเข้าคอร์สเตรียมสอบ การศึกษาของผู้ปกครอง)



# การคาดเดา ผลคะเเนน วิชา Writing โดยใช้โมเดลต่างๆ  : 

ใช้ column filter ในการเอาคะเเนนวิชาอื่นออกก่อน







![Screenshot 2023-03-04 133352](https://user-images.githubusercontent.com/96861429/222880205-819d4c47-dd2d-4289-a03c-83e9f088091c.png)




![Untitled3](https://user-images.githubusercontent.com/96861429/222880421-257ddbda-4a85-44f8-b12b-4725cee924ba.png)



ผลลัพท์ การคาดคะเเนนต่างๆของเเต่ละโมเดล (คะเเนนวิชา writing

Simple regresstion tree = 0.9444
Gradient boosted tree = 0.97
Random Forest (regression)=0.942




















