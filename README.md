# RStudio cloud github configuration for exams and project deadline

Many of the problems with not being able to push to the class organisation can be solved on q-rap rstudio by having a linked GitHub account.  Go to this link to do this [https://login.rstudio.cloud/identity/authentication](https://login.rstudio.cloud/identity/authentication)

You should see the below image once you have done this

![](photo.png)

**Once linked, your identity will be configured for you.**


Alternative you may have to do this manually as follows:

```
git config —-global user.email “you@example.com”
```

```
git config —-global user.name “Your Name”
```
To prevent your credentials from expiring after 15 minutes, a cache has been configured for 12 hours. The cache duration can be modified through the cache credential helper bundled with git. The command below would set the timeout to an hour:

```
git config —-global credential.helper ‘cache —-timeout 3600’
```

From the git documentation: “this command caches credentials in memory for use by future git programs. The stored credentials never touch the disk, and are forgotten after a configurable timeout. The cache is accessible over a Unix domain socket, restricted to the current user by filesystem permissions.”
