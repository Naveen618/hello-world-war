pipeline {
    agent {label 'java'}
    stages ('checkout'){
        stage('checkout') {
            steps {	
		
                sh 'git clone https://github.com/Naveen618/hello-world-war'
            }
        }
stages ('build'){
steps {
sh 'mvn clean package'
}
}
stages ('print') {
steps {
	sh 'echo "hello world"'    
    }
}
