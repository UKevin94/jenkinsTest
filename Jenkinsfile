node {
   stage 'Stage 1 : sanity check'
   echo 'OK pipelines work in the test instance'
   stage 'Stage 2 : steps check'
       def workflow_id = runSquashWorkflow(
           workflowPathName:'./peac.yaml',
           workflowTimeout: '20S',
           serverName:'defaultServer'
       )
       
       echo "We just ran The Squash DEVOPS workflow $workflow_id"
}
