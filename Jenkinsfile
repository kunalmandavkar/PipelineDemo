pipeline{

	agent any
		tools{
			maven 'maven'
		}
		
	stages{
		stage('Bulid'){
			steps{
				git 'https://github.com/kunalmandavkar/PipelineDemo'
				
				
				bat "mvn -Dmaven.test.failure.ignore=true clean package"
				
				echo 'Bulid Started'
			}
		}
	}
}