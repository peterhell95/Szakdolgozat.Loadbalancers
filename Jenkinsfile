pipeline {
    agent any
    stages {
        stage('Apply Kubernetes Angular Loadbalancer') {
            steps{
        	withKubeConfig([credentialsId: 'my_kubernetes2',  serverUrl: 'https://192.168.41.137:8443']) {
      			bat 'kubectl apply -f service-angular-lb.yaml'
   			}
  		}
    	 }

	  stage('Apply Kubernetes Apigateway Loadbalancer') {
            steps{
        	withKubeConfig([credentialsId: 'my_kubernetes2',  serverUrl: 'https://192.168.41.137:8443']) {
      			bat 'kubectl apply -f service-apigateway-lb.yaml'
   			}
  		}
    	 }

	  stage('Apply Kubernetes Books Loadbalancer') {
            steps{
        	withKubeConfig([credentialsId: 'my_kubernetes2',  serverUrl: 'https://192.168.41.137:8443']) {
      			bat 'kubectl apply -f service-books-lb.yaml'
   			}
  		}
    	 }

	  stage('Apply Kubernetes Order Loadbalancer') {
            steps{
        	withKubeConfig([credentialsId: 'my_kubernetes2',  serverUrl: 'https://192.168.41.137:8443']) {
      			bat 'kubectl apply -f service-order-lb.yaml'
   			}
  		}
    	 }
	
	  stage('Apply Kubernetes Rate Loadbalancer') {
            steps{
        	withKubeConfig([credentialsId: 'my_kubernetes2',  serverUrl: 'https://192.168.41.137:8443']) {
      			bat 'kubectl apply -f service-rate-lb.yaml'
   			}
  		}
    	 }
	
	  stage('Apply Kubernetes Search Loadbalancer') {
            steps{
        	withKubeConfig([credentialsId: 'my_kubernetes2',  serverUrl: 'https://192.168.41.137:8443']) {
      			bat 'kubectl apply -f service-search-lb.yaml'
   			}
  		}
    	 }
    }
}