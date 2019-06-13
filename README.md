STRUCTURE (VIEWFLOW)
------------
+---API
|   |   server_api.docx
|   |   
|   \---simple-thai-classification-mpi-master
|       |   finalized_tfidftransformer10.pkl
|       |   model_prediction.py
|       |   
|       +---data
|       |       stopwords-th_new.txt
|       |       total_40992-final1.csv
|       |       
|       \---model
|               _finalized_model_svc_v2_70p.sav
|               
\---UI_cs402
    |   About.html
    |   css_finish.css
    |   Economic.html
    |   Education.html
    |   Government.html
    |   Health.html
    |   Index_train70.html
    |   Live.html
    |   
    \---pictures
            bg-401.jpg
            clear-401.jpg
            head-401.jpg
            run-401.jpg
            subhead-401.jpg
            

##Folder /src 
------------
#### 1.โฟลเดอร์ UI_cs402 (ติดตั้งในเครื่องคอมพิวเตอร์) 
นำโฟลเดอร์ชื่อ UI_cs402 ไปวางในเครื่องคอมพิวเตอร์ ซึ่งภายในโฟลเดอร์จะมีไฟล์ชื่อ Index_train70.html ซึ่งเป็นเว็บไซด์ในการจำแนกประเภทข้อความ ที่มีการเรียกใช้งาน API จากเครื่องของ server โดยสามารถดูคู่มือการใช้งาน (User manual) ที่อยู่ในโฟลเดอร์ /doc ได้
                
#### 2.โฟลเดอร์ API (ไม่ต้องติดตั้งในเครื่องคอมพิวเตอร์) 
มีไฟล์ word ชื่อ server_api.docx ด้านในไฟล์จะมีลิ้งเพื่อเข้าไปดู code ของฝั่ง server ที่ใช้ในกระบวนการสร้าง api ซึ่งในโฟลเดอร์ API จะมีโฟลเดอร์ชื่อ simple-thai-classification-mpi-master จะเป็น code ที่ติดตั้งในฝั่ง server เป็นตัวอย่างเพื่อใช้แสดงถึงโครงสร้างของงระบบ มีรายละเอียดอธิบายแต่ละไฟล์ดังนี้
+ ไฟล์ชื่อ model_prediction.py เป็น api ที่ทำกระบวนการจำแนกข้อความ
+ ไฟล์ชื่อ finalized_tfidftransformer10.pkl ไฟล์หา TF-IDF ของโมเดลที่ผ่านการเทรนเรียบร้อยแล้ว
+ โฟลเดอร์ data เก็บไฟล์ข้อมูลที่ใช้งาน 
  * ไฟล์ชื่อ total_40992-final1.csv เก็บข้อมูลที่ใช้สำหรับเทรนโมเดลจำนวน 40,992  ข้อความ
  * ไฟล์ชื่อ stopwords-th_new.txt ลิสของตัวหยุดคำภาษาไทย(Stop Word Removal)
+ โฟลเดอร์ model  เก็บไฟล์โมเดลที่ผ่านการเทรนแล้ว
  * ไฟล์ชื่อ _finalized_model_svc_v2_70p.sav ไฟล์โมเดลที่ผ่านการเทรนเรียบร้อยแล้ว
  
 ##### การติดตั้งโปรแกรมฝั่ง server
 
 1.ดาวโหลด Python เวอร์ชั่น 3.7 `<link>` :https://www.anaconda.com/distribution/
     
 2.Install this package with conda run: `conda install python=3.5.0`
     
 3.Install TensorFlow with pip : `python -m pip install --upgrade tensorflow`
     
 4.Install library Deepcut using pip : `pip install deepcut`
     
 5.Install Wordcloud using pip : `pip install wordcloud`
      
 6.Install scikit-learn is using pip : `pip install -U scikit-learn`

##Folder /doc
------------
- ไฟล์รายงานฉบับสมบูรณ์ ไฟล์ชื่อ 61wrj01-r02.pdf
- ไฟล์บทคัดย่อภาษาไทย ไฟล์ชื่อ 61wrj01-r02_abstract_th.txt
- ไฟล์บทคัดย่อภาษาอังกฤษ ไฟล์ชื่อ 61wrj01-r02_abstract_en.txt
- คู่มือการใช้งาน (User manual) ของระบบ ชื่อไฟล์ คู่มือการใช้งาน(User manual).docx



