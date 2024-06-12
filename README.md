# Integrating-Sonarcloud-with-Github-Actions
This project will show the steps to integrate Sonarcloud to Github Actions so that the code is scanned for vulnerabilities during every new commit.

**What is SonarCloud?**
SonarCloud is a cloud-based service that analyzes your code for issues. It integrates with your development workflow to find bugs, security vulnerabilities, and code smells. This helps you write cleaner and more reliable code. SonarCloud is free for open-source projects and offers a free trial for private projects.

To do this project, you need create an account on Github and SonarCloud. 

1. After you logged in to SonarCloud, create an Organization. 
![image](https://github.com/Catheren/Integrating-Sonarcloud-with-Github-Actions/assets/94724571/d5d460ff-6c8e-4875-a67f-e9a1fc29d6a7)
2. Import your Github repository.
![image](https://github.com/Catheren/Integrating-Sonarcloud-with-Github-Actions/assets/94724571/107d70fc-3245-4bc8-92cf-8e521c52480e)

3. Create an organization as shown in the figure:

![image](https://github.com/Catheren/Integrating-Sonarcloud-with-Github-Actions/assets/94724571/8d353539-6e1b-48b1-8b30-6a273c90f0c2)

_**Note**: Provide a key as per the requirement. I have redacted mine._
4. Go to **Analyze Projects** and select the repository you would like to scan. Select **Setup**.
![image](https://github.com/Catheren/Integrating-Sonarcloud-with-Github-Actions/assets/94724571/89b0e0dc-19b8-44a1-9c50-5cb34782a2c3)

5. Setup how often or after what action you want your repository to be scanned.
![image](https://github.com/Catheren/Integrating-Sonarcloud-with-Github-Actions/assets/94724571/184be103-a1e2-4b61-b9cd-f347410d65e3)

Sonarcloud will start scanning your selected repository and provide the results as shown:
![image](https://github.com/Catheren/Integrating-Sonarcloud-with-Github-Actions/assets/94724571/cba20fc3-86a9-422b-a40d-504dac809cda)
And every single time a code commit is made, it will rescan the code to find any new vulnerabilities.

# Integrating Sonarcloud with JIRA for ticket management
Jira is a project management tool developed by Atlassian. It's particularly popular for Agile project management, but can be used for various project types. 
To integrate JIRA with Sonarcloud so that tickets can be automatically created and assigned to Developers based on the issues on code.
To do this, 
1. Go to JIRA console. Select **Apps**.
2. Select **Explore more apps**. Search for SonarQube connector in the search bar.
![image](https://github.com/Catheren/Integrating-Sonarcloud-with-Github-Actions/assets/94724571/35c74cda-300c-4f6d-84e1-5c23c08a98b0)
3. Once Sonarqube connector is added, select **Manage App**.
![image](https://github.com/Catheren/Integrating-Sonarcloud-with-Github-Actions/assets/94724571/4e07345f-7a1f-483d-8e5c-d4ff864e0d89)

5. Select **SonarQube connector** to manage the global settings of Sonarqube connector.
6. Enter the required information.
7. To get the token, go to Sonarcloud page and select **Settings>Security**.
8. Generate tokens and copy the token and paste on JIRA.
9. To provide the Resource Key, go to Sonarcloud portal, select the desired project.
    - Go to **Administration>Update Key**. Copy the project key and paste it.
11. Click **Save**.
Now, we will be able to see the SonarQube tab on our project.
And we can see the information on Sonarcloud is reflected on the project. 
Compare the following images.
![image](https://github.com/Catheren/Integrating-Sonarcloud-with-Github-Actions/assets/94724571/8f911b82-2d5a-42bd-8db2-34f224a4e2d0)
![image](https://github.com/Catheren/Integrating-Sonarcloud-with-Github-Actions/assets/94724571/1202d189-b96b-47e8-920a-40534587ba20)
You can now assign tasks and tickets to the corresponding developers so that code vulnerabilities can be mitigated.
