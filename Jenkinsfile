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
    		emailext body: 'Hey! Your Pipeline Steps are complete on Jenkins. Feel free then have a look! ', subject: 'Report on Pipeline Summary', to: 'abirbeatz@gmail.com'
    	}

    }
}
