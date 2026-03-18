## Master Doc

## DNS
- A quick note/explanation on DNS for my own understanding:\
When you type anywebsite.com into your browser, your computer has NO IDEA where that website actually LIVES; it only speaks in IP addresses. So it needs to translate that human-readable name into an IP address so it can connect to the actual webserver SERVING that site.
To do that, it asks your router. Your router then asks a DNS server (an internet phonebook) on your computer's behalf. By default, your router uses your ISP's (internet service provider) DNS server; **BUT,** you can change that!! Popular alternatives include Google (8.8.8.8), Cloudflare (1.1.1.1), and Quad9 (9.9.9.9). **I want to clarify: the IP's I've added in parenthesis aren't actual search engine's themselves, but the DNS server only.** They all have the same domain-to-IP mappings (i.e. regardless of WHERE you registered your domain, be it GoDaddy, namecheap, etc...all DNS servers have the same updated info), so they'll all return accurate results; the difference is in the perks.
Why switch? Each DNS provider has its own advantages. Cloudflare, for example, claims not to log your DNS queries, so if privacy is a priority, that's a perk. Quad9 blocks known malicious domains by default, which is pretty nice from a security POV.
Once your computer gets the IP back, your router forwards your traffic and you're connected to the webserver. And, now, you've reached anywebsite.com!
