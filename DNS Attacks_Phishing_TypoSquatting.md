layout: col-sidebar
title: "DNS Attacks_Phishing_TypoSquatting"
author:
contributors:
permalink: /MyPageTitle
tags: ["attack", "XSS"]

---

{% include writers.html %}

## DNS Infrastructure
## What Is DNS
The acronym DNS stands for “Domain Name System”.
To better relate to this you can think of it as an “address book” where you look up a name that is tied to a unique address that you use for communicating with an individual, however this “address book” is for the internet and when you enter a domain name into a browser, it will be translated to the tied unique IP address which it will use to communicate to a machine and serve up content that is hosted on it The process of translating a domain to an IP address is known as a DNS lookup. DNS lookups are performed by dedicated servers called DNS resolvers. Your Wi-Fi router is typically preconfigured to send DNS queries to the resolver owned by your ISP. However, you can choose to configure your router, operating system, or browser to use a different resolver.
## Components of DNS Infrastructure
1.	DNS Servers: These are the backbone of DNS. DNS servers come in various types, such as recursive resolvers and authoritative servers. Recursive resolvers act like your personal investigators, fetching IP addresses on your behalf. Authoritative servers, on the other hand, have the answers. They hold the official records for a specific domain, and they’re the ones you turn to when you need the precise IP address for a particular website.
2.	DNS Resolvers: Think of DNS resolvers as your web browsers’ trusty assistants. When you type in a website address, the resolver is the first to spring into action. It contacts DNS servers to find the IP address for the site you want to visit. This crucial step ensures you reach your desired destination on the web.
## The role of DNS records and Zone files:
1.	DNS Records: If DNS is the backbone, DNS records are the words in the backbone’s language. These records store essential information, like IP addresses, mail server data, and aliases. Common record types include A (Address), CNAME (Canonical Name), and MX (Mail Exchange). These records tell DNS servers where to send your requests and emails and how to find websites.
2.	Zone Files: Imagine zone files as the organizers of the DNS library. Each domain has its zone file, which contains records that point to where the data for that domain is stored. These files are managed by domain administrators and provide authoritative DNS servers with the information they need to resolve queries for that domain. Zone files are essential for the smooth operation of DNS.
## Challenges
## Typosquatting
Typosquatting is when someone registers a domain name that is an intentionally misspelled version of another popular website. While many misspelled URLs won’t work or will redirect you, some of these fake websites that look real might be a source of malware, and visiting them could even lead to identity theft. Threat actors create and register domains similar to popular websites but with common typographical errors to exploit unsuspecting users who mistype URLs. The technique is similar to lookalike domains. But unlike lookalike domains in which attackers register domains that look confusingly similar to those of trusted brands typosquatting tries to cash in on users’ clumsiness with their keyboard.

 

## Example
# Example of character substitution
```python
domain = "legit-website.com"
phishing_domain = domain.replace("i", "l")  # Replacing 'i' with 'l'
print(phishing_domain)  # Outputs: "leglt-website.com" ```

