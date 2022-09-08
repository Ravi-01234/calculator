pipeline {
	agent any
	tools {
    	maven 'my_mvn'
	}
	stages {
    	stage("Checkout") {   
        	steps {               	 
            	git url: 'https://github.com/Ravi-01234/calculator'          	 
           	 
        	}    
    	}
    	stage('Build') {
        	steps {
        	bat "mvn compile"  	 
        	}
    	}
   	 
    	stage("Unit test") {          	 
        	steps {  	 
            	bat "mvn test"          	 
       	}
}
}
}
