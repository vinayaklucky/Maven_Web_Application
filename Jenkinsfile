node('master') {
    stage('Continuous Download') {
    git branch: 'main', changelog: false, poll: false, url: 'https://github.com/mddevopsaws/Maven_Web_Application.git'
	}
    stage('Continuous Build') {
    sh '/var/lib/jenkins/tools/hudson.tasks.Maven_MavenInstallation/Maven_-_3.9.4/bin/mvn clean package'
	}
    stage('Continuous Deploy') {
    sh 'echo "Deploymnet Passed"'
	}
}
