node('default') {
	step([$class: 'JUnitResultArchiver', keepLongStdio: true, testResults: 'junit/**/TEST-*.xml'])
}
