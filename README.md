# MathSlax

A typesetting solution for all of your [Slack](https://slack.com/) chat needs.

# Dependencies
Requires Java, Node.JS and NPM.

```shell
$ sudo apt-get install nodejs npm default-jre
```

# Set up
```shell
$ cd mathslax
$ make install
$ SERVER=myhostname.com PORT=9999 node server.js
```

Set up an outgoing web hook in Slack pointing to `myhostname.com:9999/typeset`
(don't forget the `/typeset`). Use `math!` as the prefix.

# Usage
In the Slack channel with the web hook configured, you should be able to
typeset equations by starting your message with `math!`. For example, `math!
x^2 * sin(x)` would cause the `mathslax` bot to comment with a link to a
typeset image of `x^2 * sin(x)`.
