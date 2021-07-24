pipeline
{
agent any
stages
{
   stage('Clone_the_code')
   { steps { echo 'code is downloading'  } }

   stage('Execute unit test case')
   { steps { echo "Execute unit test case" }  }

   stage('Building code')
   { steps { echo "Building code" }  }

   stage('Deploy package to a dev server')
   { steps { echo "Deploy package to a dev server" }  }

   stage('Approval from QA manager')
   {steps { input 'please approve qa deployment?' }}  //wait for approval to proceed to execute next stage

   stage('Deploy package to a qa server')
   { steps { echo "Deploy package to a qa server" }  }

    stage('Approval from Release manager')
   {steps { input 'please approve Release deployment?' }}  //wait for approval to proceed to execute next stage

   stage('Deploy package to a prod server')
   { steps { echo "Deploy package to a prod server" }  }

}
}