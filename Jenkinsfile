node {
  // Mark the code checkout 'stage'....
  stage 'Stage Checkout'
  
  git branch: 'jira/NMS-9328', url: 'https://github.com/opennms/opennms.git'
  sh 'docker run -v ./opennms:/usr/src/opennms "/fullbuild.sh -DskipTests=true"'
}
