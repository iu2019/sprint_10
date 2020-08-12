# iu2019.github.io
## Yandex Praktikum Sprint 10 project
### ver. 0.0.3

Link: https://github.com/iu2019/iu2019.github.io
gh-pages: https://iu2019.github.io/

Goal: practice in git, github and regular expression usage on a form

Regular expression has been developed for four fields, matching the examples provided:

## Name:
```
Ян
Максим
Серёга
Ёль
Джон-Дон
```

Please note spaces are not allowed (i.e. no first name - last name combination allowed). 
Cyrillic letters only, case sensitive. First letter must be capital

## Email:
```
ya2@2ya.ru : digits allowed, other than in the first position of the name
ya-e@ya-ya.ru : dash allowed in the name and domain
ya@x.ru, y@ya.ru : name and domain can be as short as 1 symbol, country domain must be 2-3 symbols
some@mail.ya.ru - subdomains allowed
review.test@yandex.ru - dots in name are allowed since ver 0.0.2
```
Please note: no country domain allowed other than .ru, as per the assignment
Please also note: no name division with '.' is allowed, again, as per assignment

ver 0.0.2
Now allowing dot in the user name, not just the domain

ver 0.0.3
Corrected bug preventing the name to have just one symbol. Now truly allowed. Please note the first name symbol
must be a latin letter, the following ones can be as well digits, hyphen or underline. Leading or trailing
spaces not allowed.

## Phone
```
+7(925)900-90-90
+7(925) 900-90-90
+7 925-900-90-90
+79259009090
89259009090
```
- Please note only Russian (and other countries using +7 country code) numbers are allowed
- Any number of spaces and just one dash are allowed between groups, but not inside the groups,
    none of those are obligatory
- Brackets are accepted (optional) around the area code
- Number can start with either +7 or 8 - style country code, but can't omit it 

## Web site
```
http://ya.ru
https://www.ya.ru
http://2-domains.ru
http://ya.ru:98/
http://ya.com:30
http://ya.ru/path/to/deep/
http://ya-ya-ya.ru
http://8.8.8.8:8080
http://8.8.8.8:8080/page/to/deep#
http://mysite.com/path#
```

- Must start with http:// or https://
- May or may not contain www group
- Digits allowed 
- Dashes allowed
- Country domain: 2 or 3 letters
- Port assignement allowed: 1-4 digits
- IP address (rather than URL) allowed
- Both URL and IP-address can be continued by further names divided by slashes
- Slash may or may not finish the line
- One hash sign allowed at the end of the address, either followed by dash or not

Reasonable limitations are applied to the length of each input.

ver 0.0.2
- Now allowing hash sign in any web site address, not only an ip-based one
- Now limiting number of slahses to one in every occasion: //abc//dce disallowed
- Port number leading zeros disallowed, values 1 - 65535 only allowed
