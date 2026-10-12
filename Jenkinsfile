pipeline{
    agent any
    stages{
        stage("Restore the project"){
            bat 'dotnet restore'
        }
        stage("Build the project"){
            bat 'dotnet build --no-restore'
        }
        stage("Run the tests"){
            bat 'dotnet test --no-build --verbosity normal'
        }
    }
}