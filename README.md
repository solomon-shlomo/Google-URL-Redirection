# Google-URL-Redirection
Redirecting Users to Malicious website from GOOGLE.COM domain

Redirects are a useful function. However you need to be sure they are done safely. Otherwise you are putting your users in harm's way by enabling phishing attacks.

### POC for Redirecting users from GOOGLE.COM to Malicious Website.

GOOGLE assign a persistent unique parameter value for all domain names / web contents and it is needed for GOOGLE for redirecting users from GOOGLE search result to the destination website. [Parameter name "usg"].

##### 1. Host the malicious content / Setup phishing page

After hosting the malicious content, wait for GOOGLE to crawl the malicious content/domain.

##### 2. Search the malicious domain on GOOGLE [ icsirt.com ]
Search the malicious domain on GOOGLE then Right click on the malicious domain listed on the google search then copy the link location of the malicious domain and get the "usg" parameter value. Here the "usg" parameter value for my malicious website is "usg=AOvVaw2AcGMUccRudpmqkjcvluYq"

![screenshot from 2018-09-27 16-00-57](https://user-images.githubusercontent.com/18662912/46133246-068c7880-c20e-11e8-80fe-3b4dd4c6c58b.png)

Link location copied: [https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=2ahUKEwiihIaI49rdAhUFTI8KHQrDDBkQFjAAegQICRAB&url=http%3A%2F%2Ficsirt.com%2F&usg=AOvVaw2AcGMUccRudpmqkjcvluYq] Get the usg parameter and value.

##### 4. Craft the URL with GOOGLE domain.

A) Malicious website: http://icsirt.com/
<br>
</br>
B) USG paramenter value obtained from google search result for http://icsirt.com/ website: AOvVaw2AcGMUccRudpmqkjcvluYq
<br>
</br>
C) Final URL: https://www.google.com/url?sa=t&url=http://icsirt.com/&usg=AOvVaw2AcGMUccRudpmqkjcvluYq

There is no REDITECT NOTICE and therefore before clicking the URL, users belive the content is delivered from GOOGLE. This can lead to successful PHISHING ATTACK and DRIVE BY DOWNLOAD.

![screenshot from 2018-09-27 16-01-17](https://user-images.githubusercontent.com/18662912/46133255-0ab89600-c20e-11e8-9cf5-6c7c96a92960.png)

https://www.google.com/url?sa=t&url=http://icsirt.com/&usg=AOvVaw2AcGMUccRudpmqkjcvluYq  ====>  Redirected to http://icsirt.com/

GOOGLE SAYS THE REDIRECT NOTICE IS NOT A SECURITY FEATURE AND BY ADDING THE "USG" PARAMETER GOOGLE KNOWS THE URL IS INDEXED AND WILL BLOCK IT IF IT'S MALICIOUS. Malware writers often use obfuscation to make their files more difficult to detect or analyze. Also Fileless malware has attracted a lot of attention recently and security solutions are having difficulty in defending against it. Hope GOOGLE can block all new 0Day Malwares and obfuscated phishing pages.

https://in.linkedin.com/in/solomon-jesudasan-66b46367

![39b0fc67-48b1-4446-86d9-b428d09b84f4](https://user-images.githubusercontent.com/18662912/46135023-42294180-c212-11e8-9d3f-4b9770dbba50.png)

# Legal Disclaimer

This vulnerability is made and published for educational and ethical testing purposes only. Usage of the above vulnerability for attacking targets without prior mutual consent is illegal. It is the end user's responsibility to obey all applicable local, state and federal laws. I assume no liability and are not responsible for any misuse or damage caused by this program.
