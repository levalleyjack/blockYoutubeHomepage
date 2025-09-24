# blockYoutubeHomepage
This is a guide on how to block both the "Homepage" and "Related Videos" features on Youtube

<img width="2557" height="1339" alt="image" src="https://github.com/user-attachments/assets/a9ada1cc-7122-4fa1-8201-2fc60db9fe3e" />

## Step 1:
Install uBlock Origin. This is the best in class open source adblocker with tons of features such as the ability to modify the HTML of the site when the page loads. We will be using this specific feature.

## Step 2:
Click on the settings tab of uBlock Origin

<img width="254" height="524" alt="Screenshot 2025-09-22 153036" src="https://github.com/user-attachments/assets/82db1ec2-bcb3-4755-8ad4-4854f238062e" />


## Step 3:
Navigate to "My Filters" and paste the following in:
```
youtube.com##ytd-browse[page-subtype="home"]
youtube.com###related
```
If you would like to also block Youtube shorts, then paste this instead:
```
youtube.com##ytd-browse[page-subtype="home"]
youtube.com###related

! blocks YT-Shorts
youtube.com##ytd-guide-entry-renderer:has-text(Shorts)
youtube.com##ytd-mini-guide-entry-renderer:has-text(Shorts)
youtube.com##ytd-shorts.ytd-page-manager.style-scope
```
## Step 4: 
Click "Apply Changes" and become more productive
