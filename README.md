"# Devops-TP2-Vagrant_NGINX" 
1.	Installation de NGINX
a.	Se connecter avec vagrant ssh
b.	Taper la commande sudo apt update
c.	Taper : sudo apt install -y nginx
d.	Taper sudo service nginx start
e.	Taper : sudo service nginx status
![a04](https://github.com/user-attachments/assets/b24f5388-b9db-49fa-b902-29a964693090)
![a05](https://github.com/user-attachments/assets/f73fc795-b69b-4930-972d-3fe252db4bb4)
 
1.	Déploiement d’une Application Front
a.	Taper sudo mkdir -p /var/www/html/mini-app
b.	Taper sudo nano /var/www/html/mini-app
![a06](https://github.com/user-attachments/assets/44972223-0cfa-4a08-a8ee-7688210975fb)
c.	Taper sudo ln -s /etc/nginx/sites-available/mini-app /etc/nginx/sites-enabled/
d.	Taper sudo nginx –t pour verifier que c’est correct
![a07](https://github.com/user-attachments/assets/cf6fa1cc-8390-4b1f-b627-1c81a68cd913)
e.	Taper sudo nano /var/www/html/mini-app/index.html
![a08](https://github.com/user-attachments/assets/82c6e22a-ff47-4bfe-865e-8d90f6f255d0)
f.	Taper sudo systemctl restart nginx
![a09](https://github.com/user-attachments/assets/3dbf8000-ac63-48fb-bb77-0ba4dab5dada)
3.	Installation et Configuration de MYSQL
a.	Ajout du port forwarding
![a10](https://github.com/user-attachments/assets/5bf30753-c5d0-4c61-b9a8-a98fb810e8c1)
h.	Taper vagrant halt
i.	Taper vagrant up
j.	Taper sudo apt update
k.	Taper sudo apt install mysql-server –y
l.	Taper sudo systemctl start mysql et sudo systemctl enable mysql pour activer MYSQL
![a11](https://github.com/user-attachments/assets/14b959ad-9ab0-41d0-aabe-3d2b188eb655)

m.	Redemarrer MYSQL, sudo systemctl restart mysql
n.	Connexion à MYSQL
![a12](https://github.com/user-attachments/assets/8bf2e2cf-18c1-4857-8efe-1f4820a981f7)








