# Device and Account Security Checklist
AKA: Security for the rest of us.

-   [Checklist Instructions](#checklist-instructions)
-   [Secure Your Devices](#secure-your-devices)
    -   [Network Security](#network-security)
    -   [Consider Using a Chromebook or
        iPad](#consider-using-a-chromebook-or-ipad)
    -   [Laptop Disk Encryption](#laptop-disk-encryption)
    -   [Web Security](#web-security)
        - [DNS Security](#dns-security)
        - [VPN - Provider/Subscription](#vpn---providersubscription)
        - [VPN - Personal](#vpn---personal)
    -   [Secure your Mobile Phone
        Account](#secure-your-mobile-phone-account)
-   [Secure your Accounts](#secure-your-accounts)
    -   [Passwords](#passwords)
    -   [Password Managers](#password-managers)
    -   [Account Monitoring](#account-monitoring)
    -   [Two-factor Authentication](#two-factor-authentication)
        -   [SMS-based 2FA (ok; better than
            nothing)](#sms-based-2fa-ok-better-than-nothing)
        -   [Email-based 2FA (better than
            nothing)](#email-based-2fa-better-than-nothing)
        -   [Push-based 2FA Approvals (better - with
            awareness)](#push-based-2fa-approvals-better---with-awareness)
        -   [Token Application based 2FA
            (better)](#token-application-based-2fa-better)
        -   [Hardware Token based 2FA
            (best)](#hardware-token-based-2fa-best)
-   [Email Services](#email-services)
    -   [Google Account Security](#google-account-security)
    -   [Outlook/Live Account Security](#outlooklive-account-security)
    -   [Apple Account Security](#apple-account-security)
-   [Social, Privacy, and Identity](#social-privacy-and-identity)
    -   [Verify, then Trust](#verify-then-trust)
    -   [Important Online Accounts to
        Claim](#important-online-accounts-to-claim)
    -   [Social Media Privacy Settings](#social-media-privacy-settings)
    -   [Security Questions](#security-questions)
    -   [Freezing your Credit](#freezing-your-credit)
-   [Credit Card Safety](#credit-card-safety)
    -   [Reducing Credit Card Fraud](#reducing-credit-card-fraud)
    -   [Monitoring your Credit Cards](#monitoring-your-credit-cards)
-   [Travel Guidelines](#travel-guidelines)
    -   [Physically Secure your Digital
        Assets](#physically-secure-your-digital-assets)
    -   [Travel to High Risk Countries](#travel-to-high-risk-countries)
-   [More Information](#more-information)
-   [Credits](#credits)

An up-to-date digital copy with links is available here:
https://github.com/bdwilson/security-checklist

# Checklist Instructions

Your security awareness at home directly effets your security awareness at work, so
highlighting ways you can help secure your home life will drive employees to be
more secure at work.  Use this checklist to make sure you have reviewed all the device and
account security basics, revolving around your personal digital life. 
Print out the document and check off each item. These recommendations are
based on a threat model of a regular employee or US citizen -- if you are
an executive or have a reason to be targeted, then additional
protections may apply.

# Secure Your Devices
Keeping your laptops, phones, tablets, and "smart devices" as well as
the applications on them, updated is one of the most important ways to
keep them (and your data) secure. For example, most operating system
updates contain numerous security updates. Attackers frequently take
advantage of devices and software that have not been updated. Always
apply your updates as soon as they come out, better yet, set them to
auto-install. If you're running Windows, make sure it's a supported
version and that Windows Defender is enabled (yes, you can still update
systems from [Windows 8 to Windows 10 for free](https://www.zdnet.com/article/heres-how-you-can-still-get-a-free-windows-10-upgrade/). 

## Network Security 
Keeping your devices up-to-date also includes your router and wireless access points. These types of devices frequently have firmware updates that introduce new features as well as fix security bugs. You should check for updates at least yearly on these devices. It's also important to configure your router to to not allow Internet traffic with access to the services **inside** your network - by default, your router should be configured in this manner. You can [check your firewall](https://routersecurity.org/testrouter.php#FirewallTesters) using any number of online-tools (the Shodan.io and Censys.io links here are two good ones to start with). It's also crucial that you keep your wireless network devices secured with at least WPA2-AES PSK. Some routers offer an optional MAC address filtering capability, however this feature doesn't add any real security as an attacker can wirelessly _snoop_ in order to determine which MAC addresses can join that network, and then _spoof_ a valid MAC address. 

## Consider Using a Chromebook or iPad
A key technique for reducing the risk of a breach is to reduce your
attack surface. To that end, consider migrating your personal computing
device to a Chromebook or an iPad. Both devices offer several key
security features, which dramatically limit the options attackers have
for running malware.

## Laptop Disk Encryption
Encrypting your laptop can keep your data safe even when it is lost or
stolen. Disk encryption is easy to enable and does not take much time.
Here are the instructions: for [Macs](https://support.apple.com/en-us/HT204837) and for
[PCs](https://www.windowscentral.com/how-use-bitlocker-encryption-windows-10).
If you're using a Chromebook, your data is
[encrypted](https://support.google.com/chromebook/answer/3438631) in the
cloud.

## Web Security
Some websites do not properly enable encryption for all connections.
Luckily, there is something you can do to make sure your internet
connections are secure. In your web browser, you can install the
[HTTPS Everywhere](https://www.eff.org/https-everywhere) extension.
HTTPS Everywhere is a Firefox, Chrome, and Opera extension that
strengthens the encryption between your device and major websites. Most
reputable services use secure connections by default. Look for the LOCK
icon and stay away from sites labeled as
insecure. You may hear people mention personal VPN accounts as a way to
protect your web traffic, but that's not always the case ([see below](#vpn---providersubscription)). Websites 
delivered by HTTPS offer similar protections without cost, thus VPN subscriptions are rarely needed. Below are some more advanced methods of helping improve your overall security and privacy when browsing the web at home.

### DNS Security
**Warning, this an advanced stuff. Most people can skip this.**
Some may wish to block additional content, or apply security controls to all 
systems within their home network. One such way to accomplish this is by altering
your DNS configurations on your router. DNS stands for Domain Name Services and it's
the global system for mapping a name (www.google.com) to an IP address (8.8.8.8). By using 
a DNS server different than the one provided by your ISP, you can alter the ability for
systems on your network to _resolve_ certain names, thus limiting the ability for individuals
on your network to access any site since you control what names get resolved. 

As far as content blocking, applying security, or privacy controls to the web traffic at your home, 
you should review the options [outlined here](https://danielmiessler.com/blog/dns-servers-you-should-have-memorized/) to
see what options are right for you and your home. Another more turn-key option is to use a service like [NextDNS](https://nextdns.io/) that
provides personalized DNS filters catered to your needs, and allows you to have different profiles depending on if your need is
security-related, or goal is to limit content from others in your home.  If your goal is to block adverstisements - and thus limit ad tracking - then [PiHole](https://pi-hole.net/) is a more advanced option to give you similar results as NextDNS, but at home.

### VPN - Provider/Subscription 
**Warning, this an advanced stuff. Most people can skip this.**
VPN stands for virtual private networking - this is technology that allows you
to tunnel network traffic so that it enters and exists via another location. Think
of it like a tunnel going under a treacherous war zone - you can pass without being
subjected to any of the threats within that zone. A VPN provider provides you a with a
similiar connection allowing you to _securely_ send all your traffic through that connection, 
thus limiting your Internet Service Providers' ability to snoop on the traffic. The issue is that
you have no control over what path that data travels after it leaves your VPN provider, nor
can you control or validate what the VPN provider does with the data they __do__ know about you.

One area where one might want to leverage VPN Provider might be in a situation where
they would rather not disclose their home/Internet location.  When you 
access a website from home, it discloses your home IP address to the server serving the
web traffic. If the server you're accessing is controlled by an attacker, you've just
disclosed your location to an attacker. One such scenario might involve an 
attacker who sent you a Phishing email with an embedded image or link. 
Clicking on the link or viewing the image could disclose to an attacker 
where you are coming from and provide that attacker with additional 
information about you - perhaps if you're running services from your network 
connection? One way around this without leveraging a paid VPN Provider might be to only
open overly-suspecious links from a mobile phone connected to the cellular provider network
(not on your home Wifi network). 

The marketing budgets for VPN Providers is huge, so you will see lots of articles and recommendations
made about various providers with referral kick-backs. If you insist on protecting your home Internet
browsing with a VPN, we'd recommend you run your own in the cloud ([see below](#vpn---personal).

### VPN - Personal 
**Warning, this an advanced stuff. Most people can skip this.**
If you're concerned about securing your network traffic on-the-go, you could run your own
VPN server at home. Some individuals also run their own VPN server with a cloud service provider.
This is not for the faint of heart, however there are many options available: [PiVPN](https://www.pivpn.io/), [Replace your VPN Provider with Wireguard at a Cloud Provider](https://medium.com/@drew2a/replace-your-vpn-provider-by-setting-up-wireguard-on-digitalocean-6954c9279b17). Some home routers also feature VPN capablities, so you can check to see if your router supports this feature. Opening up your home network to run a VPN server could introduce some risks, so make sure you understand the implications before going out on your own. 

## Secure your Mobile Phone Account
Most phone carriers allow you to set a login PIN that is required in
order to make changes to your account. If your carrier supports this
feature, you should enable it because having a PIN makes it harder for
attackers to take over your account ("called SIM-swap attacks"), and
anything protected by your phone number or linked to SMS. Even if they
guess your name and password, they will still need your PIN to access
and make changes to your account.

# Secure your Accounts
## Passwords 
For every one of your online accounts, you should use a password that is
**long**, **random**, and **unique**. Here is our current
thinking:
-   **Long**: at least 16 characters
-   **Random**: generated by a computer, not you. Humans are not wired
    to generate random data.
-   **Unique**: never used twice. Attackers take advantage of password
    reuse, so don't do it.

The beauty of using different passwords for different accounts is that
should one provider become compromised, resulting in exposed passwords,
that same password cannot be used to gain access to other accounts. Most
individuals have dozens of online accounts, so unless you have a
photographic memory, organizing passwords with the above requirements is
a tall order. The solution is to use a password manager, which can be
intimidating; however, integrations with mobile devices and browsers
have made for a less disruptive user experience. 

## Password Managers 
Password managers such as [1Password](https://1password.com/) and
[LastPass](https://lastpass.com/) help you create, store and enter
login credentials for you from within your browser or mobile device.
They will create passwords that are long, random, and unique. They will
store them, in encrypted form, in a database in the cloud. When logging
into a website, they can enter your username and password in the correct
field for the correct site, so you don't need to type them -- this comes
in handy if you're following a link from an email message and it's
asking for you to login. If the site has an entry in your password
manager, then you can feel better about the site being legitimate.

The password manager you choose will both help generate and store your
website passwords. To protect all those individual website passwords,
you need to supply a "master password". The password manager will use
that master password to encrypt/decrypt all your individual website
passwords. Mobile devices have built-in integrations to allow you to use
biometrics (fingerprint or facial recognition) to limit how often your
master password will need to be entered -- it's easy when you get the
hang of it.

**Caution**: If someone obtains or guesses your master password, they
may be able to decrypt all your individual passwords. The master
password must be long and unique, but also memorable. You will type it
every day, many times a day.

To create a strong master password, use a password generator such as
this [passphrase generator.](https://www.fourmilab.ch/javascrypt/pass_phrase.html) A
good passphrase might look something like this: pigfish relay fusion
cheesy whisk impunity

This is not an exhaustive list of password managers, there are many others
available. Please make sure you look at how the products manage and react to
security issues before you select a product.

## Account Monitoring
Ever wonder if any of your online accounts have been compromised? You can use
[HaveIBeenPwned](https://haveibeenpwned.com) to lookup your email address to determine 
if your address - and potentially your password - was discovered in any online breaches.
Some password managers, specifically 1Password, also integrate with HIBP to give you a 
visual indicator of accounts and passwords that have shown up in breaches and thus should be changed. 

## Two-factor Authentication 
**Two-factor** authentication (sometimes called 2FA, "two-step",
"multi-factor", MFA, or OTP-One Time Passcodes) adds an additional and
critical step to a website's login process. 2FA systems either use your smartphone or a hardware
device/token to identify you to the website. Visit
[twofactorauth.org](https://twofactorauth.org/) for instructions on
how to enable this for various sites and services -- specific
instructions for Google, Microsoft, and Apple are below. If your
critical providers like finance and banking do not offer 2FA, you should
encourage them to add it or look for another provider that offers more
advanced security features. Note that you may have more than one account with
each provider, you'll want to protect them all.

### SMS-based 2FA (ok; better than nothing)
**Caution**: Many websites offer SMS-based (text message) two-factor
access. Unfortunately, it is possible to steal someone's phone number
(remember "[SIM-swap attacks](#secure-your-mobile-phone-account)"?), and then to intercept two-factor codes
sent via SMS. For most, SMS-based 2FA is better than no 2FA at all;
however, the other options below provide more security. 

### Email-based 2FA (better than nothing)
Some providers offer email-based 2FA where they will email you a token in order
to require you to login. This is good assuming you know your email has not been
compromised, being forwarded somewhere or some random application has access to
it. This may be better than SMS-based protection because taking over someone's
phone account is probably easier than gaining access to their email. Keep
looking at the other options. 

### Push-based 2FA Approvals (better - with awareness)
Some providers ([Symantec
VIP](https://vip.symantec.com),
[Duo](https://duo.com/product/multi-factor-authentication-mfa/authentication-methods/duo-push)
and [Microsoft
Authenticator](https://www.microsoft.com/en-us/account/authenticator)) offer
their own applications that use a real-time push message sent to your mobile
device for you to approve. This is a convenient method for the end-user,
however users **must make sure they only approve messages they initiated**. If
you receive a push message that was not initiated from you, you should take
action to immediately change your password on the impacted accounts.

### Token Application based 2FA (better)
Some providers use "token applications" to manage your credentials. [OTP
Auth](https://itunes.apple.com/us/app/otp-auth/id659877384?mt=8) (iOS)
and [TOPT Authenticator](https://www.binaryboot.com/totp-authenticator)
(Android) are reputable token applications that support standards-based
One Time Passcode tokens compatible with most sites. These apps, unlike
the Google Authenticator app, support encrypted backups (and restores to new
drvice) -- otherwise, you may have to re-enroll with 2FA at each site should you upgrade your device!

### Hardware Token based 2FA (best) 
Hardware-based security keys are the most secure method to choose, but also
comes with more hoops that a user must jump through to make them work. If you
are serious about keeping your accounts secure, a
[Yubico](https://www.yubico.com/product/security-key-nfc-by-yubico) or [Titan Security
Key](https://cloud.google.com/titan-security-key/) is the way to go. Not all
providers accept physical security keys, plus you may have mobile device
limitations that may prevent all types of keys from working with your device.
It is also advised if you use hardware-based tokens, that you review any other
authentication methods on your account (like SMS) and remove the less-secure
options from your account, otherwise an attacker could get around your hardware
key and your use of it to be more secure would be moot.

# Email Services
For most individuals, we strongly recommend using personal mail services
hosted by either Microsoft (Outlook/Live/O365), Google (Gmail/G Suite),
or Apple (iCloud). While there are other free or ISP-provided services
that might sound attractive, none of them match the security programs
and teams at Microsoft, Google, or Apple. Maintaining and securing email
services is a difficult job, so leave it to the experts.

## Google Account Security
If you use Gmail for personal email, you should get a security checkup.
Go to <https://myaccount.google.com/security-checkup>. Click on each of
the four rows, starting with "Your Devices." A few points:

1.  Under "Your Devices", make sure only devices you use on a regular
    basis are present. Remove others.

2.  Under "Recent Security Events", make sure it says "No events in 28
    days".

3.  Under "2-Step Verification," remove any devices you do not use
    anymore. Use this opportunity to enroll in the 2-Step Verification
    using one of the OTP apps from above.

4.  Under "Third-party access" (if present), remove access from any apps
    you do not use or recognize.

## Outlook/Live Account Security
If you use Outlook/Live for personal email, you can also review your
sign-ins and should enroll in their Two-Step Verification program via
<https://account.microsoft.com/security/>. To do this:

1.  Select + Signin Activity and look for Successful Signins. If you
    have unsuccessful signins, this is even more of a reason to enable
    Two-Step Verification.

2.  Go back and Select + More Security Options

3.  Turn on Two-Step Verification

4.  Set up the Identity Verification App by either downloading the
    Microsoft Authenticator App or using an OTP app discussed earlier.

## Apple Account Security
If you use Apple devices, you should
[enable](https://support.apple.com/en-us/HT204915) their Two-Factor
Authentication option. This can be done from your iOS device via:

1.  Go to Settings \> \[your name\] \> Password & Security

2.  Tap "Turn On" Two-Factor Authentication

3.  Tap "Continue"

# Social, Privacy, and Identity

## Verify, then Trust
Attacks come in many shapes and sizes, but one of the most unpredictable
attacks revolves around human trust. These social engineering attacks
often originate in the form of a phone call, text message, or email;
however, they also happen in our everyday interactions. Be diligent
about verifying the identity of someone who has urgently asked you to
perform some action. Ask to call the person back using a number you know
from your credit card -- contact the person who is *supposedly* asking
you to transfer money -- verify the identity of the person waiting
outside your building before letting them in. Don't let yourself become
the vulnerability!

## Important Online Accounts to Claim
Below are a few common accounts which individuals should *pre-claim* so
that you can maintain your identity with these providers. 

| **Account** |  **Purpose** | **Why this is important** | **Actions to take**|
| ---- | ---- | ---- | ---- |
|  [IRS.gov](https://www.irs.gov/payments/view-your-tax-account) | IRS online services account |  Identity theft prevention; as well as protecting your IRS account from someone else registering (and potentially submitting a tax return as you) | Requires access to a loan or credit card account + a mobile phone number registered to your name. Use a strong and unique password (stored in your password manager of choice) and enable 2FA|
| [login.gov](https://login.gov/) | login.gov | The long-term goal of login.gov is to be the centralized authentication provider for most US Federal websites. | Use a strong and unique password (stored in your password manager of choice) and enable 2FA|
| [SSA.gov](https://www.ssa.gov/site/signin/en/) | my Social Security | Identity theft prevention; as well as protecting your Social Security account from someone else registering (and potentially claiming your social security benefits) | Requires credit validation via Equifax, so if your credit is frozen, you will need to temporarily unfreeze to register. Use a strong and unique password (stored in your password manager of choice) and enable 2FA |
| [USPS.com](https://www.usps.com/) | Informed Delivery | Sign up for Informed Delivery - to see what is coming in your mailbox; otherwise someone else could setup this account and would know if something sensitive is waiting in your mailbox or they could perform mail forwarding without your knowledge (helps to prevent identity theft) | Use a strong and unique password (stored in your password manager of choice) and enable 2FA|

## Social Media Privacy Settings
Facebook is one of the most notable social media providers but also
collects the most information about it's users. They have recently given
users more control over their privacy settings and those can be
[reviewed here](https://www.facebook.com/settings?tab=privacy).
Consumer Reports has produced a [guide to help you tune the
settings.](https://www.consumerreports.org/privacy/facebook-privacy-settings/)
Instagram, Twitter and Snapchat privacy settings [should also be
reviewed](mailto:http://www.respectteam.com/blog/social-media-privacy-facebook-instagram-twitter-and-snapchat/),
especially if you have children using these services.

## Security Questions
A few websites still rely on account security questions ("ASQ") to help
identify you in the event you forget your password. They often ask for
information like "Where did you travel on your honeymoon?" While that
might seem like a harmless question, in a world of social media, many of
these answers can be found on the internet or the dark web, or through
other data breaches where this information has been leaked. If you
encounter a website that requires account security questions, consider
using random words or a generated password to answer those questions
rather than using real answers. Use your password manager to store your
random answers in the Notes or Comments section.

## Freezing your Credit
Freezing your credit is a great way to proactively thwart attempts to
steal your identity and open new lines of credit without your
permission. Freezing your credit at the "Big 3" credit reporting
agencies is free and can be done online. You'll use your account and/or
PIN to temporarily unfreeze your credit for a temporary period so you
can enroll in a line of credit or allow your credit to be checked. The
[FTC has a great
guide](https://www.consumer.ftc.gov/blog/2018/09/free-credit-freezes-are-here)
on how to do this for yourself and other family members, however they
fail to include the smaller two agencies that should also be reviewed.
Those may be found
[here](mailto:https://www.nerdwallet.com/blog/finance/pros-and-cons-freezing-credit/).
If you're looking for a detailed document on how to freeze the credit of a
minor, this is detailed
[here](https://brianwilson.us/2019-04-02-Credit-Protections-for-Minors/). 
You can also keep tabs on your credit for free by using either [Credit
Karma](https://www.creditkarma.com/) and/or [Turbo (by
Intuit)](https://turbo.intuit.com/) who offer apps that provide this service
in hopes that you'll take advantage of their credit offers.

# Credit Card Safety

## Reducing Credit Card Fraud
There are many options available to help you fight credit card fraud. The goal in most of these is to keep your real credit card information away from online retailers - by abstracting the payment process using virtual credit cards or a service such as Apple Pay, the online retailer does not have access to your credit card information. 
1. Virtual credit cards is a feature that many providers offer that allow users to create and manage one-time or one-site only credit cards.  [Paypal Key](https://www.paypal.com/myaccount/debitcards/key) is a relatively new funtionality that allows you to create virtual account numbers and link them to your Paypal account credit cards. [CaptialOne](https://www.capitalone.com/applications/eno/) has one such feature called ENO that has a browser plugin to do just this; other providers may offer something similar.  If your credit card provider does not do this, [Privacy.com](https://privacy.com) has a service that will do this for free, however you must link your Debit or Checking account to the service and make payments from it. 
2. Use a payment service vs. providing your credit card directly to a online retailer. These services are a middle man between you and the retailer, thus making it so the retailer does not have access to your original credit card information.

## Monitoring your Credit Cards
Keeping up with the charges on your credit cards used to require you to wait for a monthly statement. 
Now most credit card companies offer individuals the ability to receive notifications when charges
are made to their accounts. These types of nofications range from SMS or email alerts when charges 
greater than X are charged to your account. Other providers may also require you use their smartphone
app to receive these. Check with your credit card provider to find out how you can get the upper hand
on knowing when charges are made against your card. 

# Travel Guidelines

## Physically Secure your Digital Assets
Resist the urge to leave computing devices in your checked luggage or
leave your devices unattended. Keep your devices on you or with someone
you trust. If a physical lock or safe is available, use it. If you must
leave your devices in your car, lock them where they cannot be seen (in
the trunk or under the seat).

## Travel to High Risk Countries
If you're traveling for business to a high-risk country, it is advised
you do not take your primary machine or primary phone device with you.
Purchasing a device specific to travel that doesn't hold any sensitive data is
recommended. If you have to take your primary device, remove any sensitive data
from it prior to travel, and consider re-installing your system after the trip.
Another option would be to use [a device as mentioned
above like a Chromebook or iPad](#consider-using-a-chromebook-or-ipad) which
limits many attack vectors, compared to a typical laptop.

# More Information 
The information above is general guidance that will dramatically reduce
the risk of attackers compromising your devices and accounts. But, given
the daily news about security problems, it will come as no surprise that
these practices will not be sufficient in all cases.

# Credits
[Bob Lord](https://medium.com/@boblord/device-and-account-security-checklist-2-0-1f3637eec1c) for his work on the Device and Account Security checklist that this is based
off of. 
