# Bot commands

List of bot commands

# Help

The command displays help on commands.

## `!help` {docsify-ignore} :id=help

Shows list of available commands and additional information on specified command.

<!-- tabs:start -->

#### ** Using **

`!help <command>`

#### ** Arguments **

<br>

Argument | Type | Require
---------|:-----:|:---------------:
Command | [The commandcode](/arguments?id=command-code) | No

<!-- tabs:end -->

---

# Voice channel

The command controls the voice of the bot

---

## `!v join` {docsify-ignore} :id=v-join

The command makes the bot to join in the voice channel.  
The bot enters the channel on which the user is using the command.

> [!WARNING]
> For using this command you need to be in voice channel.

---

## `!v leave` {docsify-ignore} :id=v-leave
The command makes the bot to leave from the voice channel.

---

## `!v volume` {docsify-ignore} :id=v-volume
The command sets the bot voice volume.

<!-- tabs:start -->

#### ** Using **

`!v volume <volume_level>`

#### ** Arguments **

<br>

Argument | Type | Rquire
---------|:-----:|:---------------:
Volume level | [Unsigned integer (0-100)](/arguments?id=integer-unsigned) | Yes

<!-- tabs:end -->

---
# Youtube

The command controls YouTube player.

> [!WARNING]
> For use this commands you need to add bot to you voice channel by command [`!v join`](/commands?id=v-join)

## `!play` {docsify-ignore} :id=short-play

Short command for add the bot to the voice channel and start playing specified YouTube video.

> [!NOTE]
> This command automaticly adds the bot to you voice channel

<!-- tabs:start -->

#### ** Using **

`!play <youtube_link>`

#### ** Arguments **

<br>

Argument | Type | Rquire
---------|:-----:|:---------------:
YouTube link | [Link](/arguments?id=link) | Yes

<!-- tabs:end -->

---

## `!y add` {docsify-ignore} :id=y-add

The command adds song to playlist.

<!-- tabs:start -->

#### ** Using **

`!y add <youtube_link>`

#### ** Arguments **

<br>

Argument | Type | Rquire
---------|:-----:|:---------------:
YouTube link | [Link](/arguments?id=link) | Yes

<!-- tabs:end -->

---

## `!y play` {docsify-ignore} :id=y-play

The command starts playing songs from playlist.

---

## `!y stop` {docsify-ignore} :id=y-stop

The command stops playing playlist.

---

## `!y clear` {docsify-ignore} :id=y-clear

The command clear playlist.

> [!NOTE]
> The command don't stops playing current song.

---

## `!y skip` {docsify-ignore} :id=y-skip

The command skips current song.

---

## `!y list` {docsify-ignore} :id=y-list

The command shows list of songs in playlist.

---

# Online Radio

The command for listening online radio stations.

> [!WARNING]
> For use this commands you need to add bot to you voice channel by command [`!v join`](/commands?id=v-join)

## `!r play` {docsify-ignore} :id=r-play

The command starts playing specified radio station by link.
> [!WARNING]
> Needs to be specified link for online radio station stream! Web pages is not a stream.  
> You can find this by request in Google `radio m3u`  
> Sample stream link: `http://air2.radiorecord.ru:9003/rr_320`

<!-- tabs:start -->

#### ** Using **

`!r <stream_link>`  
`!r play http://air2.radiorecord.ru:9003/rr_320`

#### ** Arguments **

<br>

Argument | Type | Rquire
---------|:-----:|:---------------:
Stream link | [Link](/arguments?id=link) | Yes

<!-- tabs:end -->

---

## `!r list` {docsify-ignore} :id=r-list

The command shows the list of built-in radio stations.

---

## `!r station` {docsify-ignore} :id=r-station

The command starts playing specified radio station by key.

<!-- tabs:start -->

#### ** Using **

`!r station <station_key>`  
`!r station metalvoice`

#### ** Arguments **

<br>

Argument | Type | Rquire
---------|:-----:|:---------------:
Station key | [Station key](/arguments?id=station-key) | Yes

<!-- tabs:end -->

---

## `!r stop` {docsify-ignore} :id=r-stop

The command stops playing the radio.

---

# Weather

The command shows weather forecast for specified place.

## `!w` {docsify-ignore} :id=weather

The command show weather forecast.  
If place not specified, the command shows deffault place from guild config.

<!-- tabs:start -->

#### ** Using **

`!w`  
`!w <place>`  
`!w New-York`

#### ** Arguments **

<br>

Argument | Type | Rquire
---------|:-----:|:---------------:
Place | [String](/arguments?id=string) | No

<!-- tabs:end -->

---

# News

The command shows news from specified category

## `!n` {docsify-ignore} :id=news
The news command. Shows news from specified category.  
Selects news from specified country in guild settings.

<!-- tabs:start -->

#### ** Using **

`!n`  
`!n <category>`

#### ** Arguments **

<br>

