pipeline {
     agent {
    // Equivalent to "docker build -f Dockerfile.build --build-arg version=1.0.2 ./build/
    dockerfile {
        filename 'Dockerfile-login'
        dir '.'
        label 'login-app'
        additionalBuildArgs  '--build-arg version=1.0.2'
        args '-v /tmp:/tmp'
    }
 }
  stages {
     stage('Image build') {
      steps {
                  
            echo "Build image" 
      } 
    }

}
 
