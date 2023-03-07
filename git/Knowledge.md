# All about git


## Set my self as a verified author of commits (Well, I want to see my commit with verified badge its something nice 😂)



### In GitLab

https://docs.gitlab.com/ee/user/project/repository/gpg_signed_commits/


### Create GPG

```ssh

# Use this command for the default version of GPG, including
# Gpg4win on Windows, and most macOS versions:
gpg --gen-key

# Use this command for versions of GPG later than 2.1.17:
gpg --full-gen-key

```


### If you havee GPG, then check what is applicable

```ssh

gpg --list-secret-keys --key-id LONG
```


### Once you found it 👀 , then its time to export it (get the ID - its located after "rsa****/")

```ssh

gpg --armor --export <ID>
```


### Assuming I added it and I am brilliant ! Then set the config `user.signingkeey` and possibly `user.email` on the repo only not globally

```ssh

git config user.email "my email"

git config user.signingkey "the key on gitlab, the gpg you added"
```

### As a result 🚀



<img src="verifiedsht.PNG" alt="verified" />


<br>
<br>
<br>

### ***Note that is is for GPG only, check https://docs.gitlab.com/ee/user/project/repository/ssh_signed_commits/ for SSH***