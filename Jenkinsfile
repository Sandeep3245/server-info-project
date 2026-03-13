pipeline{
    agent any
    stages{
        stage('inspect server'){
            steps{
                bat'"C:\\Program Files\\git\\bin\\bash.exe" -c "chmod +x sysinfo.sh && ./sysinfo.sh"'

            }
        }
          stage('Trigger Next Pipeline') {
            steps {
                echo 'Passing the baton to Pipeline-B...'
                build job: 'Running SH commands', wait: false
            }
        }
    }
}