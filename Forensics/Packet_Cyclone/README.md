# Packet Cyclone

## Description

Pandora's friend and partner, Wade, is the one that leads the investigation into the relic's location. Recently, he noticed some weird traffic coming from his host. That led him to believe that his host was compromised. After a quick investigation, his fear was confirmed. Pandora tries now to see if the attacker caused the suspicious traffic during the exfiltration phase. Pandora believes that the malicious actor used rclone to exfiltrate Wade's research to the cloud. Using the tool called "chainsaw" and the sigma rules provided, can you detect the usage of rclone from the event logs produced by Sysmon? To get the flag, you need to start and connect to the docker service and answer all the questions correctly.

## Solution

First of all I cloned the [chainsaw repository]([https://github.com/WithSecureLabs/chainsaw) and build it.

In this challenge, you are given **evtx-logs** (Windows Event Logs) and a couple of **sigma-rules**.
To run the chainsaw with the given rules:
```bash
```

You have to ```nc``` the given ```address port``` to begin the prompt with the questions.

> What is the email of the attacker used for the exfiltration process? (for example: name@email.com)

* Answer: ```majmeret@protonmail.com```

* Explanation

> What is the password of the attacker used for the exfiltration process? (for example: password123)

* Answer: ```FBMeavdiaFZbWzpMqIVhJCGXZ5XXZI1qsU3EjhoKQw0rEoQqHyI```

* Explanation

> What is the Cloud storage provider used by the attacker? (for example: cloud)

* Answer: ```mega```

* Explanation

> What is the ID of the process used by the attackers to configure their tool? (for example: 1337)

* Answer: ```3820```

* Explanation

> What is the name of the folder the attacker exfiltrated; provide the full path. (for example: C:\Users\user\folder)

* Answer: ```C:\Users\Wade\Desktop\Relic_location```

* Explanation

> What is the name of the folder the attacker exfiltrated the files to? (for example: exfil_folder)

* Answer: ```exfiltration```

* Explanation