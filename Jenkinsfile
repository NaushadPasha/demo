pipeline {
           agent  any
               tools {
  terraform 'Terraform-v1'
  }
  stages{
      
       /*   stage('git checkout'){
        steps{
               git 'https://github.com/NaushadPasha/demo.git'
             }
        }*/
     stage('Terraform Init'){
        steps{
           sh '''cd /home/ubuntu/adastra-test1
terraform init'''
             }
        }

stage('Terraform apply'){
        steps{
           sh '''cd /home/ubuntu/adastra-test1
terraform apply  --auto-approve -lock=false''' 
             }
        }

 } 

}  
