node('master') {
	stage('checkout') {
		checkout scm
	}
	stage('junit Report') {
		sh 'touch junit/*/*.xml'
		step([$class: 'JUnitResultArchiver', keepLongStdio: true, testResults: 'junit/**/TEST-*.xml'])
	}
}
