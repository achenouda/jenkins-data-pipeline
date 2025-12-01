pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
		    git branch: 'main' , url: 'https://github.com/achenouda/jenkins-data-pipeline.git'
                    sh 'pip install pandas' // Installer les dépendances
                    sh 'python3 data_analysis.py' // Exécuter le script Python
                }
            }
        }
    }
}
