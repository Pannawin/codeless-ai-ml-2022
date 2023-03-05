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

![Screenshot 2023-03-05 095841](https://user-images.githubusercontent.com/96861429/222939297-648315bc-0e9c-4459-a5f7-7022acb799be.png)



หาคาเฉลี่ยเเต่ละวิชา 

คณิตศาสตร์ 66.5

วิชาการอ่าน 70

วิชาการเขียน 68.5


![Screenshot 2023-03-04 132659](https://user-images.githubusercontent.com/96861429/222879846-406bbb5f-db56-4991-a7d3-a74b729d2625.png)



ใช้ node math formula ทำการรวมคะเเนนทั้ง 3 วิชา เพื่อให้ได้ค่าคะเเนนรวม






![Screenshot 2023-03-04 132824](https://user-images.githubusercontent.com/96861429/222879913-28f75fdd-431a-4d98-bad1-5ff3027df028.png)

เปลี่ยนชุดข้อมูลตัวอักษรให้เป็นตัวเลข (เพศ เชื้อชาติ การเข้าคอร์สเตรียมสอบ การศึกษาของผู้ปกครอง)



# การคาดเดา ผลคะเเนน วิชา Writing โดยใช้โมเดลต่างๆ  : 

ใช้ column filter ในการเอาคะเเนนวิชาอื่นออกก่อน







![Screenshot 2023-03-04 133352](https://user-images.githubusercontent.com/96861429/222880205-819d4c47-dd2d-4289-a03c-83e9f088091c.png)




![Untitled3](https://user-images.githubusercontent.com/96861429/222880421-257ddbda-4a85-44f8-b12b-4725cee924ba.png)



ผลลัพท์ การคาดคะเเนนต่างๆของเเต่ละโมเดล (คะเเนนวิชา writing)

Simple regresstion tree = 0.9444


Gradient boosted tree = 0.97 (เเม่นยำที่สุด)


Random Forest (regression)=0.942



# การคาดเดา ผลคะเเนนรวม : 





![Screenshot 2023-03-04 133130](https://user-images.githubusercontent.com/96861429/222880657-a21a8c4e-d902-40d6-877d-6702fe30a5c3.png)



![Untitled5](https://user-images.githubusercontent.com/96861429/222880760-4498f7dc-5b01-4e72-90ba-e0e8c3330d15.png)


ผลลัพท์ การคาดคะเเนนรวม

Simple regresstion tree = 1  (เเม่นยำที่สุด)

Gradient boosted tree = 0.997

Random Forest (regression)=  0.993



# สรุป : 
ตัวเเปรสำคัญ ที่มีผลคือ 

การเข้าคอร์สเตรียมสอบ เพศ

เพศชายจะทำคะะเนนสอบ วิชาคณิตศาสตร์ เกิณเกณฑ์ 85 คะเเนน มีจำนวนมากกว่าเพศหญิง
![Screenshot 2023-03-02 095736](https://user-images.githubusercontent.com/96861429/222880953-d7e67a18-22fa-4f21-929a-f2f468bf5ef6.png)


เเต่กลับกันผู้หญิงจะทำคะเเนน วิชา Reading กับ Writing ได้คะเเนนเกินเกณฑ์ 85 คะเเนน มากกว่าผู้ชาย







![Screenshot 2023-03-02 095859](https://user-images.githubusercontent.com/96861429/222939195-360f4386-6fa0-428a-a264-ea783911de08.png)
วิชา writing


![Screenshot 2023-03-02 095931](https://user-images.githubusercontent.com/96861429/222939197-e07ee110-53fb-4b8d-9226-0bdbb7714d89.png)
วิชา reading
