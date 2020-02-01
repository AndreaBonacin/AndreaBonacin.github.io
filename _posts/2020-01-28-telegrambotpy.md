---
title: "Telegram Bot in Python"
date: 2018-01-28
tags: [Telegram, bot, API, Python]
header:
  image: "/images/perceptron/percept.jpg"
excerpt: "Telegram, Bot, API, Python"
mathjax: "true"
---

# Telegram Bot in Python

## H2 Heading

### H3 Heading

Here's some basic text.

And here's some *italics*

Here's some **bold** text.

What about a [link](https://github.com/andreabonacin)?

Here's a bulleted list:
* First item
+ Second item
- Third item

Here's a numbered list:
1. First
2. Second
3. Third

Python code block:
```python

import telegram
import time import sleep

id = '1053691647'
rest = 'AAEdXnh79nz-Dpn44dq2br56VUBjdIcoftY'
tk = id + ':' + rest

bot = telegram.Bot(token=tk)
#print(bot.getMe())

def myupdate():
    updates = bot.getUpdates()
    print([u.message.text for u in updates])


chatid = bot.get_updates()[-1].message.chat_id
print(chatid)


bot.send_chat_action(chat_id=chatid, action=telegram.ChatAction.TYPING)
time.sleep(3)

bot.send_message(chat_id=chatid, text="I'm sorry Dave I'm afraid I can't do that.")

bot.send_message(chat_id=chatid, 
                 text="*bold* _italic_ `fixed width font` [link](http://google.com).", 
                 parse_mode=telegram.ParseMode.MARKDOWN)
bot.send_message(chat_id=chatid, 
                 text='<b>bold</b> <i>italic</i> <a href="http://google.com">link</a>.', 
                 parse_mode=telegram.ParseMode.HTML)
```



Here's some inline code `x+y`.

Here's an image:
<img src="{{ site.url }}{{ site.baseurl }}/images/perceptron/linsep.jpg" alt="linearly separable data">

Here's another image using Kramdown:
![alt]({{ site.url }}{{ site.baseurl }}/images/perceptron/linsep.jpg)

Here's some math:

$$z=x+y$$

You can also put it inline $$z=x+y$$
