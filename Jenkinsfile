pipeline 
{
    agent any

    stages 
	{
        stage('Build') 
		{
            steps {
                echo 'Build App'
            }
        }
		
		stage('Test') 
		{
            steps {
                echo 'Test App'
            }
        }
		stage('Deploy') 
		{
            steps {
                echo 'Deploy App'
            }
        }
    }
	
	post 
	{
        always 
		{
            
           emailext attachLog: true, body: 'Pipeline Summry', subject: 'Pipeline Script Status', to: 'deeep0400@gmail.com'
        }
	}
}
