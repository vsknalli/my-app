node{
    stage('SCM checkout'){
        git 'https://github.com/vsknalli/my-app/'
    }
    stage('Compile-Package'){
        // Get Maven Home Path
        def mvnHome = tool name: 'maven-3', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
    }
    stage('Email Notification'){
    mail bcc: '', body: '''Hi Welcome to Jenkins job email alerts 
    Thanks 
    Senthil Veera''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'vsknalli@gmail.com,sabaa.23@gmail.com,deepan.redhat@gamil.com'
    }
}
