pipeline{
    agent any
    stages{
        stage('inspect server'){
            steps{
                bat'"C:\\Program Files\\git\\bin\\bash.exe" -c "chmod +x sysinfo.sh && ./sysinfo.sh"'

            }
        }
    }
}