# update-db-repo

To make this workflow work, you need the following three things:
1. Databricks token or service principle: See [this link](https://docs.databricks.com/dev-tools/api/latest/authentication.html) for creating PAT and [this link](https://docs.databricks.com/administration-guide/users-groups/service-principals.html) for creating service principle
2. Workspace instance name: See [this link](https://docs.databricks.com/workspace/workspace-details.html#workspace-instance-names-urls-and-ids) for more details
3. Repo id: unique id of the repo that you want to update. You can get this id from [opening the git dialog](https://docs.databricks.com/repos/index.html#open-the-git-dialog)
<img width="1002" alt="Screen Shot 2022-04-03 at 3 46 16 PM" src="https://user-images.githubusercontent.com/55514721/161452003-9b1220c5-f447-48d7-8a3f-d5f7731c759d.png">


Once you have the above, input the above values as below:
1. Create a GitHub Actions secret with the name "DB_TOKEN" and paste the Databricks token or service principle into it.
2. Enter the workspace instance name and repo id to the ".github/workflow.yml"

Feel free to customize the workflow to make it work for your use case. That is, you can change which events should trigger the workflow or what branch should be updated. 
