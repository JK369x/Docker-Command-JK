# Docker-Command-JK
script docker commend  
### เช็ค docker version
    docker -v
### ดู Layer ของ Image ว่าเคยทำอะไรไปบ้าง
    docker history [ชื่อ image]
### ดูเนื้อที่ docker ใช้
    docker system df
### docker rm [เลขcontainer ID]
    docker rm [container ID]
    ! container สามารถตั้งชื่อได้
### ลบ Image
    docker rmi [nameImage]
    ! ต้อง stop Image ก่อนถึงจะลบได้
### ดูว่า docker ที่ stop มีอะไรบ้าง
    docker ps -a 