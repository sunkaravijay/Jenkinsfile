try {
			node('master'){

				stage('Code Checkout')
				cleanWs()

				status.check([

					branch: 'main',

					repo: 'https://github.com/Harshilbhardwaj47/spring-petclinic.git'

				])

				

				stage('Code build')



				build.check([


					command1 : "clean install",




				])
			}
		} catch(Exception ex) {
			println ex.getCause();
			println ex.getMessage();
		}
