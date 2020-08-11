# iu2019.github.io
## Yandex Praktikum Sprint 10 project
### ver. 0.0.1

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
```
Please note: no country domain allowed other than .ru, as per the assignement
Please also note: no name division with '.' is allowed, again, as per assignement

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
- Number can start with +7 or 8 - style country code, but can't omit it 

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
