# ansible_challenges

## challenge 1
1) Write a playbook to install Nginx and ensure that it is running on port 7510. When accessing the web page on a server it should tell you the time of day eg. 'Morning', 'Afternoon', 'Evening' on the first line of the page, under that it should provide the hostname, IP address, and what environment it is on.

eg.
```console
[Production]
servera

[Development]
serverb

[Test]
serverc
```

2) There is a file called test.html in /var/www/html which needs to be accessible from the web. In that file there are multiple typos of the word TeSting that should be testing. Everything else in the file should remain the same.

3) ensure each user(s) from a list called users exists on the system setting the username to the username value, along with adding them to a group (same with UID) if given, and generate a password if a password isn't already set for each user that has alpha numeric and special characters in it. This password should be saved in a file /root/.USERNAME.password with the permissions 700.

eg.
```yaml
users:
  - first: Bob
    last: Builder
    username: bbuilder
    group: dev
    uid: 1230
```
