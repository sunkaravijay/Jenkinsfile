node('master'){

stage('Code Checkout')

                cleanWs()

                status.check([

                branch: 'master',

                repo: 'https://github.com/Harshilbhardwaj47/App-src/tree/master/Springbot.git'

                ])
  
  stage('Code build')

                

                build.check([

              command1 : 'clean',
              command2 : 'compile',
              command3 : 'package'

                

                ])

}

 



