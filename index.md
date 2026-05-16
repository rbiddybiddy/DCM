### The Issue

Cars lately have a thing called a DCM (Data Communication Module), that includes a GPS receiver and a cellular modem for sending & receiving data. Data can include "telematics" about the vehicle/driver/environment, as collected from the sensors and GPS; for example, your car's location over time, your speed, braking patterns, lane deviations etc., and in some cases driver-facing cameras and cabin microphones. This has led to a host of privacy and security issues over the years, such as:
- In 2025 Subaru had vulnerabilities allowing anyone to remotely unlock customers' cars, as well as [access the real-time GPS location and location history](https://www.wired.com/story/subaru-location-tracking-vulnerabilities/) of the car.
- Car manufacturers share your driving data with insurance companies, which then [increase your premiums](https://www.nytimes.com/2024/03/11/technology/carmakers-driver-tracking-insurance.html).
- In 2023 Tesla employees internally shared [camera footage of naked customers](https://www.reuters.com/technology/tesla-workers-shared-sensitive-images-recorded-by-customer-cars-2023-04-06/) and other sensitive images.
- In 2015 Charlie Miller and Chris Valasek famously [took over a Jeep Cherokee](https://www.wired.com/2015/07/hackers-remotely-kill-jeep-highway/) with full control of the ignition, brakes, locks, steering, etc.
- Mozilla [detailed how 25 car manufacturers scored abysmally on privacy](https://www.mozillafoundation.org/en/blog/privacy-nightmare-on-wheels-every-car-brand-reviewed-by-mozilla-including-ford-volkswagen-and-toyota-flunks-privacy-test/) and how they collect data including "sexual activity, immigration status, race, facial expressions, weight and genetic information." They sell this data to third parties and use it to build profiles about you covering "intelligence, abilities, characteristics, preferences, and more."
- Tesla had a vulnerability in 2017 that [allowed anyone to remotely see your car’s location](https://electrek.co/2020/08/27/tesla-hack-control-over-entire-fleet/), manage other features, and even summon the car to themselves.
- [The Car That Watches You Back](https://nobodyaskedforthis.lol/posts/connected-car/) details how cars are now serving you ads, as well as collecting vast amounts of data about you.

What's more, the most recently-built cars are moving toward having telemetry & tracking integrated into many disparate systems/locations, probably on purpose to make it harder to remove, sort of like metastatic cancer. But the 2019 Subaru Outback, like others of its era, has these functions pretty centralized in a self-contained DCM unit inside the dash that can be removed relatively easily.

Even better, if the DCM is removed or disabled in a 2019 Outback, no "telematics" data are cached onboard. Some cars, disabling the DCM only prevents real-time tracking; the data collected are still cached for later download by a technician at the dealership. So they still get the data as soon as you go in for repairs, and can sell it to whomever. On the 2019 Outback the only things cached are the things you would actually *want* a mechanic to see - engine diagnostics, that sort of thing.

### To Be Fair...
Having the live data connection does support emergency features such as:
- automatic crash notification
- SOS button (emergency assistance)

...and features associated with a paid Starlink (Subaru's cloud services) subscription such as:
- remote engine start and lock/unlock via smartphone app
- stolen vehicle locator (GPS tracking)
- maintenance alerts
- concierge / roadside assistance integration

Supposedly if you don't have an active Starlink subscription, no data is collected & sent about you, since there's no account (no "you") to associate it with.

### On The Other Hand...
To my mind, that doesn't diminish the value of the data at all, since brokers can easily match it up with your identity by other means. And where data still have value, the same incentives exist for them to capture & collect it.

Plus, even if we take them at their word, that nothing is collected, the policy could change sneakily overnight.

Removing or hard-disabling the DCM brings data collection from the realm of "inactive, we promise" to "literally impossible," and it's easy enough to find parts and instructions online.

### Disabling The DCM: Background
If you don't currently have an active Starlink subscription, the only real tradeoffs (things you have now that you'd be giving up by removing or disabling the DCM) are the two emergency features mentioned above:
- automatic crash notification
- SOS button (emergency assistance)

Worth considering.

A crude way to disable the DCM is to just pull fuse #9. But this also kills the front speakers and the onboard ceiling mic (up there near everybody's heads, for taking calls hands-free on a Bluetooth-paired phone), both of which route through the DCM.

The preferred way is to open up the console, disconnect/remove the DCM and install a DCM bypass, which restores the mic & speaker connections, allows all non-internet functionality including phone pairing (via Android Auto or Apple CarPlay), and doesn't raise diagnostic alarms about a missing DCM or affect driving in any way.

Interesting side story: Subaru itself used to make a DCM bypass kit (DCM Bypass Box, part no. 86229AL400). For 2019 models, Subaru had partnered with AT&T for the cellular connectivity. But when AT&T shut down its 3G network in 2022, Subaru was stuck replacing all the DCMs, because the existing ones would search and search forever for a connection to a 3G network that no longer existed, and eventually drain the battery. There initially wasn't enough inventory to replace them all, so they offered a bypass kit if you weren't an active Starlink subscriber. (Undoubtedly some customers also pulled fuse #9 as a short-term measure during this time too, and accepted the temporary loss of the speakers & mic.) Inventory has since caught up, and Subaru no longer provides the kit, instead instructing dealerships to replace the DCM with a new one. See [Subaru Technical Service Bulletin 15‑318‑24R](Subaru%20DCM%20bypass%20-%20service%20bulletin%2015-318-24R.pdf)


### Disabling the DCM: Instructions
The above-linked Technical Service Bulletin includes disassembly & replacement instructions and drawings.

Since Subaru no longer supplies the DCM bypass, you have to go aftermarket for these now. Here's one from a company that seems to have a good reputation: [https://www.autoharnesshouse.com/69018.html](https://www.autoharnesshouse.com/69018.html) That page also includes links to instructional videos. Should be enough to get the job done.

Keep the DCM unit around in case you later sell the car. You can either offer the car as-is and highlight its inherent data privacy as a selling point, or offer to reinstall the DCM if the buyer so chooses.