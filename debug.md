# **cd into server directory**

`cd t27/server`

# **Run the language server**

`mvn eclipse:eclipse`

(as a bonus you'll get all the nice tab completions, warning and error squiggles, pop-up method/variable info etc.)

you'll get this error while this is running but just ignore it: 

> Path '/s/parsons/g/under/mpbarbel/Projects/CS314_FRESH/t27/target/classes' must denote location inside project 'server'

# **Add a `launch.json` config file**

![image](https://github.com/user-attachments/assets/9634e38a-fbcb-4182-ac2d-1ec3fc489dbf)

select "java" from the menu:

![image](https://github.com/user-attachments/assets/1cdb3ea9-20ea-4f9e-b56c-fb6a2e8e9819)

This will generate a generic `launch.json` file. There will be some other general configurations in there already, you can leave them or delete them.

# **Select "Add Configuration" from the Run and Debug dropdown menu**

![image](https://github.com/user-attachments/assets/a7c05f68-68ba-471f-8ef4-9b63250bc733)

Select "{} Java: Attach to Process" from dropdown menu

![image](https://github.com/user-attachments/assets/788ac85e-2888-41ca-8e6b-a8ca5cbf4997)

# **Add `"projectName:" "server"` to the config block** 

Don't forget the comma separating the previous statement

![image](https://github.com/user-attachments/assets/5d8787c5-b0dd-480b-8837-5bd46f75e668)

Save the file when complete.

This will enable the "watch" variable functionality.

# **Run the bin.sh script**

`cd ..`

`./bin/run.sh`

# **Under Run and Debug dropdown menu, select "Attach by Process ID" then click the little green arrow next to the menu

![image](https://github.com/user-attachments/assets/7fc52a2f-6731-4186-8c10-4b7a741b2fc2)

# **Select the running process from the dropdown menu

![image](https://github.com/user-attachments/assets/64ccd711-a0af-4bd4-8f89-cb845f492694)

# **Debug**

Set a breakpoint in the code. You can now interactively debug by triggering a request from the app running on localhost:43127

![image](https://github.com/user-attachments/assets/86f2c01f-8021-4b40-882e-dd4e762e00a2)

# **Add files to .gitignore**

Add `.classpath` and `launch.json` to your .gitignore so they're not annoying




