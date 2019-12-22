
node
{
    stage('clone the source code'){
        git 'https://github.com/nagendra464/mahalogin.git'
    }
    stage('convert the java files to class file'){
        sh label: '', script: 'mvn package'
    }
    stage('test the source code with selinium tool'){
        sh label: '', script: 'mvn test'
    }
    stage('transfer the data from workspace to local'){
        sh label: '', script: 'mvn install'
    }
    stage('sucess'){
        sh label: '', script: 'echo "the new file is added"'
    }
    
}
