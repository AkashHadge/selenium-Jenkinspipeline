node ('windows'){
	stage ('SCM checkout'){
		git "https://github.com/AkashHadge/selenium-Jenkinspipeline"
		}
	stage ('Build'){
    	dir("comtest") {
	   bat "mvn install"
       }
	}
    stage ('test') {
    	bat "java -jar comtest/target/com.test-1.0-SNAPSHOT.jar"
    }
}
