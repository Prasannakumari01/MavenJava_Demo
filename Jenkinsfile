node {
    stage('Checkout Code') {
        git url: 'https://github.com/Prasannakumari01/MavenJava_Demo.git',
            branch: 'main'
    }

    stage('Build') {
        echo "Building Maven project..."
        sh "mvn clean install"
    }

    stage('Run Tests') {
        echo "Running Tests..."
        sh "mvn test"
    }

    stage('Package') {
        echo "Packaging the project..."
        sh "mvn package"
    }

    stage('Post Build') {
        echo "Build completed successfully!"
    }
}

