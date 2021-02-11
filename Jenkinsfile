pipeline {
    agent none

    stages {
        stage ("Detemine Targets") {
            parallel {
                stage ("PushPhase 1") {
                    agent { label "master" }
                    stages {
                        stage ("smc:configerator.tumbleweed.paiwei") {
                            steps {
                                echo "Hello in parallel1 stage1"
                            }
                        }
                    }
                }

                stage ("PushPhase 2") {
                    agent { label "master" }

                    stages {
                        stage ("smc:configerator.tumbleweed.rajain") {
                            steps {
                                echo "Hello in parallel1 stage2"
                            }
                        }
                    }
                }
            }
        }

        stage ("Detemine Targets") {
            parallel {
                stage ("PushPhase 1") {
                    agent { label "master" }
                    stages {
                        stage ("smc:configerator.tumbleweed.paiwei") {
                            steps {
                                echo "Hello in parallel1 stage1"
                            }
                        }
                    }
                }

                stage ("PushPhase 2") {
                    agent { label "master" }

                    stages {
                        stage ("smc:configerator.tumbleweed.rajain") {
                            steps {
                                echo "Hello in parallel1 stage2"
                            }
                        }
                    }
                }
            }
        }

    }
}
