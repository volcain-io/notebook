# Security

Index of contents:

1. [The Matrix](#the-matrix)

## The Matrix

1. Create two or more identities
    Insulate as much as possible between these identities
        -> They shouldn't talk about the same stuff
        -> They shouldn't know each other
        -> They shouldn't buy the same things
        -> Diligently separate them from your original physical identity
            -> maintain different wallets, bags, user accounts & computers
+ Change MAC Address (=Unique 48 bit identifier burned into the EEPROM on the card)
    -> This is only important if you don't wish the LAN admin is able
        to identify you. MAC addresses do not cross router boundaries.
    -> Works on Ethernet, Wireless, Token Ring
    -> [MAC Address Spoofing](https://wiki.archlinux.org/index.php/MAC_address_spoofing)
        WIRED:
        sudo ifconfig enp7s0 down
        sudo macchanger -r enp7s0      " OR: ifconfing enp7s0 hw enter de:ad:be:ef:f0:0d)
        sudo ifconfig enp7s0 up
        WIRELESS:
        sudo ifconfig wlp8s0 down
        sudo macchanger -r wlp8s0
        sudo ifconfig wlp8s0
+ Change 802.11 nickname
    -> sends your hostname to the AP
        sudo iwconfig eth0 nickname "Fucko the Clown"
+ DHCP Properties
+ Get a VPN at [Mullvad](https://mullvad.net)
