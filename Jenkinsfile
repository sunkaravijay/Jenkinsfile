node('master'){

stage('Code Checkout')

                cleanWs()

                status.check([

                branch: 'master',

                repo: 'https://github.com/Harshilbhardwaj47/App-src.git'

                ])
  
  stage('Code build')

                

                build.check([

              command : 'install',
              

                

                ])

}

 