Argument | Type | Rquire
---|:---:|:---:
Category | [News category](/arguments?id=news-category) | No

#### ** Categories **

<br>

Category | Description
---|---
business | Busines news
entertainment | Entertainment news
health | Health news
science | Science news
sports | Sport news
technology | Technology news

<!-- tabs:end -->

---

# Translate

The translate command.  
Using Yandex.Translate for translate the text.

## `!t` {docsify-ignore} :id=translate

The command translates specified text to specified language

<!-- tabs:start -->

#### ** Using **

`!t <language> <text>`  
`!t ru Hello World! This text will be translated into Russian language.`

#### ** Arguments **

<br>

Argument | Type | Rquire
---|:---:|:---:
Language | [Language code](/arguments?id=lang-code) | Yes
Text | [String](/arguments?id=string) | Yes

#### ** Available languages **

<br>

Language | Code | Language | Code
:--- | ---: | :--- | ---:
Azerbaijani | az | Malayalam | ml
Albanian | sq | Maltese | mt
Amharic | am | Macedonian | mk
english | en | Maori | mi
Arabic | ar | Marathi | mr
Armenian | hy | Mari | mhr
Afrikaans | af | Mongolian | mn
Basque | eu | German | de
Bashkir | ba | Nepali | ne
Belarusian | be | Norwegian | no
Bengali | bn | Punjabi | pa
Burmese | my | Papiamento | pap
Bulgarian | bg | Persian | fa
Bosnian | bs | polish | pl
Welsh | cy | Portuguese | pt
Hungarian | hu | Romanian | ro
Vietnamese | vi | Russian | ru
Haitian (Creole) | ht | sebouan | ceb
Galician | gl | Serbian | sr
Dutch | nl | Sinhala | si
Gornomariysky | mrj | Slovak | sk
Greek | el | Slovenian | sl
Georgian | ka | Swahili | sw
Gujarati | gu | sundanese | su
Danish | da | Tajik | tg
Hebrew | he | thai | th
Yiddish | yi | Tagalog | tl
indonesian | id | Tamil | ta
Irish | ga | Tatar | tt
italian | it | Telugu | te
Icelandic | is | Turkish | tr
spanish | es | Udmurt | udm
Kazakh | kk | Uzbek | uz
Kannada | kn | Ukrainian | uk
Catalan | ca | Urdu | ur
Kyrgyz | ky | Finnish | fi
Chinese | zh | french | fr
Korean | ko | Hindi | hi
braid | xh | Croatian | hr
Khmer | km | czech | cs
Lao | lo | swedish | sv
Latin | la | Scottish | gd
Latvian | lv | Estonian | et
Lithuanian | lt | Esperanto | eo
Luxembourgish | lb | Javanese | jv
Malagasy | mg | japanese | ja
Malay | ms

<!-- tabs:end -->

---

# Currency rate

The command shows currency rate and cat convert one currency to another.

## `!c` {docsify-ignore} :id=currency

The command shows currency rate for specified currencies.  
If currency not specified shows currency rate for currencies from guild settings.

> [!NOTE]
> Can specify one or some currencies.

<!-- tabs:start -->

#### ** Using **

`!c`  
`!c <currency>`  
`!c USD RUB UAH`

#### ** Arguments **

<br>

Argument | Type | Rquire
---|:---:|:---:
Currency | [Currency code](/arguments?id=currency-code) | No

#### ** Available currencies **

<br>

Currency | Code | Currency | Code
:--- | ---: | :--- | ---:
Ruble | RUB | US dollar | USD
Moldovan Leu | MDL | Canadian Dollar | CAD
Uzbek sum | UZS | Norwegian Krone | NOK
Czech Koruna | CZK | Pound sterling | GBP
Belarusian ruble | BYN | Forint | HUF
Indian Rupee | INR | Ukrainian hryvnia | UAH
Zloty | PLN | Rand | ZAR
Singapore Dollar | SGD | Euro | EUR
Swiss franc | CHF | Tenge | KZT
Yen | JPY | Danish krone | DKK
Azerbaijani manat | AZN | Yuan | CNY
Som | KGS | Turkish Lira | TRY
New Romanian Leu | RON | New Turkmen Manat | TMT
Somoni | TJS | Swedish crown | SEK
Armenian Dram | AMD | Won | KRW
Bulgarian lion | BGN | Australian Dollar | AUD
Hong kong dollar | HKD | Brazilian Real | BRL
SDR (Special Drawing Rights) | XDR

<!-- tabs:end -->

---

## `!c conv` {docsify-ignore} :id=c-conv

The command converts one currency to another.

<!-- tabs:start -->

#### ** Using **

`!c conv <first_currency> <second_currency> <sum>`  
`!c conv RUB USD 1000`

#### ** Arguments **

<br>

Argument | Type | Rquire
---|:---:|:---:
First currency | [Currency code](/arguments?id=currency-code) | Yes
Second currency | [Currency code](/arguments?id=currency-code) | Yes
Sum | [Number](/arguments?id=number) | Yes


