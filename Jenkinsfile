pipeline
{
    agent
    {
        docker
        {
            image 'praqma/native-gradle'
            args '-v $HOME/.m2:/home/jenkins/.m2 -v $HOME/.gradle:/home/jenkins/.gradle'
        }
    }
    stages
    {
        stage ('Increment version')
        {
             steps
             {
                 sh './gradlew incrementVersion'
             }
        }
        
        stage ('build')
        {
            steps
            {
                sh "mkdir -p /home/jenkins/.m2"
                sh "./gradlew publish"
            }
        }
        stage ('results')
        {
            steps
            {
                archiveArtifacts 'build/distributions/*.zip'
            }
        }
    }
}
