node('linux') {
		stage('Test') {
		    git 'https://github.com/ikewrobel/java-project.git'
		    sh 'ant -buildfile test.xml'
		}
		stage('Results'){
		    junit 'reports/result.xml'
		}
		stage('Build'){
		    sh 'ant'
		    sh 'ant -f build.xml -v'
		    
		}
}