#### ** Available currencies **

<br>

Currency | Code | Currency | Code
:--- | ---: | :--- | ---:
Ruble | RUB | US dollar | USD
Moldovan Leu | MDL | Canadian Dollar | CAD
Uzbek sum | UZS | Norwegian Krone | NOK
Czech Koruna | CZK | Pound sterling | GBP
Belarusian ruble | BYN | Forint | HUF
Indian Rupee | INR | Ukrainian hryvnia | UAH
Zloty | PLN | Rand | ZAR
Singapore Dollar | SGD | Euro | EUR
Swiss franc | CHF | Tenge | KZT
Yen | JPY | Danish krone | DKK
Azerbaijani manat | AZN | Yuan | CNY
Som | KGS | Turkish Lira | TRY
New Romanian Leu | RON | New Turkmen Manat | TMT
Somoni | TJS | Swedish crown | SEK
Armenian Dram | AMD | Won | KRW
Bulgarian lion | BGN | Australian Dollar | AUD
Hong kong dollar | HKD | Brazilian Real | BRL
SDR (Special Drawing Rights) | XDR

<!-- tabs:end -->

---

# Polls

The command for making polls

> [!WARNING]
> For one guild can be made only one poll.

## `!p new` {docsify-ignore} :id=p-new

The command makes new poll.

<!-- tabs:start -->

#### ** Using **

`!p new <Answers>`

#### ** Arguments **

<br>

Argument | Type | Rquire
---|:---:|:---:
Answers | [Answers list](/arguments?id=answers) | Yes

<!-- tabs:end -->

---

## `!p vote` {docsify-ignore} :id=p-vote

Vote command. Sets you vote to specified answer.

<!-- tabs:start -->

#### ** Using **

`!p vote <answer_number>`

#### ** Arguments **

<br>

Argument | Type | Rquire
---|:---:|:---:
Answer number | [Unsigned integer](/arguments?id=integer-unsigned) | Yes

<!-- tabs:end -->

---

## `!p end` {docsify-ignore} :id=p-end

The command ends the poll.

---

# Map

Команда отправки карты.


## `!m` {docsify-ignore} :id=map

The command sends the map image for specified place.

<!-- tabs:start -->

#### ** Using **

`!m <type> <zoom> <place>`  
`!m map 17 Moscow`

#### ** Arguments **

<br>

Argument | Type | Rquire
---|:---:|:---:
Type | [Map type](/arguments?id=map-type) | Yes
Zoom | [Unsigned integer (1-17)](/arguments?id=integer-unsigned) | Yes
Place | [String](/arguments?id=string) | Yes


#### ** Типы карты **

<br>

Type | Description
:---|:---
map | Default map
sat | Satellite shots

<!-- tabs:end -->

---

# Geo IP

Determination of location by IP address.

## `!geoip` {docsify-ignore} :id=geoip

The command determines location by IP address.
<!-- tabs:start -->

#### ** Using **

`!geoip <ip_address>`  
`!geoip 123.123.123.123`

#### ** Arguments **

<br>

Argument | Type | Rquire
---|:---:|:---:
IP address | [String](/arguments?id=string) | Yes

<!-- tabs:end -->

---

# Twitch announcer

Twitch stream announcer

> [!WARNING]
> For using this command you needs to have [admin rules](/configuration?id=admin-rules)!

## `!twitch add` {docsify-ignore} :id=twitch-add

The command adds streamer to announcer.

<!-- tabs:start -->

#### ** Using **

`!twitch add <twitch_login>`  

#### ** Arguments **

<br>

Argument | Type | Rquire
---|:---:|:---:
Twitch login | [String](/arguments?id=string) | Yes

<!-- tabs:end -->

---

## `!twitch remove` {docsify-ignore} :id=twitch-remove

The command removes streamer from announcer.

<!-- tabs:start -->

#### ** Using **

`!twitch remove <twitch_login>`  

#### ** Arguments **

<br>

Argument | Type | Rquire
---|:---:|:---:
Twitch login | [String](/arguments?id=string) | Yes

<!-- tabs:end -->

---

# Greetings for new users

Adds greetings message for new joined users.

> [!WARNING]
> For using this command you needs to have [admin rules](/configuration?id=admin-rules)!

## `!greetings add` {docsify-ignore} :id=greetings-add

The command adds greetings message.

<!-- tabs:start -->

#### ** Using **

`!greetings add <text>`  

#### ** Arguments **

<br>

Argument | Type | Rquire
---|:---:|:---:
Text | [String](/arguments?id=string) | Yes

<!-- tabs:end -->

---

## `!greetings remove` {docsify-ignore} :id=greetings-remove

The command removes greetings from guild.

---

## `!greetings test` {docsify-ignore} :id=greetings-test

The command sends greetings message for you.