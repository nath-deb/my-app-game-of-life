node{
	stage('SCM Checkout')
		git 'https://github.com/nath-deb/my-app-game-of-life'
	}
	stage('Compile-Package'){
		//Get maven home path
		def mvnHome = tool name "maven-3", type: 'maven'
		sh "${mavnHome}/bin/mvn package"
	}
}
