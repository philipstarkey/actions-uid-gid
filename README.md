# actions-uid-gid

Test repository for showing uid and gid in GitHub Actions virtual environment.

## Context

ubuntu 18.04 LTS has an [`id`](http://manpages.ubuntu.com/manpages/bionic/man1/id.1.html) command which prints user and group information for the specified USER, or (when USER omitted) for the current user.

```shell
# print only the effective user ID (also known as UID)
id --user 

# print only the effective group ID (also known as GID)
id --group
```

As of November 26, 2019, running these commands in GitHub Actions' Virtual Environment on `ubuntu-latest` will [show a UID of `1001` and GID of `115`.](https://github.com/francisfuzz/actions-uid-gid/commit/d27a19b212282f0401cfd3fc3b7d0b932dd63751/checks?check_suite_id=329888828#step:2:5)
