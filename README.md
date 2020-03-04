# le-scan
Let's Encrypt Revocation Event, for full details see [my blog](https://scotthelme.co.uk/lets-encrypt-to-revoke/).

I'm also keeping a [Twitter thread](https://twitter.com/Scott_Helme/status/1234853555116421121) up to date with information.

The purpose of this project is to scan all hosts that may be affected and identify who still needs to replace a certificate due for imminent revocation at **2020-03-04 20:00 UTC (3:00pm US EST)**.

The file `log.txt` contains a list of all hosts that are affected and is derived from the official list provided by Let's Encrypt. The file can be found [here](https://www.dropbox.com/s/tp47jrpge6brv2g/log.txt?dl=0).

The file `need-renewing.txt` is the result of my crawler scanning those hosts to see which are still using certificates that are due to be revoked and thus need replacing ASAP.

In the `results` folder are country based lists of hosts that are still affected. The hope is that individuals will choose a list and work to notify hosts on that list that they need to take action. 

If you'd like to pick up a list please leave a comment on [this bug](https://github.com/ScottHelme/le-scan/issues/1) so that we don't double up on lists and spam organisations with notifications.

The data on the lists will be updated at regular intervals throughout the day. If a host is on the list they definitely need to take action!