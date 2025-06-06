# gitlab-ctl

> Manage the GitLab omnibus.
> More information: <https://docs.gitlab.com/omnibus/maintenance/>.

- Display the status of every service:

`sudo gitlab-ctl status`

- Display the status of a specific service:

`sudo gitlab-ctl status {{nginx}}`

- Restart every service:

`sudo gitlab-ctl restart`

- Restart a specific service:

`sudo gitlab-ctl restart {{nginx}}`

- Display the logs of every service and keep reading until `<Ctrl c>` is pressed:

`sudo gitlab-ctl tail`

- Display the logs of a specific service:

`sudo gitlab-ctl tail {{nginx}}`

- Send the SIGKILL signal to specific service:

`sudo gitlab-ctl kill {{nginx}}`

- Reconfigure the application:

`sudo gitlab-ctl reconfigure`
