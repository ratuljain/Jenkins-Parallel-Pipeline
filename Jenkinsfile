pipeline {
    agent none

    stages {
        stage ("Detemine Targets") {
            parallel {
                stage ("P1") {
                    agent { label "master" }
                    stages {
                        stage ("smc:configerator.tumbleweed.paiwei") {
                            steps {
                                echo "Hello in parallel1 stage1"
                            }
                        }
                    }
                }

                stage ("P2") {
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

        stage ("HealthCheck") {
            parallel {
                stage ("P1") {
                    agent { label "master" }
                    stages {
                        stage ("smc:configerator.tumbleweed.paiwei") {
                            steps {
                                echo "Hello in parallel1 stage1"
                            }
                        }
                    }
                }

                stage ("P2") {
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
        
        stage ("RestartTargetsAction") {
            parallel {
                stage ("P1") {
                    agent { label "master" }
                    stages {
                        stage ("smc:configerator.tumbleweed.paiwei") {
                            steps {
                                echo "Hello in parallel1 stage1"
                            }
                        }
                    }
                }

                stage ("P2") {
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
        
        stage ("BakeAction") {
            parallel {
                stage ("P1") {
                    agent { label "master" }
                    stages {
                        stage ("smc:configerator.tumbleweed.paiwei") {
                            steps {
                                echo "Hello in parallel1 stage1"
                            }
                        }
                    }
                }

                stage ("P2") {
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
