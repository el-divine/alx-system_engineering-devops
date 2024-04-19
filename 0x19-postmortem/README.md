Report / Postmortem
Issue Summary:
On April 19, 2024, between 9:00 AM and 11:00 AM West African Time, users experienced a service outage for our website. During this period, users were unable to access the website, and some users reported errors when attempting to access certain pages. Approximately 75% of our users were affected. The root cause of the outage was a typo in the wp-settings.php file, which gave it the extension "phpp" instead of "php."
Timeline:
8:00 AM: The issue was first detected when users reported errors while accessing certain pages of the website.
8:05 AM: The monitoring system alerted the team to a spike in server errors.
8:10 AM: The team began investigating the server logs and identified that the errors were related to the wp-settings.php file.
8:20 AM: The team identified that the file had been incorrectly named with a "phpp" extension instead of "php."
8:30 AM: The team attempted to revert the file to its previous state but encountered errors.
9:00 AM: The team realized that the file had been incorrectly modified by a junior developer who had mistakenly saved the file with the wrong extension.
9:20 AM: The team escalated the incident to senior management and communicated the impact of the outage.
10:00 AM: The team successfully restored the wp-settings.php file to its correct state and tested the website to ensure it was functioning properly.
11:00 AM: The website was fully restored and users were able to access it without any issues.
Root Cause and Resolution:
The root cause of the outage was a typo in the wp-settings.php file, which gave it the extension "phpp" instead of "php." This error caused the website to fail to load correctly, resulting in the service outage. To resolve the issue, the team identified and corrected the typo in the wp-settings.php file, restored it to its correct state, and tested the website to ensure it was functioning properly.
Corrective and Preventative Measures:
To prevent similar issues from occurring in the future, the team will implement the following corrective and preventative measures:
Increase code review processes to ensure all changes are thoroughly reviewed before being deployed to the website.
Implement stricter naming conventions to prevent similar typos in file extensions.
Implement a testing environment to ensure changes can be thoroughly tested before deployment.
Improve documentation and training for junior developers to prevent similar errors from occurring in the future.
Conclusion:
The service outage on May 11, 2023, was caused by a typo in the wp-settings.php file, which gave it the extension "phpp" instead of "php." The team was able to quickly identify and correct the issue, restoring the website to its normal state within two hours. The team will take steps to prevent similar issues from occurring in the future by implementing stricter code review processes, naming conventions, and improving documentation and training for junior developers.
