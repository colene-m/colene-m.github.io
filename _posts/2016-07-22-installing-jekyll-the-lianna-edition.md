---
layout: page
title: "Installing Jekyll the Lianna Edition"
date: 2016-07-22
desc: "Instructions on how to install Jekyll for Lianna."
---
### Verification

1. Verify that you have  
    a.  Ruby (including headers): v1.9.3 or higher for Jekyll 2 and v2 or higher for Jekyll 3

        $ which ruby

     > **_Note:_** This should return a folder location, if not then ruby is not installed. If it does return a location do:
        ``` $ ruby --version ``` for the version update to the desired ruby version needed for Jekyll 2 or 3.
2. RubyGems -- this should come installed with Ruby automatically, verify with:

        $ which gem && gem --version

    > **_Note:_** The first part of the command check to see where RubyGems are installed and the second tells you the version (you can do both or just one of the commands).

3. NodeJS -- if you don't know what this is then you don't have it and it doesn't come installed automatically on any OS, but to check to see if you installed it already do:

        $ node -v

    > **_Note:_** If nothing is returned after running that command, then you need to install it (with Homebrew (this makes life sooo much easier)):  
    1. [Go here](http://brew.sh/)  
    2. Slap that command in the terminal -- wait for it to install  
    3. Install nodejs: ``` $ brew install node ```  
    4. Update homebrew and node: ``` $ brew update && brew doctor ```  
    5. Now check the node version again if all is well: ``` $ node -v ```  
    6. If something went wrong and you can't figure it out tnen let me know and I'll try to help.  
4. Python -- you need to have at least 2.7, check with:

        $ python -V

    > **_Note:_** If that command does something else type in: ``` $ exit() ``` to exit python and then do: ``` $ python --help ``` look for the switch to show you the version of python installed.

5. You made it!!

### Install Jekyll  
1. Install Jekyll with RubyGems:

        $ gem install

2. Initialize your blog site:  
    a. In a new folder:

        $ cd desired_root_location_here && mkdir folder_name_here && jekyll new blog_name_here

    b. In an existing folder:

        $ cd existing_folder_path && jekyll new .

    > **_Important:_** You may need to pass the ```--force``` option in ```jekyll new .``` if the directory isn't empty => ```jekyll new . --force```  

    > **_Note:_** The . (dot) refers to the current working directory (if you didn't know that).

3. Fire up your local instance of your jekyll blogging site:

        $ cd path_to_blog && jekyll serve

4. Navigate to: ```http://localhost:4000``` to view your blog  
5. Done!
