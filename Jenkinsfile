pipeline {
	agent any
	stages {
    stage ('checkout'){
            steps {		
                sh 'git clone https://github.com/Naveen618/hello-world-war.git'
            }
        }
stage ('build'){
steps {
sh 'mvn clean package'
}
}
stage ('print') {
steps {
	sh 'echo "hello world"'    
    }
}
    }
}
