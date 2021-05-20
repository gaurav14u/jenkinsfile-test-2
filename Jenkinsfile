pipeline {
    agent any
    parameters {
        choice(name: 'INSTANCENAME', choices: ['One', 'Two', 'Three'], description: 'Pick something')
        choice(name: 'ACTION', choices: ['Start', 'Stop', 'Status'], description: 'Pick something')
    }
    stages {
        stage('Example') {
            steps {
                script{
                  if(${params.INSTANCENAME} == 'One'){
                    echo "INSTANCENAME ${params.INSTANCENAME}"
                  }
                  echo "ACTION: ${params.ACTION}"
                }
            }
        }
    }
}
