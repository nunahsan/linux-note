### Create Custom Shortcut Command
1. nano ~/.bashrc

2. create new line using following syntax
`# alias <your_shotcut>='<real_command>'`

3. example :
`alias dc='docker-compose'`

4. save the file

5. refresh the profile by running the following command
`source ~/.bashrc`

6. try your command
`dc ps`
