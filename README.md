# optional default grub live boot menu entry #

Adds a grub live boot menu entry as first option.

Existing grub boot entries stay unmodified.

Allows booting the system in live mode. Meaning, no persistent modifications
will be written to the disk. All changes stay in RAM.

No claims are made with regard to anti forensics.
## How to install `grub-default-live` using apt-get ##

1\. Download [Whonix's Signing Key]().

```
wget https://www.whonix.org/patrick.asc
```

Users can [check Whonix Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key) for better security.

2\. Add Whonix's signing key.

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg add ~/patrick.asc
```

3\. Add Whonix's APT repository.

```
echo "deb https://deb.whonix.org buster main contrib non-free" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `grub-default-live`.

```
sudo apt-get install grub-default-live
```

## How to Build deb Package ##

Replace `apparmor-profile-torbrowser` with the actual name of this package with `grub-default-live` and see [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/apparmor-profile-torbrowser).

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`grub-default-live` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
