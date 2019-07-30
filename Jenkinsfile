#!groovy

pipeline {
    agent none

    stages {
        stage ("Stage1") {
            parallel {
                stage ("parallel1") {
                    agent { label "master" }
                    stages {
                        stage ("parallel1 stage1") {
                            steps {
                                echo "Hello in parallel1 stage1"
                            }
                        }
                        stage ("parallel1 stage2") {
                            steps {
                                echo "Hello in parallel1 stage2"
                            }
                        }
                    }
                }

                stage ("parallel2") {
                    agent { label "master" }

                    stages {
                        stage ("parallel2stage1") {
                            steps {
                                echo "Hello in parallel2stage1"
                            }
                        }
                    }
                }
            }
        }

        stage ("Stage2") {
          agent { label "master" }
          steps {
            echo "Hello in stage2"
          }
        }
    }
}
