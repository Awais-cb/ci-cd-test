pipeline {
        agent any
        stages {
            stage ('build') {
                steps {
                    echo 'In Build Stage.........'
                }
            }
            stage ('test') {
                steps {
                    echo 'In Test Stage...'
                }
            }
            stage ('deploy') {
                steps {
                    echo 'git pull'
                    sh "cd /var/www/html/ci_cd_test"
                    // sh "git checkout master"
                    sh "git pull"
                }
            }
        }
}
