# JSON
 1. Create a remote repository named JSON.
    - Go to GitHub account ;
    - click on the `new repository` button ;
    - enter Repository name "JSON" ;
    - click on the `Public` button ;
    - click `Add a README file` ;
    - click on `Create repository` button
 
 ----
2. Clone the JSON repository to the local computer.
   - Go to the repository page ;
   - click on `Code` => `Local`=> ` SSH` => `Copy link` ;
   - on PC open terminal  => enter command `mkdir git_hw_1` => `cd git_hw_1` =>  `git clone git@github.com:olyacenko/JSON.git`
```
dmitrijostalskij@MacBook-Pro-2 hw_ksendzov_courses % mkdir git_hw_1
dmitrijostalskij@MacBook-Pro-2 hw_ksendzov_courses % cd git_hw_1
dmitrijostalskij@MacBook-Pro-2 git_hw_1 % git clone git@github.com:olyacenko/JSON.git
Cloning into 'JSON'...
remote: Enumerating objects: 36, done.
remote: Counting objects: 100% (36/36), done.
remote: Compressing objects: 100% (31/31), done.
remote: Total 36 (delta 11), reused 8 (delta 0), pack-reused 0
Receiving objects: 100% (36/36), 9.57 KiB | 3.19 MiB/s, done.
Resolving deltas: 100% (11/11), done.
dmitrijostalskij@MacBook-Pro-2 git_hw_1 % 
```
 ----
