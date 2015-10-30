# Kex

Kex is a Kerl inspired tool to easy building and installing of [Elixir](http://elixir-lang.org) instances.

## Downloading

You can download the script directly from github:

```
$ curl -O https://raw.githubusercontent.com/user/kex/master/kex
```

Then ensure it is executable

```
$ chmod a+x kex
```

and drop it in your `$PATH`

## Usage

Update availables elixir versions  :

``` 
$ kex update
Updating...
```

Then list availables version :

```
$ kex list
Available versions:
v0.10.0 v0.10.1 v0.10.2 v0.10.3 v0.11.0 v0.11.1 v0.11.2 v0.12.0 v0.12.1 v0.12.2 v0.12.3 v0.12.4 v0.12.5 v0.13.0 v0.13.1 v0.13.2 v0.13.3 v0.14.0 v0.14.1 v0.14.2 v0.14.3 v0.15.0 v0.15.1 v0.5.0 v0.6.0 v0.7.0 v0.7.1 v0.7.2 v0.8.0 v0.8.1 v0.8.2 v0.8.3 v0.9.0 v0.9.1 v0.9.2 v0.9.3 v1.0.0 v1.0.0-rc1 v1.0.0-rc2 v1.0.1 v1.0.2 v1.0.3 v1.0.4 v1.0.5 v1.1.0 v1.1.0-beta v1.1.0-rc.0 v1.1.1
```

Pick your choise and install it :

```
$ kex install v1.1.1
Installing Elixir v1.1.1 in /home/user/.kex/installs/v1.1.1
You can activate this installation running the following command:
. /home/user/.kex/installs/v1.1.1/activate
Later on, you can leave the installation typing:
kex_deactivate
```

By default, the version is installed in `~/.kerl/installs/<version>`.  However you can chose the installation directory by specifying it as second parameter :

```
$ kex install v1.1.1 /opt/elixir/1.1.1
Installing Elixir v1.1.1 in /opt/elixir/1.1.1
You can activate this installation running the following command:
. /opt/elixir/1.1.1/activate
Later on, you can leave the installation typing:
kex_deactivate
```

Then activate it : 

```
. /opt/elixir/1.1.1/activate
```

You can list availables installations :

```
$ kex list-installs 
v1.0.5 /home/user/.kex/installs/v1.0.5
v1.1.0 /home/user/.kex/installs/v1.1.0
v1.1.1 /opt/elixir/1.1.1
```

You can also check which installation, if any, is currently active :

```
$ kex status
   v1.0.5 /home/user/.kex/installs/v1.0.5
   v1.1.0 /home/user/.kex/installs/v1.1.0
=> v1.1.1 /opt/elixir/1.1.1
```

You can also remove an installation :

```
$ kex delete v1.0.5
Delete Elixir installation v1.0.5 from /home/user/.kex/installs/v1.0.5
```

You can deactivate the current active installation :

```
$ kex_deactivate
``` 

Use `status` to ensure that there is no active installation :

```
$ ./kex status
No Elixir kex installation is currently active
``` 

## Licence  

[![](http://www.wtfpl.net/wp-content/uploads/2012/12/wtfpl-badge-4.png)](http://www.wtfpl.net/)

Copyright © 2015 Grégoire Lejeune  <gregoire.lejeune@free.fr>

This work is free. You can redistribute it and/or modify it under the terms of the Do What The Fuck You Want To Public License, Version 2, as published by Sam Hocevar. See the COPYING file for more details.

