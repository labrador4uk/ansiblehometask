# ansiblehometask

# To start the hometask pull project and start Vagrant enviroment from
git clone https://github.com/aliusmiles/training-ansible.git
# (Task will be deployed on node02 machine (ubuntu), so you can remove unnecessary things from vagrantfile)
# After enviroment is up just follow this small script to make everything work

vagrant ssh bastion

cd ansible

ansible -m ping all

git clone https://github.com/labrador4uk/ansiblehometask.git

cp ./ansiblehometask/* ./

ansible-playbook ashtest2.yml

# Give a playbook some time to setup everything, and when it is done you are free to check "Hello world" in your web browser on "http://192.168.13.114:8080" or using curl 192.168.13.114:8080

# Thank You for attention.
