# gitlab_dashboard
GitLab dashboard for viewing assigned issues and milestones

**REQUIREMENTS**  
1. Authentication with login | pass
2. Viewing milestones with issues
3. Viewing the task assignee and their issues

**PURPOSE:**  
Create dashboard for fast analyze tasks and the workload of the developers

**LINKS:**
1. We can use that NodeJS library https://www.npmjs.com/package/gitlab

**TASK:**
1. When logging in, the user must enter a username and password.  
Request example:  
```CURL
echo 'grant_type=password&username=<your_login>&password=<your_pass>' > auth.txt
curl --data "@auth.txt" --request POST http://gitlab.dk/oauth/token
```
Response:
```JSON
{"access_token":"8eeb43b80002d00f03b600642d5798e5e5822b0473e2fd1825dc16b614805172",
"token_type":"bearer",
"refresh_token":"e180fe9c9e053e360475f329772d567556bf9faee42f357f327fbea1ceaaa5fc",
"scope":"api",
"created_at":1587487049}
```
2. After authorization we need display dashboard with projects and number of open issues for the each project  
Request Projects List:

