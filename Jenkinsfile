stage('Deploy in Test env') {
            when {
                branch 'test'
            }            
        steps {
                sh "kubectl apply -f deployment.yaml"
            }
        }

        stage('Deploy in Prod env') {
            when {
                branch 'prod'
            }
            steps {
                sh "kubectl apply -f deployment.yaml"
            }
        }
