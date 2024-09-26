# Security & Bug Bounty

_This policy is valid from the 1st of November of 2024_

At Felix, we take security very seriously. We've designed our smart contracts and the systems around them to help reduce the risk of vulnerabilities, and we have a roadmap of different tasks and tools we'll implement to harden our system more as we grow.&#x20;

Among the many initiatives, we're starting a Bug Bounty program. Whether you are an experienced hacker, security researcher, or software engineer, we invite you to scrutinize and help us harden the security of our systems. In return, we'll distribute payouts to the reporters who responsibly disclose any bugs or security vulnerabilities they might find.

Below, you'll find a table describing the types of vulnerabilities in the program for both the smart contract and the web application. This follows the same criteria used by [Immunefi](https://immunefi.com/).

## Smart Contract

<table><thead><tr><th width="127">Level</th><th>Impact</th></tr></thead><tbody><tr><td>4. Critical</td><td>- Direct theft of any user funds, whether at-rest or in-motion, other than unclaimed yield<br>- Direct theft of any user NFTs, whether at-rest or in-motion<br>- Permanent freezing of funds<br>- Permanent freezing of NFTs<br>- Predictable or manipulable RNG that results in abuse of the principal, NFT or other participants<br>- Protocol insolvency<br></td></tr><tr><td>3. High</td><td>- Theft of unclaimed yield<br>- Permanent freezing of unclaimed yield<br>- Permanent freezing of unclaimed royalties<br>- Temporary freezing of funds<br>- Temporary freezing NFTs<br></td></tr><tr><td>2. Medium</td><td>- Smart contract unable to operate due to lack of token funds<br>- Block stuffing<br>- Griefing (e.g. no profit motive for an attacker, but damage to the users or the protocol)<br>- Theft of gas</td></tr><tr><td>1. Low</td><td>- Contract fails to deliver promised returns, but doesn't lose value</td></tr></tbody></table>

## Web App

<table data-header-hidden><thead><tr><th width="131">Level</th><th>Impact</th></tr></thead><tbody><tr><td>Critical</td><td>- Execute arbitrary system commands<br>- Retrieve sensitive data/files from a running server, such as:<br>        - /etc/shadow<br>        - database passwords<br>        - blockchain keys<br>(this does not include non-sensitive environment variables, open source code, or usernames)<br>- Taking down the application/website<br>- Taking down the NFT URI<br>- Taking state-modifying authenticated actions (with or without blockchain state interaction) on behalf of other users without any interaction by that user, such as:<br>        - Changing registration information<br>        - Commenting<br>        - Voting<br>        - Making trades<br>        - Withdrawals, etc.<br>- Changing the NFT metadata<br>- Subdomain takeover with already-connected wallet interaction<br>- Direct theft of user funds<br>- Malicious interactions with an already-connected wallet, such as:<br>        - Modifying transaction arguments or parameters<br>        - Substituting contract addresses<br>        - Submitting malicious transactions<br>- Direct theft of user NFTs<br>- Injection of malicious HTML or XSS through NFT metadata<br></td></tr><tr><td>3. High</td><td>- Injecting/modifying the static content on the target application without JavaScript (persistent), such as:<br>        - HTML injection without JavaScript<br>        - Replacing existing text with arbitrary text<br>        - Arbitrary file uploads, etc.<br>- Changing sensitive details of other users (including modifying browser local storage) without already-connected wallet interaction and with up to one click of user interaction, such as:<br>        - Email or password of the victim, etc.<br>- Improperly disclosing confidential user information, such as:<br>        - Email address<br>        - Phone number<br>        - Physical address, etc.<br>- Subdomain takeover without already-connected wallet interaction</td></tr><tr><td>2. Medium</td><td>- Changing non-sensitive details of other users (including modifying browser local storage) without already-connected wallet interaction and with up to one click of user interaction, such as:<br>        - Changing the first/last name of user<br>        - Enabling/disabling notifications<br>- Injecting/modifying the static content on the target application without JavaScript (reflected), such as:<br>        - Reflected HTML injection<br>        - Loading external site data<br>- Redirecting users to malicious websites (open redirect)</td></tr><tr><td>1. Low</td><td>- Changing details of other users (including modifying browser local storage) without already-connected wallet interaction and with significant user interaction, such as:<br>        - Iframing leading to modifying the backend/browser state (must demonstrate impact with PoC)<br>- Taking over broken or expired outgoing links, such as:<br>        - Social media handles, etc.<br>- Temporarily disabling user to access target site, such as:<br>        - Locking up the victim from login<br>        - Cookie bombing, etc.</td></tr></tbody></table>

