Mutt + OfflineIMAP + MSMTP + Gnome-Keyring = EMAIL CLIENT
=========================================================

## Get all things:

```
# install some from ubuntu package manager
sudo apt-get install mutt mutt-patched msmtp seahorse libsecret-tools gpicview abook urlview mairix maildir-utils abook

# install keyring for python to use gnome-keyring
sudo pip2 install keyring

# get offlineimap from github, here I use v6.5.6
wget https://github.com/OfflineIMAP/offlineimap/archive/v6.5.6.tar.gz
tar -xvf v6.5.6.tar.gz
cd v6.5.6
sudo python setup.py install

# get vcard2abook to convert vcard to abook
wget https://raw.github.com/yaroot/scripts/master/vcard2abook.py
python3 vcard2abook.py  -f /data/Downloads/contacts.vcf -o /data/Dropbox/Private/Contacts/abook

```

## Config things:

All my things is in this repo.


## Run things:

```
# First thing first
offlineimap

# Second thing second
mairix -v

# Third thing last
mutt

```

## Fix somethings:

```
# chmod for msmtprc
chmod 600 ~/.mutt/msmtprc

```

## Not done yet

**How to sync contacts?**

## Reference:

[Here][1], [here][2] and [here][3].

[1]: https://www.proteansec.com/linux/the-ultimate-guide-to-mutt/
[2]: http://stevelosh.com/blog/2012/10/the-homely-mutt
[3]: http://www.google.com
