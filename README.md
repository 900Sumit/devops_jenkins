# devops_jenkins
Task 4: Integrating Jenkins with GitHub (with Timer Trigger)

Using Jenkins + GitHub

1. Create GitHub Repository
Go to GitHub → Create a new repository
Add your project files (or a simple README.md)
2. Create Jenkins Job
Open Jenkins → New Item
Enter name → Select Freestyle Project → OK
3. Connect Jenkins with GitHub
In job configuration:
Go to Source Code Management
Select Git

Enter Repository URL:

https://github.com/your-username/your-repo.git
4. Add Build Step
Go to Build → Add build step
Select Execute Windows batch command

Add:

echo Hello from Jenkins + GitHub Integration
5. Add Timer Trigger (Important)
Go to Build Triggers

Select:

Build periodically

Add cron expression:

H/2 * * * *

👉 This means:

Job will run every 2 minutes automatically
6. Save and Run
Click Save
Wait for scheduled run OR click Build Now
7. Verify Output
Open build → Console Output
Check execution logs
