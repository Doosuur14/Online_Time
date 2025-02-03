Код был загружен в мастер(master), а не в main ветку.

Steps to Run the Code
1. Clone the repository: git clone https://github.com/Doosuur14/Online_Time.git
2. Build the Docker image (optional)
If you're running it in a Docker container, you can follow these steps to build your image. Make sure you are inside the project directory
3.Run the Docker container (if using Docker)
Start the container:
docker run -it my-ubuntu-container /bin/bash
4.Make the timeserver and timeclient scripts executable (chmod +x timeserver timeclient)



Для проверки буде запущена программа timeserver в фоновом режиме с указанием порта для прослушивания:

./timeserver 8182 &
Для проверки буде запущена программа timeclient в фоновом режиме с IP адреса и порта для подключения:

./timeclient 127.0.0.1 8182
