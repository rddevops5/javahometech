node{
        stage('checkout'){
    sh '''
   git 'https://github.com/rddevops5/javahometech.git'

    '''
   }
        stage('Build'){
    sh '''
    mvn clean package
    '''
   }
   stage('Docker-build'){
    sh '''
    ls
    pwd
    docker build -t rddevops5/webapp:2.0.0 .
    '''
   }
}
