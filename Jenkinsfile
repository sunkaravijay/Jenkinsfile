node('master'){
  def specs = [:]
  def specsDir = "./Specs/V1.0"

if(fileExists(specsDir + "/ci-spec.yml")){
ci_specs = readYaml file : specsDir + "/ci-spec.yml"
specs = specs + ci_specs
}
  println specs
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

 



