node {
    stage('createImage') {
        sh 'echo "Creating Dockerfile..."'
        sh 'echo "FROM ubuntu:16.04" > Dockerfile'
        sh 'echo "ENV MYSQL_HOST=DB_Server" >> Dockerfile' 
        sh 'echo "ENV MYSQL_PASSWORD=5TTnvuTDJJSq6" >> Dockerfile'
        sh 'echo "LABEL description=Test_Twistlock_Jenkins_Plugin" >> Dockerfile' 
        sh 'docker build --no-cache -t dev/my-ubuntu:$BUILD_NUMBER .'
    }
}
