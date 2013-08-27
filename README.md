twiliosh
========

Yet another Twilio command line client. However, it only requires curl and a simple, plain-text
configuration file (stuck in ```$HOME/.twiliosh.conf```) to get started. Ideal for being notified of the
completion of long-running tasks.

Usage
========

Send a default message to the default number:

```sh
twiliosh
```

Send a default message to a specified number:

```sh
twiliosh -n 4085551212
```

Send a specified message to a specified number:

```sh
twiliosh -n 4085551212 -m "Hello from $HOSTNAME"
```

Send a specified message to a specified number using the specified configuration file:

```sh
twiliosh -n 4085551212 -m "Hello from $HOSTNAME" -c ~/.my.twiliosh.conf
```

Example configuration file:

```sh
export TWILIO_SID=b150dcc45d2cfc3cfa383496cd23d0d05b
export TWILIO_AUTHTOKEN=710fa32bf38c3ed9f61c64fe50b94fb3
export TWILIO_NUMBER=+14085551212
export TWILIO_DEFAULT_RECIPIENT=+14085551212
```

