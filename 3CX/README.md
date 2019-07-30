# Using Voxbone with 3CX

It's easy to connect numbers from your Voxbone account to the 3CX platform, and enjoy both inbound and outbound calling services with a simple configuration.

What you'll need to get started:

1. A registered Voxbone account with assigned numbers. (Create your account [here](https://www.voxbone.com/trial-choose))
2. A working deployment of 3CX (Create it [here](https://www.voxbone.com/trial-choose))

Note: On both platforms, a free-trial account is enough to get started!

# Import VoIP Provider settings for Voxbone
You can easily import an XML file containing all the configuration options explained in detail below. With this option, you can simply import, add in your credentials and good to go! To do so,
1. Log in to your 3CX console
2. Go to “SIP Trunks” view via the side navigation
3. Click “Import Provider”
4. Upload the 3CX provider XML file in this repo : voxbone-3cx-provider.xml
5. Add your SIP Digest credentials
6. Set inbound routing by “Route calls to” section on “General” tab
7. Create at least one Outbound Rule that uses the newly configured trunk

# Setup authentication for outbound calling
Here’s how you can configure authentication on your Voxbone trunk :
1. For either authentication option, select “Do not require - IP Based” for “Type of Authentication”
2. Recommended authentication method for outbound calls on Voxbone platform is SIP Digest. Enter your digest username and password generated from Voxbone portal. This can be done by logging in to the portal and generation of new credentials on Configure > Configure Outbound Voice
![Setup SIP Authentication for Outbound Calls on 3CX VoIP Provider Settings](http://live-voxbonecom.pantheonsite.io/wp-content/uploads/2019/07/Screenshot-2019-07-15-at-13.47.03.png)
