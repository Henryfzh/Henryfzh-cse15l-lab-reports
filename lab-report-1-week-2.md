# Tutorial for Incoming 15L Students
## Install Visual Studio Code(VSC)
- Go to the website below and click on install:
  [Link](https://code.visualstudio.com/)
- If you install it successfully, you can see it like this:
![@AC4GAYML2PH {V 8V6 DB4](https://user-images.githubusercontent.com/59184714/162260692-4209e540-9cae-405f-ad7c-2c735ade9729.png)
 
## Remote Connecting
- To start using remote connecting, we need to use SSH.
- The command should look like: (*ssh cs15lsp22 + your id + @ieng.ucsd.edu*)
- Then you need to enter your password and press enter
- If you see the following code, it means you enter the server!
![QQ图片20220407094749](https://user-images.githubusercontent.com/59184714/162255438-4284a780-28ce-4a5f-9340-bfa20657052f.png)

## Trying Some Commands
- **Move Files**: (mv)
* ![image](https://user-images.githubusercontent.com/59184714/163079210-05859120-1012-4f40-81a8-4a8452a7c2ad.png)

- **List Files**: (ls)
* ![image](https://user-images.githubusercontent.com/59184714/163078748-c2723032-7ac8-4005-b5c8-1845c31c08cf.png)
- **List Hidden Files**: (ls -a)
- ![image](https://user-images.githubusercontent.com/59184714/163078786-19849c3d-cb65-446f-aeca-aaebb2b4794a.png)

- **Create Files**: (touch + fileName)
- ![image](https://user-images.githubusercontent.com/59184714/163078963-ba8fb9d6-08ab-48af-b071-e3471424a734.png)

- **Create a Directory**: (mkdir+ NewDirectoryName)
- ![image](https://user-images.githubusercontent.com/59184714/163079091-3d34cacc-1617-4789-a666-ce76e5d09cb0.png)

- **Enter a Directory**: (cd)
- ![image](https://user-images.githubusercontent.com/59184714/163079141-577ba29e-0379-4d57-97be-203ca1e3042e.png)



## Move Files with scp
- First exit the server, and go back to local client
- Use the command:(scp + fileName + cs15lsp22zz@ieng6.ucsd.edu:~/)  Note: zz should be replaced by your user name
- If the file is sent successfully, you can see the following picture:
![38_X%U1_ILZ~4{EJQGA4X$X](https://user-images.githubusercontent.com/59184714/162260984-98f5f8b6-ec74-4675-937a-5a8db17707a0.png)

## Setting an SSH Key
- $ ssh-keygen
  After running this command you will see the following codes:
  ![JMQ@RDA2H($D)_ZMS)`D5~0](https://user-images.githubusercontent.com/59184714/162262922-c50f878d-94a9-4734-8f6e-24e44ab412af.png)
  (you can press enter to use default setting)
- If you have done successfully you will see the image of your key:
  ![6HY0E~CT(8`458X01$M8`P0](https://user-images.githubusercontent.com/59184714/162262379-4d246e53-6d52-456e-ab6d-8625b1a39806.png)
- if you are using windows you have several steps more, please go to following link and finish the steps:
  [Link](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement#user-key-generation)
- Go to the server and enter the command (*mkdir .ssh*), then exit the server back to client
- Use scp command to send the key to the server (the code should look like this): (*scp /Users/<user-name>/.ssh/id_rsa.pub cs15lsp22zz@ieng6.ucsd.edu:~/.ssh/authorized_keys*)
- If you finish all the steps, you can log in your server without entering password!

## Optimizing Remote Running
- You can write a command in quotes at the end of an ssh command to directly run it on the remote server
  ![image](https://user-images.githubusercontent.com/59184714/162264787-682a6a9e-6227-4ef7-bbde-6e5c8132ec54.png)
- You can run multiple commands on the same line by using *;* to seperate them
  ![image](https://user-images.githubusercontent.com/59184714/162264692-44b97dce-25ef-4e00-8548-df894b1ef97d.png)
- You can use up-arrow to back to your last command 
