pipeline{

	agent any
		tools{
			maven 'maven'
		}
		
	stages{
		stage('Bulid'){
			steps{
				git 'https://github.com/kunalmandavkar/Assignment'
				
				
				bat "mvn -Dmaven.test.failure.ignore=true clean package"
				
				echo 'Bulid Started'
			}
		}
	}
}