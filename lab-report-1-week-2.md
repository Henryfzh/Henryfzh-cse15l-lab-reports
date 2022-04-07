# Tutorial for Incoming 15L Students
## Install Visual Studio Code(VSC)
- Go to the website below and click on install:
  [Link](https://code.visualstudio.com/)
- If you install it successfully, you can see it like this:
![@AC4GAYML2PH {V 8V6 DB4](https://user-images.githubusercontent.com/59184714/162260692-4209e540-9cae-405f-ad7c-2c735ade9729.png)
 
## Remote Connecting
- To start using remote connecting, we need to use SSH.
- The command should look like: *ssh cs15lsp22 + your id + @ieng.ucsd.edu*
- Then you need to enter your password and press enter
- If you see the following code, it means you enter the server!
![QQ图片20220407094749](https://user-images.githubusercontent.com/59184714/162255438-4284a780-28ce-4a5f-9340-bfa20657052f.png)

## Trying Some Commands
- **Move Files**: mv
- **List Files**: ls
- **List Hidden Files**: ls -a
- **Create Files**: touch + fileName
- **Create a Directory**: mkdir+ NewDirectoryName
- **Enter a Directory**: cd

## Move Files with scp
- Use the command:scp + fileName + cs15lsp22zz@ieng6.ucsd.edu:~/  Note: zz should be replaced by your user name
