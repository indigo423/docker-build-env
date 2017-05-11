node {
    // Mark the code checkout 'stage'....
    stage ('Stage Checkout') {
        git branch: 'jira/NMS-9328', url: 'https://github.com/opennms/opennms.git'
    }

    stage ('Compile and Assemble') {
        sh 'docker run --rm -v $(pwd)/opennms:/usr/src/opennms opennms/build-env /fullbuild.sh -DskipTests=true'
    }
}
