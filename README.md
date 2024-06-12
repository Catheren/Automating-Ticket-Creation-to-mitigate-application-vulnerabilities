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

