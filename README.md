# AIP To Sigma

## Description
This project contains rules from F5 Distributed Cloud App Infrastructure Protection (AIP) in the [Sigma](https://sigmahq.io/) format. Sigma is a "Generic Signature Format for SIEM Systems" and could best be summed up as "Sigma is for log files what Snort is for network traffic and YARA is for files". 

Since AIP reached End-Of-Sale in June 2023 and will reach End-Of-Life in June 2024 the AIP Detection Engineering Team decided to create Sigma version of as many of our rules as possible so customers can take advantage of our rules in other products after June 2024. If any changes are made to existing rules in the AIP product or if new rules are created those changes will be pushed to this project shortly after. 

These rules are provided "as is" though every effort has been made to make them align as closely as possible with the AIP version of the rule. Field names have been changed to align with the [Sigma specification](https://github.com/SigmaHQ/sigma-specification) and not every AIP rule will have a Sigma version. There is likely going to be overlap with the base Sigma rules. 

## Usage
Rules can be converted into queries using the following tools:
- The [Sigma CLI](https://github.com/SigmaHQ/sigma-cli)
- [Uncoder.IO](https://uncoder.io/) (Community Edition of UncoderAI requires registration with work e-mail)
- [sigconverter.io](https://sigconverter.io/)
- If the Sigma CLI or Uncoder do not support your target query language it may be supported in [Sigma Legacy](https://github.com/SigmaHQ/legacy-sigmatools) tooling
- If you want to customize a rule and prefer a GUI to a text editor you can utilize the [SigmaHQ Rule Creation GUI](https://sigmahq.streamlit.app/)

If you would like to look up the AIP version of a rule the `id` field matches up with the Rule ID in the AIP platform if you are subscribed to Managed Rules. 

## Support
While each rule has been run through the [Sigma CLI](https://github.com/SigmaHQ/sigma-cli) in order to check for syntax errors please open up an Issue if you discover a syntax error. 

If you are an AIP customer and have any questions about this project please reach out to your PSE or the AIP SOC.

## Coverage and Roadmap
As of December 18th, 2023 we have converted 82% of the rules in the AIP Platform with 298 out of 363 converted. Of the remaining 65 rules: 45 cannot be converted, 4 are covered by other rules, and 16 require additional work. Updates will be made to the repo as we complete work on the remaining 16 rules. 

## Contributing
At this time we are not accepting pull requests. 

## Maintainers
[<img alt="Ethan Hansen" src="https://avatars.githubusercontent.com/u/140435226" width="80"/>](https://github.com/f5-ehansen) [<img alt="Levi Smith" src="https://avatars.githubusercontent.com/u/141268759" width="80"/>](https://github.com/lsmith8) [<img alt="Bria Atchley" src="https://avatars.githubusercontent.com/u/140658380" width="80"/>](https://github.com/briaaatchley)

## Acknowledgments
The original Sigma project was developed by Florian Roth and Thomas Patzke.

## License
The content of this repository is released under the following licenses:

* The [Sigma Specification](https://github.com/SigmaHQ/sigma-specification) and the Sigma logo are public domain
* The rules contained in the [SigmaHQ repository](https://github.com/SigmaHQ) are released under the [Detection Rule License (DRL) 1.1](https://github.com/SigmaHQ/Detection-Rule-License)

Copies of these licenses are included in this repo.