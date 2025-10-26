pipeline{
    agent any

    stages{
        stage("Restore .NET packages"){
            steps{
                bat "dotnet restore" //for Windows
            }
        }
        stage("Build .NET Project"){
            steps{
                bat "dotnet build --no-restore" //for Windows
            }
        }
        stage("Run .NET tests"){
            steps{
                bat "dotnet test --no-build --verbosity normal" //for Windows
            }
        }
    }
    
}