pipeline 
{
    agent any
    
        stages
        {
            stage("SCM Checkout")
            {
                 steps {
             git url: 'https://github.com/sakshi151990/Nginx_Assignment.git'
            }
            }
            stage("Install Nginx")
            {
                steps { 
               
               sh 'ansible-playbook $WORKSPACE/ansible_nginx_playbook.yml -e "workspace=$WORKSPACE"'
            } 
            }

            
        }
    
}