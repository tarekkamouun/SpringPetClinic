node {  
    stage ('Checkout'){
        git branch: 'main', url: 'https://github.com/tarekkamouun/SpringPetClinic.git'
    }
    stage ('Build'){
        withMaven(maven: 'M3'){
           bat 'mvn compile'
        }
    }
     stage ('Test'){
        withMaven(maven: 'M3'){
           bat 'mvn test'
        }
    }
     stage ('Package'){
        withMaven(maven: 'M3'){
           bat 'mvn package'
        }
    }
}
