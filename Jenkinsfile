node{
    stage('SCM checkout'){
        git 'https://github.com/vsknalli/secound-app'
    }
    stage('Compile-Package'){
        // Get Maven Home Path
        def mvnHome = tool name: 'maven-3', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
    }
}
