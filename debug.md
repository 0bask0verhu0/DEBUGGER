# **cd into server directory**

`cd t27/server`

# **Run the language server**

`mvn eclipse:eclipse`

(as a bonus you'll get all the nice tab completions, warning and error squiggles, pop-up method/variable info etc.)

you'll get this error while this is running but just ignore it: 

> Path '/s/parsons/g/under/mpbarbel/Projects/CS314_FRESH/t27/target/classes' must denote location inside project 'server'

# **Add a `launch.json` config file**

![1](https://github.com/user-attachments/assets/9c4a927b-ded4-471a-b61f-bde8bba56736)


select "java" from the menu:

![2](https://github.com/user-attachments/assets/af888e1a-c242-4056-95c8-0b256bc8798b)


This will generate a generic `launch.json` file. There will be some other general configurations in there already, you can leave them or delete them.

# **Select "Add Configuration" from the Run and Debug dropdown menu**

![3](https://github.com/user-attachments/assets/bf4d51b3-b34b-461b-8bb4-01ff6385078f)


Select "{} Java: Attach to Process" from dropdown menu

![4](https://github.com/user-attachments/assets/105a1535-29c6-4ac7-985e-a7a974e80b0f)


# **Add `"projectName:" "server"` to the config block** 

Don't forget the comma separating the previous statement

![5](https://github.com/user-attachments/assets/6cc18fd8-5b53-43c4-bec8-5522ee74f11e)


Save the file when complete.

This will enable the "watch" variable functionality.

# **Run the bin.sh script**

`cd ..`

`./bin/run.sh`

# **Under Run and Debug dropdown menu, select "Attach by Process ID" then click the little green arrow next to the menu

![6](https://github.com/user-attachments/assets/33d9e1ce-7a39-47fb-9c40-b2c8e41dbc54)


# **Select the running process from the dropdown menu

![7](https://github.com/user-attachments/assets/634c82a8-4793-49f3-8e1a-918be29662b1)

# **Debug**

Set a breakpoint in the code. You can now interactively debug by triggering a request from the app running on localhost:43127

![8](https://github.com/user-attachments/assets/a9a6a1f4-dcbf-4e3f-9560-42ac8f16f94d)


# **Add files to .gitignore**

Add `.classpath` and `launch.json` to your .gitignore so they're not annoying




