pipeline { 
 agent any 
 stages { 
 
 stage('Recupération du projet') { 
 steps { 
 git 'https://github.com/Amiine12/myapp-ansible.git' 
 } 
 } 
 
 stage('Lancer Ansible') { 
 steps { 
 ansiblePlaybook credentialsId: 'vagrant-private-key', disableHostKeyChecking: 
true, installation: 'ansible2', inventory: '/home/vagrant/local_inventory', playbook: 'apache.yml' 
 } 
 } 
 
 } 
}