3. Inside the local JSON, create a "new.json" file.
```
dmitrijostalskij@MacBook-Pro-2 git_hw_1 % cd JSON 
dmitrijostalskij@MacBook-Pro-2 JSON % touch new.json  
dmitrijostalskij@MacBook-Pro-2 JSON % 
```
----
4. Add the file for tracking git.
```
dmitrijostalskij@MacBook-Pro-2 JSON % git add new.json 
```
----
5. Commit the file.
```
dmitrijostalskij@MacBook-Pro-2 JSON % git commit -m "add file new.json"
[main 0651027] add file new.json
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new.json
dmitrijostalskij@MacBook-Pro-2 JSON % 
```
----
6. Send the file to the remote GitHub repository.
```
dmitrijostalskij@MacBook-Pro-2 JSON % git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 284 bytes | 142.00 KiB/s, done.
Total 3 (delta 0), reused 1 (delta 0)
To github.com:olyacenko/JSON.git
   58a0052..0651027  main -> main
dmitrijostalskij@MacBook-Pro-2 JSON % 
```
----
7. Edit the content of the file "new.json" - write information about yourself (full name, age, number of pets, future desired salary). Write everything in JSON format.
```
dmitrijostalskij@MacBook-Pro-2 JSON % cat >> new.json
{
"name": "Olya",
"surname": "Yatsenko",
"age": 29 ,
"pets": null ,
"future_salary": 500
}
^C
dmitrijostalskij@MacBook-Pro-2 JSON %
```
----
8. Send the changes to the remote repository.
```
dmitrijostalskij@MacBook-Pro-2 JSON % git add new.json
dmitrijostalskij@MacBook-Pro-2 JSON % git commit -m "add data to new.json"
[main 9845d11] add data to new.json
 1 file changed, 7 insertions(+)
dmitrijostalskij@MacBook-Pro-2 JSON % git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 360 bytes | 360.00 KiB/s, done.
Total 3 (delta 0), reused 1 (delta 0)
To github.com:olyacenko/JSON.git
   0651027..9845d11  main -> main
dmitrijostalskij@MacBook-Pro-2 JSON % 
```
----
9. Create "preferences.json" file
```
dmitrijostalskij@MacBook-Pro-2 JSON % touch preferences.json 
```
----
10. In the preferences.json file, add information about your preferences (Favorite movie, favorite show, favorite food, favorite time of year, party you would like to visit) in JSON format.
```
dmitrijostalskij@MacBook-Pro-2 JSON % cat >> preferences.json
{
"favourite_movie": "A beautiful mind",
"favourite_series": "The Sopranos",
"favourite_meal": "meat",
"favourite_time_of_year": "summer",
"country_would_like_visit": "Canada"

}
^C
dmitrijostalskij@MacBook-Pro-2 JSON % 
```
----
11. Create skills.json file and add information about skills that will be learned on the course in JSON format.
```
dmitrijostalskij@MacBook-Pro-2 JSON % cat > skills.json
{
"Basic_theory": "What is testing, bug reports, documentation, types, methods, testing directions, SDLC, STLC.",
"Client-server_architecture": "Theory of client-server architecture",
"HTTP": "HTTP methods, HTTP server response codes, structures of HTTP inputs and responses",
"JSON_XML": "JSON, XML structure",
"Postman": "API testing via Postman, JS, API autotests",
"Logs": "Removing and reading logs from an external server",
"Charles_Fiddler": "Sniffing http web traffic and interception of traffic on iOS, Android",
"Dev_Tools": "Web Dev Tools of Google Chrome, FireFox",
"VPN": "How it works, why you need it, how to use it, tool options",
"Mobile_testing": "Features of mobile testing, special cases",
"iOS_Android": "Feature, guidelines",
"XCode": "Building iOS applications",
"Android_Studio": "Building Android applications",
"ADB": "Android device management",
"Proxy_vpn": "Setting up on iOS and Android",
"Terminal_Linux": "copy, create, view, move files on servers without a graphical interfacsh_scripting": "Automation of routine tasks on the server",
"SQL": "basic operators: create, delete, delete, insert, select from, where, join)",
"Postgres": "database installation, configuration and use",
"Redis": "Non-relational database installation, configuration and use",
"Scrum": "Theory of Development Methodology"
}
^C
dmitrijostalskij@MacBook-Pro-2 JSON % 
```
----
12. Send 2 files at once to the remote repository.
```
dmitrijostalskij@MacBook-Pro-2 JSON % git add skills.json preferences.json
dmitrijostalskij@MacBook-Pro-2 JSON % git commit -m "add files skills.json and preferences.json"
[main 409de06] add files skills.json and preferences.json
 2 files changed, 31 insertions(+)
 create mode 100644 preferences.json
 create mode 100644 skills.json
dmitrijostalskij@MacBook-Pro-2 JSON % git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.16 KiB | 1.16 MiB/s, done.
Total 4 (delta 0), reused 2 (delta 0)
To github.com:olyacenko/JSON.git
   9845d11..409de06  main -> main
dmitrijostalskij@MacBook-Pro-2 JSON % 
```
----
13. Create bug_report.json file on the web interface.
    - go to the remote repository ;
    - click `Add file` button ;
    - `Create new file` ;
    - enter name of the file "bug_report.json" ; 
-----
14. Make Commit changes (save) the changes on the web interface.
    - click `Commit changes` => enter the description "create bug_report.json " ;
    - click `Commit directly to the main branch` ;
    - click `Commit changes` 
----
15. On the web interface, modify bug_report.json file, add bug report in JSON format.
    - click on the file "bug_report.json" ;
    - click `edit this file` ;
    - add data to the file
----
16. Make Commit changes (save) the changes on the web interface.
    - click `Commit changes` => enter the description "add data to bug_report.json " ;
    - click `Commit directly to the main branch` ;
    - click `Commit changes`
----
17. Synchronize remote and local JSON repository.
```
dmitrijostalskij@MacBook-Pro-2 JSON % git pull
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), done.
From github.com:olyacenko/JSON
   409de06..01ce2e8  main       -> origin/main
Updating 409de06..01ce2e8
Fast-forward
 bug_report.json | 20 ++++++++++++++++++++
 1 file changed, 20 insertions(+)
 create mode 100644 bug_report.json
dmitrijostalskij@MacBook-Pro-2 JSON % 
```










   
