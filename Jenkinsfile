node {
  scmVars = checkout scm
  def ecr = new org.bellhops.ECR()

  ecr.login('airflow', 'us-east-1')
  //Do not push until we've tested this.
  airflow_image = ecr.build('airflow', '.') 
}