## Vulnerability Disclosure Policy

### Introduction

Felix is committed to ensuring the security of our systems and protecting our users' data. We value the work of security researchers and ethical hackers who help us maintain high security standards. This policy provides guidelines for conducting vulnerability research and reporting security issues.

### Scope

This policy applies to the following systems and services:

* \*.felixapp.xyz
* any smart contract deployed via the platform

Any services not explicitly listed here are excluded from the scope of this policy.

### Guidelines

We require that all researchers:

1. Make every effort to avoid privacy violations, degradation of user experience, disruption to production systems, and destruction of data during security testing.
2. Perform research only within the scope set out above.
3. Use the identified communication channels to report vulnerability information to us.
4. Keep information about any vulnerabilities you've discovered confidential until we've had 90 days to resolve the issue.

### Safe Harbor

When conducting vulnerability research according to this policy, we consider this research conducted under this policy to be:

* Authorized in view of any applicable anti-hacking laws, and we will not initiate or support legal action against you for accidental, good-faith violations of this policy.
* Authorized in view of relevant anti-circumvention laws, and we will not bring a claim against you for circumvention of technology controls.
* Lawful, helpful to the overall security of the Internet, and conducted in good faith.

You are expected, as always, to comply with all applicable laws. If legal action is initiated by a third party against you and you have complied with this policy, we will take steps to make it known that your actions were conducted in compliance with this policy.

### Reporting a Vulnerability

We accept vulnerability reports via [security@felixapp.xyz](mailto:security@felixapp.xyz). Reports may be submitted anonymously.

We do not require that you provide your real name when reporting a vulnerability.

What we would like to see from you:

* Well-written reports in English will have a higher chance of being accepted.
* Reports that include proof of concept code be in the the Stacks mainnet or the testnet will be more likely to be accepted.
* Reports that include only crash dumps or other automated tool output will most likely not be accepted.
* Reports that include products not on the covered list will most likely be ignored.

Please include the following in your reports:

* Detailed description of the vulnerability
* Steps to reproduce the issue
* Proof of concept (if possible)
* Impact of the issue
* Suggested mitigation or fix (if known)

### What you can expect from us:

* A timely response to your email (within 2 business days).
* An open dialog to discuss issues.
* Notification when the vulnerability analysis has completed each stage of our review.
* An expected timeline for patches and fixes (usually within 7 days).
* Credit for discovering the issue (if you want it).

### Disclosure Policy

* Let us know as soon as possible upon discovery of a potential security issue, and we'll make every effort to quickly resolve the issue.
* Provide us a reasonable amount of time to resolve the issue before any disclosure to the public or a third party. We suggest at least 90 days.
* Make a good faith effort to avoid privacy violations, destruction of data, and interruption or degradation of our services during your research.
* Do not post or share any information about the vulnerability without our explicit permission. If you inadvertently cause a privacy violation, interruption, or degradation of service, please let us know immediately.

### Rewards

Felix is a bootstrapped company with no investors behind it. For now we cannot offer the same bounties you see on the bigger platforms, but still we are deeply appreciative of your efforts to help keep our systems secure. As a token of our gratitude, we offer the following:

* 100 STX for the successful disclosure of any Critical Level issues
* 50 STX for the successful disclosure of any High Level issues
* 25 STX for the successful disclosure of any Medium issues
* 10 STX for the successful disclosure of any Low issues

While it's early days, we must limit the bounties payments per month to 300 STX. We recognize that's way bellow what we should be offering. but we make a compromise of increasing it as the platform grows. We'll keep a public record of all disclosures in the queue and all the payments being done.

### Questions

For any questions about this policy, please contact us at [security@felixapp.xyz](mailto:security@felixapp.xyz).

Thank you for helping keep Felix and our users safe!
