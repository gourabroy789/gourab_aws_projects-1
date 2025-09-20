1. Launch an EC2 Instance:
**Go to AWS Console → EC2 → Instances → Launch Instance**
Choose AMI: Use Amazon Linux 2 or Ubuntu (common choice: Ubuntu Server 22.04 LTS)
Instance Type: t2.micro (eligible for free tier)
Key Pair: Create/download a key pair (e.g.Ohio key.pem).

2. Security Group (Firewall):
Allow SSH (port 22) from your IP
Allow HTTP (port 80) from anywhere

3. Connect to Your Instancec:
Conect EC2 Instance from aws portal 

4. Install a Web Server (e.g. Nginx)

sudo apt update
sudo apt install nginx -y

5. Start the Web Server
Nginx:
sudo systemctl start nginx
sudo systemctl enable nginx

Open a browser and go to address bar:

Search :  http://"your-ec2-public-ip"

Nginx Ubuntu Default Page or the Welcome to Nginx! page will reflect.

Deploy your own website:  Replace the default web root content in /var/www/html with your own html code and save. 
Search :  http://<your-ec2-public-ip>

you will able to see your own page. 
