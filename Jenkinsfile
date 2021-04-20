node('master'){
 
stage('Code Checkout')
 cleanWs()

                status.check([

                branch: 'master',

                repo: 'https://github.com/Harshilbhardwaj47/spring-petclinic.git'
                  
               ])
  
   def specs = [:]
  def specsDir = "./Specs/V1.0"

if(fileExists(specsDir + "/ci-spec.yml")){
 bat cd
ci_specs = readYaml file : specsDir + "/ci-spec.yml"
specs = specs + ci_specs
}
  println specs
  
  stage('Code build')

                

                build.check([

              
              command1 : specs.Build.command1,
       

                

                ])

}

 



