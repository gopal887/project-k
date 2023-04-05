pipeline{
    agent { label 'ubuntu' }
    parameters{
        string(name: 'MAVEN_GOAL', defaultValue: 'clean install', description: 'maven goal')
    }
    triggers{
        cron('* * * * *')
    }
    stages{
        stage('vcs'){
            steps{
                git branch: 'REL_INT_1.0',url: 'https://github.com/GitPracticeRepo/spring-petclinic.git'

            }
        }
    }
}