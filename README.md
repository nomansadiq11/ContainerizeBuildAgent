# Azure DevOps Build Agents Containerize as Docker Container

Microsoft documentation URL : https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/docker?view=azure-devops

### Note:

Using Linux Image you can make CI/CD .Net Core, Nodejs, Python using your own build agent. 

### Pre-requisite

- Azure DevOps Account (https://azure.microsoft.com/en-in/services/devops/)
- Create Personal Token (https://docs.microsoft.com/en-us/azure/devops/organizations/accounts/use-personal-access-tokens-to-authenticate?view=azure-devops&tabs=preview-page)


### How to use Linux Docker Container Image

| Steps      | Action | Comments |
| ------------- | ------------- | ------------- | 
| 1       | docker push nomansadiq11/azurebuildagent:linux   | Pull docker image from docker hub |
| 2 | docker run -e AZP_URL=https://dev.azure.com/organization -e AZP_TOKEN=PersonalAccessToken -e AZP_AGENT_NAME=mydockeragent nomansadiq/azurebuildagent:linux  | Replace organization with your Azure DevOps Organization and Replace PersonalAccessToken with your Personal Access token |


