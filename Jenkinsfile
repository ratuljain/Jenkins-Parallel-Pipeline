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
                        stage ("smc:configerator.tumbleweed.paiwei") {
                            steps {
                                echo "Hello in parallel1 stage2"
                            }
                        }
                    }
                }

                stage ("PushPhase 2") {
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

        stage ("PreHealthCheckAction") {
            parallel {
                stage ("PushPhase 1") {
                    agent { label "master" }
                    stages {
                        stage ("smc:configerator.tumbleweed.paiwei") {
                            steps {
                                echo "Hello in parallel1 stage1"
                            }
                        }
                        stage ("smc:configerator.tumbleweed.paiwei") {
                            steps {
                                echo "Hello in parallel1 stage2"
                            }
                        }
                    }
                }

                stage ("PushPhase 2") {
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
        
        stage ("PushOverrideAction") {
            parallel {
                stage ("PushPhase 1") {
                    agent { label "master" }
                    stages {
                        stage ("smc:configerator.tumbleweed.paiwei") {
                            steps {
                                echo "Hello in parallel1 stage1"
                            }
                        }
                        stage ("smc:configerator.tumbleweed.paiwei") {
                            steps {
                                echo "Hello in parallel1 stage2"
                            }
                        }
                    }
                }

                stage ("PushPhase 2") {
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
        
        stage ("BakeAction") {
            parallel {
                stage ("PushPhase 1") {
                    agent { label "master" }
                    stages {
                        stage ("smc:configerator.tumbleweed.paiwei") {
                            steps {
                                echo "Hello in parallel1 stage1"
                            }
                        }
                        stage ("smc:configerator.tumbleweed.paiwei") {
                            steps {
                                echo "Hello in parallel1 stage2"
                            }
                        }
                    }
                }

                stage ("PushPhase 2") {
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
    }
}
