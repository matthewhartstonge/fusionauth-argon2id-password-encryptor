# fusionauth-argon2id-password-encryptor

This plugin provides a pure Java implementation for generating argon2id password
digests in FusionAuth.

## Java Install
To install Java, you will need the OpenJDK. Due to licensing, you can't simply
use the Oracle JDK distribution due to 'commercial use'.

Hop over to [Adoptium](https://adoptium.net/?variant=openjdk11) to download the
OpenJDK for your platform.

## Building

This project uses Maven, so to build the required JAR file, you need to run:

```bash
$ mvn package
```

This will spit out a "shaded" uber JAR, that is a JAR file packaged with all 
required dependencies packed into a single JAR file.

## Deployment
### FusionAuth Cloud
The required JAR file need to be sent on to the FusionAuth's support team via 
email or via a support ticket, so they can plug it directly into the specific 
cloud deployment.

### FusionAuth
Take the shaded JAR and copy/paste/add it into FusionAuth's `plugin` folder.
