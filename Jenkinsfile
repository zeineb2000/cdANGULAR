pipeline
{
   agent any
    stages {
     stage('Pull') {
      steps{
       script{
     checkout([$class: 'GitSCM', branches: [[name: '*/main']],
         userRemoteConfigs: [[
        
         url:'https://github.com/zeineb2000/cdANGULAR.git']]])
         
         }
         }
         }
       stage('Build')
  {
             steps {
               script{
       sh "ansible-playbook ansible/build.yml -i ansible/inventory/host.yml"
                        }}}
 

         }
         }
         
