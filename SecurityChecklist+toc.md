# Security Checklist

-   [Checklist Instructions](#checklist-instructions)
-   [Secure Your Devices](#secure-your-devices)
    -   [Consider Using a Chromebook or
        iPad](#consider-using-a-chromebook-or-ipad)
    -   [Laptop Disk Encryption](#laptop-disk-encryption)
    -   [Web Encryption](#web-encryption)
    -   [Secure your Mobile Phone
        Account](#secure-your-mobile-phone-account)
-   [Secure your Accounts](#secure-your-accounts)
    -   [Passwords](#passwords)
    -   [Password managers](#password-managers)
    -   [Two-factor authentication](#two-factor-authentication)
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
-   [Travel Guidelines](#travel-guidelines)
    -   [Physically Secure your Digital
        Assets](#physically-secure-your-digital-assets)
    -   [Travel to High Risk Countries](#travel-to-high-risk-countries)
-   [More Information](#more-information)
-   [Credits](#credits)

An up-to-date digital copy available:
https://github.com/bdwilson/security-checklist

Checklist Instructions
======================

Use this checklist to make sure you have reviewed all the device and
account security basics, starting with your personal digital life. Print
out the document and check off the boxes. These recommendations are
based on a threat model of a regular employee or US citizen -- if you
are an executive or have a reason to be targeted, then additional
protections may apply.

Secure Your Devices
===================

Keeping your laptops, phones, tablets, and "smart devices" as well as
the applications on them, updated is one of the most important ways to
keep them (and your data) secure. For example, most operating system
updates contain numerous security updates. Attackers frequently take
advantage of devices and software that have not been updated. Always
apply your updates as soon as they come out, better yet, set them to
auto-install. If you're running Windows, make sure it's a supported
version and that Windows Defender is enabled.

Consider Using a Chromebook or iPad
-----------------------------------

A key technique for reducing the risk of a breach is to reduce your
attack surface. To that end, consider migrating your personal computing
device to a Chromebook or an iPad. Both devices offer several key
security features, which dramatically limit the options attackers have
for running malware.

Laptop Disk Encryption
----------------------

Encrypting your laptop can keep your data safe even when it is lost or
stolen. Disk encryption is easy to enable and does not take much time.
Here are the instructions: for
[Macs](https://support.apple.com/en-us/HT204837) and for
[PCs](https://www.windowscentral.com/how-use-bitlocker-encryption-windows-10).
If you're using a Chromebook, your data is
[encrypted](https://support.google.com/chromebook/answer/3438631) in the
cloud.

Web Encryption
--------------

Some websites do not properly enable encryption for all connections.
Luckily, there is something you can do to make sure your internet
connections are secure. In your web browser, you should install the
[HTTPS Everywhere](https://www.eff.org/https-everywhere) extension.
HTTPS Everywhere is a Firefox, Chrome, and Opera extension that
strengthens the encryption between your device and major websites. Most
reputable services use secure connections by default. Look for the LOCK
icon and stay away from sites labeled as insecure. You may hear people
mention personal VPN accounts as a way to protect your web traffic;
however, you have no control over what path that data travels or what
the provider does with the data. HTTPS and Secure Websites offer similar
protections without cost.

Secure your Mobile Phone Account
--------------------------------

Most phone carriers allow you to set a login PIN that is required in
order to make changes to your account. If your carrier supports this
feature, you should enable it because having a PIN makes it harder for
attackers to take over your account ("called SIM-swap attacks"), and
anything protected by your phone number or linked to SMS. Even if they
guess your name and password, they will still need your PIN to access
and make changes to your account.

Secure your Accounts
====================

Passwords
---------

For every one of your online accounts, you should use a password that is
**long**, **random**, and **unique**. Here is our current thinking: -
**Long**: at least 15 characters - **Random**: generated by a computer,
not you. Humans are not wired to generate random data. - **Unique**:
never used twice. Attackers take advantage of password reuse, so don't
do it.

The beauty of using different passwords for different accounts is that
should one provider become compromised, resulting in exposed passwords,
that same password cannot be used to gain access to other accounts. Most
individuals have dozens of online accounts, so unless you have a
photographic memory, organizing passwords with the above requirements is
a tall order. The solution is to use a password manager, which can be
intimidating; however, integrations with mobile devices and browsers
have made for a less disruptive user experience.

Password managers
-----------------

Password managers such as [1Password](https://1password.com/) and
[LastPass](https://lastpass.com/) help you create, store and enter login
credentials for you from within your browser or mobile device. They will
create passwords that are long, random, and unique. They will store
them, in encrypted form, in a database in the cloud. When logging into a
website, they can enter your username and password in the correct field
for the correct site, so you don't need to type them -- this comes in
handy if you're following a link from an email message and it's asking
for you to login. If the site has an entry in your password manager,
then you can feel better about the site being legitimate.

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
this [passphrase
generator.](https://www.fourmilab.ch/javascrypt/pass_phrase.html) A good
passphrase might look something like this: pigfish relay fusion cheesy
whisk impunity

This is not an exhaustive list of password managers, there are many
others available. Please make sure you look at how the products manage
and react to security issues before you select a product.

Two-factor authentication
-------------------------

**Two-factor** authentication (sometimes called 2FA, "two-step",
"multi-factor", MFA, or OTP-One Time Passcodes) adds an additional and
critical step to a website's login process. 2FA systems either use your
smartphone or a hardware device/token to identify you to the website.
Visit [twofactorauth.org](https://twofactorauth.org/) for instructions
on how to enable this for various sites and services -- specific
instructions for Google, Microsoft, and Apple are below. If your
critical providers like finance and banking do not offer 2FA, you should
encourage them to add it or look for another provider that offers more
advanced security features.

Some providers use "token applications" to manage your credentials. [OTP
Auth](https://itunes.apple.com/us/app/otp-auth/id659877384?mt=8) (iOS)
and [TOPT Authenticator](https://www.binaryboot.com/totp-authenticator)
(Android) are reputable token applications that support standards-based
One Time Passcode tokens compatible with most sites. These apps, unlike
Google Authenticator, support encrypted backups -- otherwise, you may
have to re-enroll with 2FA at each site should you upgrade your device!

**Caution**: Many websites offer SMS-based (text message) two-factor
access. Unfortunately, it is possible to steal someone's phone number
(remember "SIM-swap attacks"?), and then to intercept two-factor codes
sent via SMS. For most, SMS-based 2FA is better than no 2FA at all;
however, the other options provide more security. Note that you may have
more than one account on these services. Protect them all

Email Services
==============

For most individuals, we strongly recommend using personal mail services
hosted by either Microsoft (Outlook/Live/O365), Google (Gmail/G Suite),
or Apple (iCloud). While there are other free or ISP-provided services
that might sound attractive, none of them match the security programs
and teams at Microsoft, Google, or Apple. Maintaining and securing email
services is a difficult job, so leave it to the experts.

Google Account Security
-----------------------

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

Outlook/Live Account Security
-----------------------------

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

Apple Account Security
----------------------

If you use Apple devices, you should
[enable](https://support.apple.com/en-us/HT204915) their Two-Factor
Authentication option. This can be done from your iOS device via:

1.  Go to Settings &gt; \[your name\] &gt; Password & Security

2.  Tap "Turn On" Two-Factor Authentication

3.  Tap "Continue"

Social, Privacy, and Identity
=============================

Verify, then Trust
------------------

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

Important Online Accounts to Claim
----------------------------------

Below are a few common accounts which individuals should *pre-claim* so
that they can maintain their identity with the providers.

  **Account**   **Purpose**                   **Why this is important**                                                                                                                                                                                                                                                                **Actions to take**
  ------------- ----------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- ---------------------------------------------------------------------------------------------
  IRS.gov       IRS online services account   Identity theft prevention; as well as protecting your IRS account from someone else registering (and potentially submitting a tax return as you)                                                                                                                                         Use a strong and unique password (stored in your password manager of choice) and enable 2FA
  SSA.gov       my Social Security            Identity theft prevention; as well as protecting your Social Security account from someone else registering (and potentially claiming your social security benefits)                                                                                                                     Use a strong and unique password (stored in your password manager of choice) and enable 2FA
  USPS.com      Informed Delivery             Sign up for Informed Delivery - to see what is coming in your mailbox; otherwise someone else could setup this account and would know if something sensitive is waiting in your mailbox or they could perform mail forwarding without your knowledge (helps to prevent identity theft)   Use a strong and unique password (stored in your password manager of choice) and enable 2FA

Social Media Privacy Settings
-----------------------------

Facebook is one of the most notable social media providers but also
collects the most information about it's users. They have recently given
users more control over their privacy settings and those can be
[reviewed here](https://www.facebook.com/settings?tab=privacy). Consumer
Reports has produced a [guide to help you tune the
settings.](https://www.consumerreports.org/privacy/facebook-privacy-settings/)
Instagram, Twitter and Snapchat privacy settings [should also be
reviewed](mailto:http://www.respectteam.com/blog/social-media-privacy-facebook-instagram-twitter-and-snapchat/),
especially if you have children using these services.

Security Questions
------------------

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

Freezing your Credit
--------------------

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
You can also keep tabs on your credit for free by using either Credit
Karma and/or Turbo (by Intuit) who offer apps that provide this service
in hopes that you'll take advantage of their credit offers.

Travel Guidelines
=================

Physically Secure your Digital Assets
-------------------------------------

Resist the urge to leave computing devices in your checked luggage or
leave your devices unattended. Keep your devices on you or with someone
you trust. If a physical lock or safe is available, use it. If you must
leave your devices in your car, lock them where they cannot be seen (in
the trunk or under the seat).

Travel to High Risk Countries
-----------------------------

If you're traveling for business to a high-risk country, it is advised
you do not take your primary machine or primary phone device with you.
Removing sensitive data from a system before travel is advised.
Re-installing your system after a trip, or using a device as mentioned
above like a Chromebook or iPad - which limits many attack vectors,
compared to a typical laptop.

More Information
================

The information above is general guidance that will dramatically reduce
the risk of attackers compromising your devices and accounts. But, given
the daily news about security problems, it will come as no surprise that
these practices will not be sufficient in all cases.

Credits
=======

[Bob
Lord](https://medium.com/@boblord/device-and-account-security-checklist-2-0-1f3637eec1c)