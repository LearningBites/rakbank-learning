# RAKBANK Learning Bites - Live Excel Sync Version

This package adds Live Excel Sync to the Dashboard.

What changed:
- Dashboard now has a Live Excel URL field.
- Paste your OneDrive/SharePoint Excel direct download link once.
- Click Save Live Excel URL.
- Click Sync Live Excel Now, or open the Dashboard and it will attempt to refresh automatically.
- Manual Excel upload still remains as a fallback.

Required Excel columns:
Date
Name
EmployeeID
Department
Course
Score
Attempts
Passed
Email

Important:
The Live Excel URL must be accessible by the browser. If your OneDrive/SharePoint link is private or blocked by browser permissions, Live Sync may fail. In that case, manual upload will still work.

Recommended flow:
Microsoft Forms > Power Automate > OneDrive Excel > Dashboard Live Sync.


## Dedicated Learner Link Fix
This version includes a separate Learner.html page.
Upload BOTH files to GitHub Pages:
- DemoInABox.html = admin/platform page
- Learner.html = learner-only page

In Settings > Hosted URL, paste your platform URL:
https://learningbites.github.io/rakbank-learning/DemoInABox.html

When you click Assign to All Learners, the generated learner links will automatically use:
https://learningbites.github.io/rakbank-learning/Learner.html#learn=...

This prevents learners from falling back to the admin/platform screen.
