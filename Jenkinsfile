pipeline 
{
    agent any
    {
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
               sh 'ansible-playbook  -h localhost --become true $WORKSPACE/ansible_nginx_playbook.yml'
            } 
            }

            
        }
    }
}