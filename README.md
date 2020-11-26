# EPAM Home Work #1

I used next commands to did all tasks:
```bash
ssh-keygen -t rsa -b 4096 -C "@gmail.com" # generate key for github
git config --global user.name "Lilia"
git config --global user.email @gmail.com 
git clone git@github.com:leskivl/EPAM_HW.git # clone repo to my pc
git checkout -b feature_x #create new branch
touch datePattern.txt # make new file
git add datePattern.txt # add file contents to the index
git status # check status 
git commit -m "Add regex to file" #create commit
git push # push changes to github 
git pull # gets changes after pull&request on github
```
A regular expression was written as same format YYYY/MM/DD HH:MM(:SS)
I create regular expression that provide next feature:
* Checks leap years
* Checks number of days in months
* Checks the correctness of the entered hour
* Check time with or without seconds 
```javascript
^([1-2][0-9]{3}[-/]?((0[13-9]|1[012])[-/]?(0[1-9]|[12][0-9]|30)|(0[13578]|1[02])[-/]?31|02[-/]?(0[1-9]|1[0-9]|2[0-8]))|([1-2][0-9](([2468][048]|[02468][48])|[13579][26])|([13579][26]|[02468][048]|0[0-9]|1[0-6])00)[-/]?02[-/]?29) (0?[0-9]|1[0-9]|2[0-3]|[0-9]):[0-5][0-9](:[0-5][0-9]){0,1}$
```
