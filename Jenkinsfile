pipeline {
	agent any
	stages {
		stage('Clone Git Repo'){
				steps{
					git 'https://github.com/qaboxletstest/cypress-jenkins-demo.git'
		    }
		}
		stage('Install Dependencies'){
				steps{
					git 'npm install'
				}
		}
		stage('Run Tests'){
				steps{
					git 'npm test'
				}
		}
		// stage('Publish HTML Report'){
		// 		steps{
		// 			publishHTML([allowMissing: false, alwaysLinkToLastBuild: false, keepAll: false, reportDir: 'cypress/reports/mochareports', reportFiles: 'report.html', reportName: 'HTML Report', reportTitles: ''])
		// 		}
		// }
	}
}