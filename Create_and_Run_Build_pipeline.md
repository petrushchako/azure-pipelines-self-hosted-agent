1. On the left menu, click Pipelines.

2. Click Create Pipeline.

3. Select Azure Repos Git.

4. Select the application repository.

5. Select the ASP.NET pipeline template.

6. In the YAML under pool, delete the vmImage line and replace it with the following:

```pool:```
```  name: Default```
7. Click Save and run > Save and run.

A status window will appear stating the pipeline needs permissions to access a resource before this run can continue.

8. In the status window, click View > Permit > Permit.

9. To verify our job ran on the selected agent once the build has run, click Project settings > Agent pools > Default > Agents.

10. Click the listed agent to see the job attached to the agent.
