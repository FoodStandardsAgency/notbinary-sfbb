## How to copy a Github wiki from one repo to another (with a clean history)

1. Create a new repo

2. Create a wiki page in the new repo (a default homepage is fine just to get it initiated)

3. Create a new folder on your desktop (or wherever) and launch the terminal/console

4. Clone source wiki repo

For this one:
`git clone git@github.com:notbinary/discovery-template.wiki.git`

For another repo:
`git clone git@github.com:username/sourceRepoName.wiki.git`

5. Clone new wiki repo

`git clone git@github.com:username/newRepoName.wiki.git`

6. Navigate to new wiki folder

`cd newRepoName.wiki`

7. Copy in the source wiki files

For this one:
`cp -r ../discovery-template.wiki/*.md ./`

For another repo:
`cp -r ../sourceRepoName.wiki/*.md ./`

8. Add all new files

`git add .`

9. Commit all to new repo

`git commit -m "Add source wiki content to new wiki repo“`

10. Push all to new repo

`git push`