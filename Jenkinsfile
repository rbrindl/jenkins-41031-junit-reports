node('master') {
	stage('checkout') {
		checkout scm
	}
	stage('junit Report') {
		step([$class: 'JUnitResultArchiver', keepLongStdio: true, testResults: 'junit/**/TEST-*.xml'])
	}
}
