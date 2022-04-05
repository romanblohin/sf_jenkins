pipeline {
    agent any

    stages {
        stage('My-JenkinsBuild-Steps') {
            steps {
               echo "Start getting data from db"
               sh   "mysql --user rfamro --host mysql-rfam-public.ebi.ac.uk --port 4497 --database Rfam < script.sql | tee /tmp/select_rfam.txt"
               echo "End"
            }
        }
    }
}
