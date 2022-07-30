pipeline 
{
    agent any

    stages 
    {
        stage('Build') 
        {
            steps 
            {
                echo 'Building App'
            }
        }

        stage('Test') 
        {
            steps 
            {
                echo 'Testing App'
            }
        }

        stage('Deploy') 
        {
            steps 
            {
                echo 'Deploying App'
            }
        }
    }

    post
    {

    	always
    	{
    		emailext body: 'Summary', subject: 'Pipeline Status', to: 'abirbeatz@gmail.com'
    	}

    }
}
