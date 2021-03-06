Totem AirPlay Plugin
--------------------------------------------------------------------------------

A FOSS Python PoC implementation of the server side AirPlay Protocol.

It announces the AirPlay service over avahi to any iOS devices capabable of
AirPlay and allows a video to be played back in Totem easily.

The playback can also be controlled from the iOS device including play/pause
aswell as seeking to certain time offsets.

AirPlay photo "playback" is not supported.

Future versions could act as a client themself and allow Totem to stream
media to iOS capable servers like the Apple TV 2 or other computers running
Totem with AirPlay support.

Requirements
--------------------------------------------------------------------------------

Software:
	Totem
	Python with Avahi, GObject and DBUS bindings
	Working Avahi stack (http://avahi.org)

Installation
--------------------------------------------------------------------------------

To install the plugin simply symlink the source directory into your Totem's
plugin directory.

<pre>
cd ~ && git clone https://github.com/wheelcomplex/totem-plugin-airplay.git

mkdir -p ~/.local/share/totem/plugins/ && ln -s ~/totem-plugin-airplay ~/.local/share/totem/plugins/airplay/
</pre>

Then restart Totem and activate the plugin. Obviously Totem must be compiled
with Python support.

python3-avahi for Ubuntu: 
--------------------------
https://launchpad.net/~yavdr/+archive/ubuntu/experimental-main
