# Signal Mini Project
หัวข้อที่เลือก : ตัวเลือกที่1 ( Oscilloscope ที่สามารถใส่สัญญาณ input เองได้ )


วัตถุประสงค์ :


    • ใช้ App designer ของ MATLAB ให้เป็นประโยชน์


    • นำความรู้เรื่อง Fourier series มาประยุกต์ใช้


    • นำความรู้เบื้องต้นมาทำ Application ที่เป็นประโยชน์ต่อการเรียนรู้


    • ฝึกการทำงานแบบเป็นทีม


สิ่งที่ได้ดำเนินการแล้ว:


  1. Application มีช่องสำหรับปรับแต่งค่า Amplitudes, Frequency และ DC Offset
![image](https://user-images.githubusercontent.com/88447071/142366910-637d506d-1e35-42f1-bd5f-c48a0142551d.png)


  2. Application สามารถเลือกชนิดของสัญญาณมีคาบได้ ได้แก่ square, triangular, sine, และsawtooth wave
![image](https://user-images.githubusercontent.com/88447071/142366939-b6612474-4b76-4fba-87d8-a207614ba17a.png)


  3. Application สามารถเพิ่ม-ลดขอบเขตของเวลา และสามรถเปลี่ยนหน่วยของขอบเขตเวลา(time div) โดยการหมุน
![image](https://user-images.githubusercontent.com/88447071/142366959-d3603cee-6408-4205-8d13-c3c38d4d9f1a.png)



  4. Application มีปุ่มแบบ toggle ที่สามารถเปิด-ปิดการใช้งานได้ และ มีปุ่ม Default เพื่อรีเซ็ตค่าทุกอย่างกับไปเป็นค่าเริ่มต้น
![image](https://user-images.githubusercontent.com/88447071/142367050-4f6bc2f6-2e0f-4f4d-8511-2c6773b1acd4.png)


  5. ที่มาของสมการแต่ละชนิดรูปคลื่นสัญญาณ

    Sine wave 
    สามารถนำแอมพลิจูดไปคูณกับ sin(omega*t) ได้เลยและการ + offset หลังสมการเพื่อให้ยกระดับแรงดันของรูปคลื่นสัญญาณได้

    Square wave
   ![image](https://user-images.githubusercontent.com/88447071/142365425-998b1def-47f0-4e46-89da-e14b482ff1a1.png)
   ![image](https://user-images.githubusercontent.com/88447071/142365642-1ea7b989-04ae-4c51-b909-e754b10bb382.png)
   ![image](https://user-images.githubusercontent.com/88447071/142365664-2ebaa5a5-cc67-408a-9cd7-e21d9075a7b0.png)
   ![image](https://user-images.githubusercontent.com/88447071/142365675-f20878ee-632e-4e09-bef9-cde89cc3043b.png)
    
    Sawtooth
   ![Binder1_Page_08](https://user-images.githubusercontent.com/88447071/142366327-d89d7961-9f9a-4861-9494-e0f9b9ba01a6.jpg)
   ![Binder1_Page_09](https://user-images.githubusercontent.com/88447071/142366400-a0befced-951a-4b6d-8b8c-249cc46ead4c.jpg)

    Triangular
   ![Binder1_Page_10](https://user-images.githubusercontent.com/88447071/142366459-58f74190-53ef-43c1-a9ce-c15f2168b02f.jpg)
   ![Binder1_Page_11](https://user-images.githubusercontent.com/88447071/142366469-ed5f74c3-5de0-4e5e-9dc7-30a7c1c798e7.jpg)

  6. หลักการทำงานโดยทำการ plot รูปคลื่นสัญญาณจากสมการที่หามาได้โดยทำการวนลูปที่ k เริ่มต้นที่ 1 แล้วเพิ่มไปเรื่อย ๆ โดยจะแบ่งได้เป็นสองกรณี กรณีที่ฟังก์ชันเป็นฟังก์ชันคี่จะเพิ่มทีละ 2 กรณีที่เป็นฟังก์ชันปกติจะเพิ่มทีละ 1 โดยจำนวนการวนลูปกำหนดสูงสุดที่ k เป็น 50000 โดยหากกำหนดค่า k มากกว่านี้จะทำให้โปรแกรมช้า

  7. Application มีกราฟที่สามารถแสดงผลได้แบบ Realtime
![image](https://user-images.githubusercontent.com/88447071/142367187-f28353a2-40d9-4b72-afb1-b759847f478a.png)
