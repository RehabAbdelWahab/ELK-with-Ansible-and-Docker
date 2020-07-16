# ELK-stack-with-Ansible-and-Docker


# How to run:


# Open "inventory\hosts.yml" file and change this data with your ip and credentials 


  ansible_host: <your_server_ip>
  
  
  ansible_ssh_user: <your_server_username>
  
  
  ansible_ssh_pass: <your_server_pass>




# Deploy the ELK stack


$ ansible-playbook -i inventory elk.yml


# Clean the ELK stack.


$ ansible-playbook -i inventory elk-clean.yml


# Here is the Ansible output:

![alt text](https://github.com/RehabAbdelWahab/ELK-with-Ansible-and-Docker/blob/master/111.PNG)


![alt text](https://github.com/RehabAbdelWahab/ELK-with-Ansible-and-Docker/blob/master/222.PNG)


# If you go to http://<your_server_ip>:9200 in your browser, you will see this:

Enter your username: elastic


Enter your Pass: H9H9YOuu75SwFYKSTIVJ


![alt text](https://github.com/RehabAbdelWahab/ELK-with-Ansible-and-Docker/blob/master/444.PNG)


# If you go to http://<your_server_ip>:8084 in your browser you will find the welcome page of Nginx:

![alt text](https://github.com/RehabAbdelWahab/ELK-with-Ansible-and-Docker/blob/master/333.PNG)
