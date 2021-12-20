pipeline {
	agent {label 'slave-3'}
	stages {
    stage ('checkout'){
            steps {		
                sh 'git pull https://github.com/Naveen618/hello-world-war.git'
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
stage ('deploy') {
steps {
	sh 'sudo chmod 777 /opt'
	sh 'sudo cp -R /var/lib/jenkins/workspace/Test1/target/hello-world-war-1.0.0.war /opt/apache-tomcat-9.0.56/webapps'
	sh 'echo "hello world"'    
    }
}
    }
}
