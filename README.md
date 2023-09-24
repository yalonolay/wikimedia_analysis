# Analyzing Wikipedia

a repository for fetching data on Wikipedia in order to analyze it.
Contains 2 different jobs:
1. "pages" - fetches data on pages in Wikipedia
2. "users" - fetches data on users in Wikipedia

## Run
In order to run the code, first go to `wikimedia_analysis` and run:
```bash
pip install -r requirements.txt
```
Then, run the following command:
```bash
python main.py -j=<job_name>
```
where `<job_name>` is either `pages` or `users`.

Sample of wiki pages data:
```csv
                   page_name                                           page_url     last_fetch_page_name_ts    
5          "O"-Jung.Ban.Hap.  https://he.wikipedia.org/wiki/%22O%22-Jung.Ban...  2023-09-02 21:23:19.138335        
6  "The Spaghetti Incident?"  https://he.wikipedia.org/wiki/%22The_Spaghetti...  2023-09-02 21:23:19.139723        
7               "אבא גוריון"  https://he.wikipedia.org/wiki/%22%D7%90%D7%91%...  2023-09-02 21:23:19.141204        
8                 "אינטגרנד"  https://he.wikipedia.org/wiki/%22%D7%90%D7%99%...  2023-09-02 21:23:19.142446        
9          "אני רופא, לא..."  https://he.wikipedia.org/wiki/%22%D7%90%D7%A0%...  2023-09-02 21:23:19.143879   
```

Sample of wiki users data:
```csv
      user_name   user_id  edits_size_bytes tags is_hidden_user      page_name user_talk kohelet_talk 
0      Lionster   99779.0                64   []        [False]  טורס דל פיינה      None         None 
1         Ewan2   48020.0                42   []        [False]  טורסד דה פואה      None         None     
2  Anna.kiselov  205151.0              1847   []        [False] טורסד דה פואנט      None         None   
3       Bom2013  234567.0              3789   []        [False] טורסד דה פואנט      None         None     
4        DMbotY   41054.0              1993   []        [False] טורסד דה פואנט      None         None
```

## Information about users you can find here:   
1. [Wiki HE user list](https://he.m.wikipedia.org/w/index.php?title=%D7%9E%D7%99%D7%95%D7%97%D7%93:%D7%A8%D7%A9%D7%99%D7%9E%D7%AA_%D7%9E%D7%A9%D7%AA%D7%9E%D7%A9%D7%99%D7%9D&group=sysop)
2. [Wiki EN user list](https://en.wikipedia.org/wiki/Special:ListUsers)