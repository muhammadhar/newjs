pipeline
{
    agent any
        tools
        {
            nodejs "16.20.2"
        }
        stages
        {
            stage('version npm')
            {
                steps
                {
                sh 'npm version'
                }
            }
            stage('clone github') 
            {
            steps {
                git 'https://github.com/thezeeshanasghar/sha.git'
            }
            }
            
            stage('Test') {
            steps {
                sh 'ls'
             //   sh 'npm install'
              //  sh 'npm test'
            }
        }
            stage('Build') {
            steps {
                sh 'npm install'
                sh 'npm run build'
            }
        }
}
}
