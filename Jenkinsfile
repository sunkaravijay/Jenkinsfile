try {
			node('master'){

				stage('Code Checkout')
				

				status.check([

					branch: 'main',

					repo: 'https://github.com/Harshilbhardwaj47/spring-petclinic.git'

				])

				

				stage('Code build')



				build.check([


					command1 : "clean install",




				])
				stage('Code Test')
				
				build.check([


					command1 : "test",

				])
			}
		} catch(Exception ex) {
			println ex.getCause();
			println ex.getMessage();
		}
