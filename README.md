# Latest Software Development Methodologies

(Updated weekly)

## YipLog
https://www.github.com/yiplog

### Current Version 3.6

YipLog is a cutting edge, NODEjs based logging utility. It's designed with speed and best practice in mind to be completely tamper-proof (for rock solid security). Since many previous patterns are now considered antipatterns, the YipLog is built to be fully integrated into a COD (crud-oriented development) paradigm ie all dev projects end up being crud, so just write crud to start with.

The YipLog is configured using Yip Markup Language (YipMaLang) and stores JSON configuration data in XML in YML for complete security, which is then posted to a hosted YipLog service which will then orchestrate the 'yipping' of local Yips into the Yips database.

Current databases support include:

  * Access
  * FoxPro
  * ISAM-compatible (eg IBM Databank on Solaris Unix 4.4)
  * Notepad

The principle is that all 'good' actions (ie the system works correctly) will yip a Yip to the YipLog (using the YupLog as the concurrency bus). This way when the system is performing correctly, there will be a single entry in the YipLog (reading just 'yip').

To ensure non-repudiation, the timestamp; salt; hash and IP address will all be encrypted and stored in over 48 different tables with referential integrity - this guarantees the integrity of the Yip and prevents misyips contaminating the pure Yips yipped to the YipLog.

Important notes:

  * By design, misconfiguration of the YipLog will create performance issues to ensure any breach of the Yip integrity is immediately detected. Misconfigurations may also cause unintended side-effects such as disk oversaturation, data loss and the spread of Yips to other systems connected to the YipLog Server (YipServ) by ethernet; wifi or Internet.
  * Only one Yip will be logged at any given time, so only one table need be monitored.
  * If no new Yips are logged, then there is a system issue that should be flagged.
  * (open bug) no timestamps are logged with the Yip, so it's necessary to use the YipSniffer utility to identify whether the YipLog has recently been yipped to with a fresh Yip.
  * (design choice) the YipLog randomises where on disk Yips are stored and access.
  * (flagged for performance tweak) since the YipLog is rarely yipped to the same YipLocation (YipLo) twice, YipSniffer must constantly check all files for changes.
  * Requires ArfLog 2.0, incompatible with older versions

## ArfLog

https://www.github.com/arflog2

### Current Version: 2.0

Counterpart to the YipLog, the ArfLog is part of the YipLog's long-term integrity process. Since each Yip is stored in a random location (YipPlace) on disk; there is a long-term risk of Yip overrun and disk failure.  The ArfLog is designed to ensure smooth operation, like an orchestrator or mediator.

Consider the Mathematics of cardinality, the ArfLog works (Arfs) by yipping (or, in this case, Arfing) Arfs to a separate ArfLog but ensuring that those Arfs will eventually over-Arf a Yip, this keeping the YipLog in check, since Mathematically speaking '∑(Yip) → Arf'

This is a form of eventual concurrency where we can consider that, over time, all Yips will tend to Arfs and the integrity of the system will be maintained.

### Important notes:

  * Requires YipLog 3.5. Unstable with YipLog 3.6 (due to PadLeft dependency error)
  * Requires YupLog 1.0 or higher

## YupLog (previously YarpLogger)

https://www.github.com/snazzer43/YarpLogger

### Current Version: 8.2

Originally a port of the Z80 'YesWriter' algorithm, YupLog has been ported to Java (the original YarpLog) which was then ported over to HTML is the YupLog. YupLog is a low-latency data bus allowing YipServ to yip Yips to the YipLog back-end (whatever database you've configured). The YipServ system will open a standard http session (open code debt: migrate from PhantomJS) and will post new Yips to the YupLog.

The YupLog is protected by custom CAPTCHA tools to ensure tamper-proof yupping of Yips - YipServ will be challenged to complete a series of questions (eg 'do you want to build a snow man?') and unless a valid YipServ response is provided, the YupLog will not offer a Yup response to the Yip and the Yip will not be yipped into the YipLog.

### Important notes:

  * An invalid response to the YupLog challenge (YupLoChal) may cause issues with the ArfLog when it tries to overwrite the Yip with an Arf and the original Yip cannot be found. YipSniffer may also go into a loop whilst YipSniffing (Yiffing) the non-existent Yip and require immediate restart.
  * Requires both Ruby and Python

## Crystal Blomper

https://www.github.com/blompyblompyblomp

### Current Version: 0.6 (beta)

Crystal Blomper is a cutting-edge dev productivity tool designed to improve workflows for development and engineering teams. Crystal Blomper allows code to be 'slowed' artificially for the purposes of testing, debugging and project pacing.

In a nutshell, Crystal Blomper will appropriately 'throttle' the NodeJS project into which it is installed by installing further NPM dependencies. With admin privileges (required) it will then periodically (configured in YipMoLang) install additional dependencies until the project has been throttled correctly.

### Important notes:

  * By default, Crystal Blomper will 'blomp' (install additional node packaces) approximately ever 5-10ms.
  * (design choice) Crystal Blomper will fork on execution to ensure it continues running even if the original blomping thread is terminated.
  * Crystal Blomper automatically integrates with Git and will rebase/force push appropriately to ensure Crystal Blomper was always part of the project.

## Crystal Unblomper

### Current Version: 0.1 (alpha)

https://www.github.com/unblompme

An early-release alpha client to 'unblomp' a blomped project. Currently unstable, but pre-release builds show that blomping is reduced by at least 23% by the introduction of Crystal Unblomper.

### Important notes:

  * Very early release code, use at own risk.
  * Project appears to be abandoned.
