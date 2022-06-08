node {
    stage('Git Clone') {
       git credentialsId: 'git', url: 'https://github.com/alvorg11/alv.git'
    }
	stage('Maven Version') {
      sh 'mvn --version'
    }
    stage('Maven Clean') {
      sh 'mvn clean'
    }
    stage('Maven Validate') {
      sh 'mvn validate'
    }
	stage('Maven Compile') {
      sh 'mvn compile'
    }
	stage('Maven Test') {
      sh 'mvn test'
    }
	stage('Maven Package') {
      sh 'mvn package'
    }
    stage('Maven Deploy') {
      sh 'mvn deploy'
    }
}

