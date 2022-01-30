# HAL-remote-control
This is the repo for all the helper scripts and executables to push and pull between a local machine and HAL (in NCSA, UIUC).

## Steps to Use (all on local machine)

-   Install `expect` using command line, like `brew install expect` or `sudo apt install expect`.
-   Move the two `.exp` files into your workdir.
-   Create a file called `account.key` in the same dir, and input your account for HAL in the first line, and password for HAL in the second line. example:

```txt
haob2
FAKED_PASSWD
```

-   If you want to pull, you will pull the whole dir with all the single files using `expect pull.exp <dir_name>`. If your files is in a subdir, you have to pull them one more time. 
-   If you want to push, you can only push one file at a time, using `expect push.exp <dir_name/file_name>`.
-   After executing `expect`, you will find your *DUO* software on your mobile devices pushes you a notification to sign in. Please choose `Approve`.

![image-20220129225943590](http://jacklovespictures.oss-cn-beijing.aliyuncs.com/2022-01-30-045944.png)

## Play with the code

You can always change the script as you like. Reading through it is more than simple. Enjoy!

