node('master'){

  def specsDir = "./Specs/V1.0"

if(fileExists(specsDir + "/ci-specs.yml")){
ci_specs = readYaml file : specsDir + "ci/-specs.yml"
specs -specs = ci_specs
}
  
stage('Code Checkout')

                cleanWs()

                status.check([

                branch: specs.SCM.branch,

                repo: specs.SCM.repo

                ])
  
  stage('Code build')

                

                build.check([

              
              command1 : specs.Build.command,
       

                

                ])

}

 



