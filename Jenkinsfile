node('master'){

stage('Code Checkout')

                cleanWs()

                status.check([

                branch: 'master',

                repo: 'https://github.com/spring-projects/spring-petclinic.git'

                ])
  
  stage('Code build')

                

                build.check([

              
              command1 : 'clean install',
       

                

                ])

}

 



