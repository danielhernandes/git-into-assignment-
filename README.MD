<h1 align="center">Creating SSH AND LEARNING GIT</h1>
<!-- Table of Content -->

<li>
    <a href="#GenerateSSHKey">Generate SSH Key</a>

</li>

<li>
    <a href="https://www.youtube.com/">Youtube</a>

</li>

# Generate SSH Key

<p>SSH stands for Secure Shell and is a method used to establish a secure connection between two computers.
SSH works by authenticating based on a key pair, with a private key being on a remote server and the corresponding public key on a local machine. When the keys match, access is granted to the remote user.</p>

## Step 1 Verify if OpenSSH Client is Installed

1. Open the Settings panel, then click Apps.
2. Under the Apps and Features heading, click Optional Features.
3. Scroll down the list to see if OpenSSH Client is listed.

   - If it’s not, click the plus-sign next to Add a feature.
   - Scroll through the list to find and select OpenSSH Client.
   - Finally, click Install.

![ssh1](https://user-images.githubusercontent.com/69836474/153216693-1aacb42a-2f58-4888-ad32-c1cdae3e92ce.JPG)
![ssh2](https://user-images.githubusercontent.com/69836474/153216776-a8b2bfb6-cef6-4b29-b90f-430c7fb91336.JPG)

## Step 2 Open Command Prompt

1. Press the Windows key.
2. Type cmd.
3. Under Best Match, right-click Command Prompt.
4. Click Run as Administrator. <br>
   ![step2 ssh](https://user-images.githubusercontent.com/69836474/153217077-f1021f1e-9223-4fe2-8794-a1149e147948.JPG)
5. If prompted, click Yes in the Do you want to allow this app to make changes to your device? pop-up.

## Step 3 Use OpenSSH to Generate an SSH Key Pair

1. In the command prompt, type the following:

   ```sh
   ssh-keygen
   ```

2. By default, the system will save the keys to C:\Users\your_username/.ssh/id_rsa. You can use the default name, or you can choose more descriptive names. This can help distinguish between keys, if you are using multiple key pairs. To stick to the default option, press Enter.
3. You’ll be asked to enter a passphrase. Hit Enter to skip this step.
4. The system will generate the key pair, and display the key fingerprint and a randomart image.
5. Open your file browser.
6. Navigate to C:\Users\your_username/.ssh.
7. You should see two files. The identification is saved in the id_rsa file and the public key is labeled id_rsa.pub. This is your SSH key pair.
8. You can open copy your ssh by opening the file in notepad.

## Step 4 Add SSH into Github Account

1. Go to your Github Account.
2. GO to setting
3. Click on SSH & Key
4. Create the name and copy the key and then save.

# GitTutorial

1. create a new repository
2. Dont add anything let it be empty first.
3. echo "# git-into-assignment-" >> README.md
4. git init
5. git add README.md
6. git commit -m "first commit"
7. git branch -M main
8. git remote add origin https://github.com/danielhernandes/git-into-assignment-.git
9. git push -u origin main
