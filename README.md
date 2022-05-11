# Docker-Command-JK  

---

## Lean Docker-beginner
- [WEEK1-First-Time-Docker](https://github.com/JK369x/first-time-docker)

---

### เช็ค docker version
    docker -v
    
---    
    
### ดู Layer ของ Image ว่าเคยทำอะไรไปบ้าง
    docker history [ชื่อ image]
### ดูเนื้อที่ docker ใช้
    docker system df
### ดูว่า docker ที่ stop มีอะไรบ้าง
    docker ps -a 
### ดู Image ที่ถูกสร้าง
    docker images
    
---    
    
### docker rm [เลขcontainer ID]
    docker rm [container ID]
    ! container สามารถตั้งชื่อได้` 
   
### ลบ Image
    docker rmi [nameImage]
    ! ต้อง stop Image ก่อนถึงจะลบได้
 
---    
    
### รัน Docker image
    docker run hello-docker
    
---

### สร้าง Docker image
    docker build -t hello-docker

---

### คำสั่งหลักๆ ของ Dockerfile 12 คำสั่ง ได้แก่
- FROM กำหนด Base image
- LABEL ใช้กำหนด Metadata เช่น ชื่อ Version หรือเจ้าของ Image
- ENV กำหนด Environment variable ภายใน Container
- RUN ใช้สำหรับติดตั้ง Packagesให้ Container
- COPY สำหรับ Copy file และ Folder ไปยัง Container
- ADD สำหรับ Copy file และ Folder ไปยัง Container โดยสามารถแตกไฟล์ .tar รวมทั้ง Copy file จาก Host ภายนอกได้
- CMD สำหรับรันคำสั่งที่ต้องการขณะรัน Container
- WORKDIR กำหนด Working directory ของ Container
- ARG กำหนด Variable ขณะสร้าง Image
- ENTRYPOINT สำหรับรันคำสั่งที่ต้องการขณะรัน Container
- EXPOSE กำหนด Port ที่เปิดให้ Container อื่นติดต่อเข้ามา
- VOLUME สร้าง Folder เก็บข้อมูลแบบถาวรให้ Container

