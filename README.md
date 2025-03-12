# 2048 Game Deployment 🚀

This project deploys the "2048 game" using "Docker" and "AWS EC2".

# 🌟 Features
- Dockerized 2048 Game  
- Deployed on AWS EC2 using Docker  
- Accessible via Public IP  

# 🛠️ Technologies Used
- Docker (Containerization)  
- AWS EC2 (Cloud Deployment)  
- Nginx (Web Server)  
- Git & GitHub (Version Control)  

# 🚀 How I Deployed It

1. Created a Docker Image for 2048:
   
   docker build -t 2048_game .

2-Pushed the Image to Docker Hub:

  docker tag 2048_game charlotte020901/2048_game
  docker push charlotte020901/2048_game
3-Launched an AWS EC2 Instance (Ubuntu 22.04 Free Tier).

4- Installed Docker on EC2:

  sudo apt update
  sudo apt install -y docker.io
5-Pulled & Run the Docker Container on EC2:
  docker pull charlotte020901/2048_game
  docker run -d -p 80:80 charlotte020901/2048_game
6- Allowed HTTP Traffic in AWS Security Group to access the game online.

7-HURRAY!!Game is Live on EC2 Public IP! 🎉

🎮 Play the Game!
🔗 Open in Browser:
http://your-ec2-public-ip
(Replace with your actual EC2 Public IP.)

📌 Future Improvements
✅ Add SSL with Let's Encrypt
✅ Deploy on AWS ECS for Scalability
✅ Use a Custom Domain Name

📜 License
This project is open-source and free to use!

🚀 Happy Coding! 😊
