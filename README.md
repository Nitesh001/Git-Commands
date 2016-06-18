# Git-Commands

To configure Git in local system

git config --global user.name "Nitesh001"
git config --global user.email "its.nits.world@gmail.com"

SSH (Secure Shell):

It uses RSA encryption to share public key between two systems.
For windows download Putty which is a very SSH client.
Now open Git Bash shell to generate ssh

Type: 
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

output:
# Creates a new ssh key, using the provided email as a label
Generating public/private rsa key pair.

Now enter passphrase (any password) for 2 times simultaneously

After this, add SSH key to the SSH agent:

First enable SSh agent
eval $(ssh-agent -s)
It will generate agent pid.

Now, add SSH key to the agent:
ssh-add ~/.ssh/id_rsa

Now, SSH key is generated. This has to be added in our github account.

This key is stored in .pub file.

Now open id_rsa.pub file located in C://Users/Nitesh/.ssh
copy entire text without any extra space.







