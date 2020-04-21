# gitlab_dashboard
GitLab dashboard for viewing assigned issues and milestones

**REQUIREMENTS**  
1. Authentication with login | pass
2. Viewing milestones with issues
3. Viewing the task assignee and their issues

**PURPOSE:**  
Create dashboard for fast analyze tasks and the workload of the developers

**TASK:**
1. When logging in, the user must enter a username and password.  
Example:  
```CURL
echo 'grant_type=password&username=<your_login>&password=<your_pass>' > auth.txt
curl --data "@auth.txt" --request POST http://gitlab.dk/oauth/token
```
2. After authorization we need display dashboard with projects and assignes
