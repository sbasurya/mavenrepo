pipeline {
        agent {
  label 'Jenkins-node-slave'
}
	
	    stages {
      stage('MVN Clone') {
            steps {
                git branch: 'master', url: "https://github.com/sbasurya/mavenrepo.git"
            }
		}
		stage('MVN Build') { 
            steps {
                echo "hello MVN Build Stage"
				sh "/usr/local/src/apache-maven/bin/mvn package" 
            }
        }
 }
}
© 2020 GitHub
