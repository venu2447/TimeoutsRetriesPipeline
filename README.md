# TimeoutsRetriesPipeline
  The "Deploy" stage retries the flakey-deploy.sh script 3 times, and then waits for up to 3 minutes for the health-check.sh script to execute. If the health check script does not complete in 3 minutes, the Pipeline will be marked as having failed in the "Deploy" stage.  "Wrapper" steps such as timeout and retry may contain other steps, including timeout or retry.
