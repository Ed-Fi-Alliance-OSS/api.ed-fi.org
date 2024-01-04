# Vision: Automation

Notes in brief, to be fleshed out as we learn more about IT expectations:

1. TerraForm is available to us for managing desired-state.
2. Azure DevOps is the desired orchestration tool.
3. We need to deploy from pre-built NuGet packages or Docker containers, rather
   than letting Azure DevOps rebuild the code.
4. All automation needs to be fully scripted (no point-and-click required), and
   the scripts / configuration files should be in this repository.
   * Taking care, of course, to keep environment variables and secrets in
     appropriately safe locations, not in source code.
5. Need to configure log export / ingestion into Azure Monitor.
