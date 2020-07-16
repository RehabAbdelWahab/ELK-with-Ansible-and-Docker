# ELK-with-Ansible-and-Docker


# How to run:


# Open "inventory\hosts.yml" file and change this data with your ip and credentials 


  ansible_host: <your_server_ip>
  
  
  ansible_ssh_user: <your_server_username>
  
  
  ansible_ssh_pass: <your_server_pass>




# Deploy the ELK stack


$ ansible-playbook -i inventory elk.yml


# Clean the ELK stack


$ ansible-playbook -i inventory elk-clean.yml


# Here is the Ansible output:

![alt text](https://github.com/RehabAbdelWahab/ELK-with-Ansible-and-Docker/blob/master/imgs/1.PNG)


![alt text](https://github.com/RehabAbdelWahab/ELK-with-Ansible-and-Docker/blob/master/imgs/2.PNG)


# If you go to http://<your_server_ip>:9200 in your browser, you will see this:

Enter your username: elastic


Enter your Pass: "oOYUXhSg2DcImWEsPpR5"  


![alt text](https://github.com/RehabAbdelWahab/ELK-with-Ansible-and-Docker/blob/master/imgs/4.PNG)


# If you go to http://<your_server_ip>:5600 in your browser, you will see this:

Enter your username: elastic


Enter your Pass: oOYUXhSg2DcImWEsPpR5


![alt text](https://github.com/RehabAbdelWahab/ELK-with-Ansible-and-Docker/blob/master/imgs/5.PNG)


Then the Kibana will open, like this:


![alt text](https://github.com/RehabAbdelWahab/ELK-with-Ansible-and-Docker/blob/master/imgs/6.PNG)


# If you go to http://<your_server_ip>:8084 in your browser you will find the welcome page of Nginx:

![alt text](https://github.com/RehabAbdelWahab/ELK-with-Ansible-and-Docker/blob/master/imgs/3.PNG)
