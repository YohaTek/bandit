# Level 0

The first level is just a login. No password is given up front — level 0 is
reached with the password published on the wargame page.

Connect over SSH to port 2220:

```sh
ssh bandit0@13.63.65.121 -p 2220
```

If your network restricts outbound SSH, tunnel the same connection through
`proxychains`:

```sh
proxychains ssh bandit0@13.63.65.121 -p 2220
```

## Notes

- Port `2220` is required; plain `ssh bandit0@13.63.65.121` will fail.
- `proxychains` needs a working proxy configured in
  `/etc/proxychains4.conf` before the tunnelled form will connect.
