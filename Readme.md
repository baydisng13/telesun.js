<header>
<img src="https://github.com/abdiu34567/telesun.js/blob/main/assets/telesun.jpg" alt="logo" height="90" align="left">
<h1 style="display: inline">Telesun.js</h1>

Modern Telegram Bot API framework for App Script

[![Bot API Version](https://img.shields.io/badge/Bot%20API-v6.0-f36caf.svg?style=flat-square)](https://core.telegram.org/bots/api)
![JavaScript](https://img.shields.io/github/languages/top/abdiu34567/Lost_and_Found)
[![Telesun](https://img.shields.io/badge/telesun-v1.0-f36caf.svg?style=flat-square)](https://core.telegram.org/bots/api)
[![English chat](https://img.shields.io/badge/English%20chat-grey?style=flat-square&logo=telegram)](https://t.me/App_Script_Js)

</header>

## መግቢያ

ቴሌሰን ቦት የሚለዋወጥ የፕሮግራም እና የአከባቢ ድረ-ገጾች የሚናገረው አትክልት ነው ተግባራዊ መረጃዎት እና ተጠቃሚ መደብ የምንኖር እውነተኛ ነው።

ቴሌሰን ከ JavaScript እና [Apps Script](https://developers.google.com/apps-script) በሚገኝ አይነት ቦት ላይ የሆነውን እትም መጠቀም አድርጋችኋል።

### አማራጮች

- በ [Telegram Bot API 6.0](https://core.telegram.org/bots/api) የተጠቀሙ እትም
- በተለያዩ መረጃዎት መከታተል ያለ
- በ Google እናቶን እትም ላይ በ `Youtube`, `Drive`, `Gmail...` ተብሏል
- በጊዜ በተጨማሪ ወጥተን ወደ Google Cloud መገኘን
- በራሱ በ የ Google ተማሪ (Google sheet) ለመጠቀም አልቻልኩም
- የምንገኝ ስለ በለጠ የ `100+` ቦት መረጃ ይጠቀሙ
- በመንገድ ወደ ተከተለ የ `Basic Javascript` እና እንደሚጠቀሙ መቀመጫ ነው


---

## [Apps Script እና Telesun.js እንደመጠቀሚያ እና መጀመሪያ መረጃ](https://github.com/abdiu34567/telesun.js/wiki/Getting-Started)

---

<br>

### ምንዛሬ

በመከፋቱ ከተመነሻ `መረጃ እንደሚሰጠውን በአፕስ ስክሪፕት` እና በሌላ ክፍል ውጤቱ ከምሳሌ መከፋት እና `ምላሽ ተጠቅመን ወደ ተማሪዎች ላይ መመገብ` አልቻልኩም ።

```js
// ከአፕስ ስክሪፕት ውስጥ መመገብ ከማንበረት በተመነሻ የተመደበ የፋይና ትክክለኛ አካባቢ ይሰጠዋል
function WelcomeToTelesun() {
  // ለመመገብ የተቀበለ የታነበ አፕስ ስክሪፕት ውስጥ ተከታታይ የሆነ ስኩዕ ቶክን ይጠቀሙ
  const bot = new Bot.Telesun(<<botToken>>);

  // ለመቆጣጠር ለአንደኛው የስነልቦና ሰው ማህበረሰብ ይኖርበታል
  bot.Use((ctx) => ctx.reply("ሰላም ሰላም!"));

  // ለመከታተል <</start>> ኮማንድ ላይ የተቀበለ ስኩዕ ቶክን ይጠቀሙ
  bot.Start((ctx)=> ctx.reply("ይህ ምንዛሬ ኮማንድ ነው"))

  // ለምሳሌ <hello> መልዕክት ተጠቀመበት የተቀበለ ስኩዕ ቶክን ይጠቀሙ
  bot.Hears('hello', (ctx)=> ctx.reply("ይህ የመልዕክት መልዕክት ነው"))

  // ለምሳሌ ሎክ ተመን ላይ የተመነሻ መልዕክት ተጠቀመበት
  bot.Photo((ctx)=> ctx.reply("ይህ ሎክ ነው"))
}
```

ለተጨማሪ መረጃ ምንዛሬ [ምዝገባው](https://github.com/abdiu34567/telesun.js/wiki/Example-Bots) ዝርዝሩን ይመልከቱ

<br>

### ስለኛው አስነብበን

- **[ቴሌግራም ቡድን](https://t.me/App_Script_Js)**
- **[GitHub ሰነድ](https://github.com/abdiu34567/telesn.js/discussions)**
- **[መረጃ](https://github.com/abdiu34567/telesun.js/wiki)**

<br>

## መጀመሪያ ምንዛሬ
<br>
### 💊 ቴሌግራም ቶክን
ተመን የቴሌግራም ቦታ አፕነ በተመነሻ ተጠቅመን በ [BotFather](https://t.me/BotFather) በማግኘት አካባቢ ይደውሉ።
BotFather ይህን ቶክን እናመሰግናለን እናመሰግናለን፣ ይህም ለአንደኛው ቦታ ነው እና ወደ `123456789:AbCdfGhIJKlmNoQQRsTUVwxyZ` ወደታች ታሪክ አይደለም።
<br>

### 👩‍💻 የመጀመሪያ ለመመገብ ቦታ እናደርጋለን

➖ በ [ለማወቅ](https://github.com/abdiu34567/telesun.js/wiki/Long-Polling) የአትክምህ፣ የቡድንና የይለና ይደረገበት ቦታ።<br>
➖ በተጨማሪ ወደ `webhook` አገናኝ ተመን እናመጣለን

> - [አፕስ ስክሪፕት ፐሮጀንት መልእክት](https://github.com/abdiu34567/telesun.js/wiki/Getting-Started)
> - [አምፐርት ሊመጣ](https://github.com/abdiu34567/telesun.js/wiki/Import-Telesun)

```js
/**
 * የምንዛሬ የ doPost() ማድረግ ይፈጥሩ።
 * እናነግሩ በአንድ ለመቀጠል እና አንደ መረጃውን ለመሞከር ወደ << /startreg >> ኮማንዶ አቅርብዎ።
 * ተጨማሪ ወደ apps script ውስጥ ለመነሻዎ ውጤቱን በጣም መረጃውን ያግኙ።
 * ከዚህም በኋላ ወደ መከፋቱ መቆጣጠር ይጀምሩ።
 */

/**
 * አፕስ ስክሪፕት ለ Telesun Library ተጠቅመን
 * የቡድን ኮማንድ አካባቢ ለመጠቀም
*/
const bot = new Bot.Telesun(<<botToken>>);

function doPost(){

 /**
  * እናንተን ያግኙ በ /startreg ኮማንዶ ለመሞከር
  */
  bot.Command('startreg',(ctx)=>{

    //ይህንን የተለያዩ ምንዛሬ እናመሰግናለን
    ctx.reply("እባኮት መጠቀም ያለብን መለያ ያላቸውን መረጃ ይላኩልን ?")

    //እባኮት መረጃ በጣም መረጃውን በ አልባ ያስገቡ
    ctx.setStage("username")
  })

}

```

```js
/**
 * የምንዛሬ የ doPost() ማድረግ ይፈጥሩ።
 * እናነግሩ በአንድ ለመቀጠል እና አንደ መረጃውን ለመሞከር ወደ << /startreg >> ኮማንዶ አቅርብዎ።
 * ተጨማሪ ወደ apps script ውስጥ ለመነሻዎ ውጤቱን በጣም መረጃውን ያግኙ።
 * ከዚህም በኋላ ወደ መከፋቱ መቆጣጠር ይጀምሩ።
 */

/**
 * አፕስ ስክሪፕት ለ Telesun Library ተጠቅመን
 * የቡድን ኮማንድ አካባቢ ለመጠቀም
*/
const bot = new Bot.Telesun(<<botToken>>);

function doPost(){

 /**
  * እናንተን ያግኙ በ /startreg ኮማንዶ ለመሞከር
  */
  bot.Command('startreg',(ctx)=>{

    //ይህንን የተለያዩ ምንዛሬ እናመሰግናለን
    ctx.reply("እባኮት መጠቀም ያለብን መለያ ያላቸውን መረጃ ይላኩልን ?")

    //እባኮት መረጃ በጣም መረጃውን በ አልባ ያስገቡ
    ctx.setStage("username")
  })

}
```


```js
/**
 * እባኮት እናንተን የምንዛሬ የ doPost() ማድረግ እናዘንባለን፣ በመከፋቱ ያለብን ኮድ መቆጣጠር የተቻለ ምንዛሬውን መነሻ ተመን እናመጣለን።
 * ለአንደ የምንዛሬው መረጃ በ apps script ውስጥ ያቀናሉ
 */
function doPost(){

  ...... //❌ በማወቅ ተመን ከሚታገል እባኮት በጣም ይሄንን የምንዛሬ ማህበረሰብ አድርጉ

  //ስለዚህ መረጃው የ username ያለብን ምንዛሬ መነሻ ተመን እናመጣለን
  bot.Stage('username', (ctx)=>{
      //መነሻ ተመን እና አዲስ የ username ይዞ የመረጃ ግምት ተመን ለአንደኛው አዝማሚ አስመጡ

      //username የሚመጣውን መነሻ እናቀመጣለን
      let _Username = ctx.message().text

      //በአንደ ሰነዶ ላይ ለመቀመጥ ሊመረጡ የእያንዳንዱ የምንዛሬ የመረ

ጃ ግምት እናቀመጣለን
      Bot.TSession.set('username', _Username)

      //የተጠቀመበት ድረ-ገጽ እና ላይ መረጃ ለ ማንበረት እና መከታተል
      ctx.reply("እባኮት መጠቀም ያለበትን የመረጃ ግምት መመከር እናሳውቅ።\nምንዛሬ አዲስ የመረጃውን ግምት እና እስከ ሰነዶ ታሪክ በመቀመጥ እናሳውቃለን")
      
      //የ username መመረጃ በጣም የ password እናመጣለን
      ctx.setStage('password')
  })

}

```

```js
/**
 * ለአንደ ምንዛሬ እናንተን የምንዛሬ የ doPost() ማድረግ እናዘንባለን፣ በመከፋቱ ያለብን ኮድ መቆጣጠር የተቻለ ምንዛሬውን መነሻ ተመን እናመጣለን።
 * ለአንደ የምንዛሬው መረጃ በ apps script ውስጥ ያቀናሉ
 */
function doPost(){

  ...... //❌ በማወቅ ተመን ከሚታገል እባኮት በጣም ይሄንን የምንዛሬ ማህበረሰብ አድርጉ

  ...... //❌ በማወቅ ተመን ከሚታገል እባኮት በጣም ይሄንን የምንዛሬ ማህበረሰብ አድርጉ

   //ስለዚህ መረጃው የ password ያለብን ምንዛሬ መነሻ ተመን እናመጣለን
  bot.Stage('password', (ctx)=>{

       //መነሻ ተመን እና አዲስ የ password ይዞ የመረጃ ግምት ተመን ለአንደኛው አዝማሚ አስመጡ

       //username የሚመጣውን መነሻ እናቀመጣለን
      let _Username = Bot.TSession.getValue('username')

      //password የሚመጣውን መነሻ እናቀመጣለን
      let _Password = ctx.message().text

      //የተጠቀመበት ድረ-ገጽ እና ላይ መረጃ ለ ማንበረት እና መከታተል
      ctx.reply(`የተመን መመረጃ\n\n`+
     `መጠቀም የተቀበለበት ምንዛሬ: ${_Username}\n`+
     `የምንዛሬ ኮድ: ${_Password}`)
    }
  })


}
```


/**
 * እናንተን በ doPost() ወደገጠሩ እትም ወደኋላ አስማምጣት፣ በመከፋቱ ያለብን ኮድ መቆጣጠር የተቻለ ምንዛሬውን መነሻ ተመን እናመጣለን።
 * ለአንደ የምንዛሬው መረጃ በ apps script ውስጥ ያቀናሉ
 */
function doPost(){

  ...... //❌ በማወቅ ተመን ከሚታገል እባኮት በጣም ይሄንን የምንዛሬ ማህበረሰብ አድርጉ

  //ግንዛቤ እናንተን በ username የተለያዩ ምንዛሬ መነሻ ተመን እናመጣለን
  bot.Stage('username', (ctx)=>{
      //ምንዛሬ መነሻ የሚመጣውን መነሻ እናቀመጣለን

      //መነሻ ተመን እና አዲስ የ username ይዞ የመረጃ ግምት ተመን ለአንደኛው አዝማሚ አስመጡ

      //username የሚመጣውን መነሻ እናቀመጣለን
      let _Username = ctx.message().text

      //በአንደ ሰነዶ ላይ ለመቀመጥ ሊመረጡ የእያንዳንዱ የምንዛሬ የመረጃ ግምት እናቀመጣለን
      Bot.TSession.set('username', _Username)

      //የተጠቀመበት ድረ-ገጽ እና ላይ መረጃ ለ ማንበረት እና መከታተል
      ctx.reply("እባኮት መጠቀም ያለበትን የመረጃ ግምት መመከር እናሳውቅ።\nምንዛሬ አዲስ የመረጃውን ግምት እና እስከ ሰነዶ ታሪክ በመቀመጥ እናሳውቃለን")
      
      //የ username መመረጃ በጣም የ password እናመጣለን
      ctx.setStage('password')
  })

}

/**
 * እናንተን በ doPost() ወደገጠሩ እትም ወደኋላ አስማምጣት፣ በመከፋቱ ያለብን ኮድ መቆጣጠር የተቻለ ምንዛሬውን መነሻ ተመን እናመጣለን።
 * ለአንደ የምንዛሬው መረጃ በ apps script ውስጥ ያቀናሉ

 */
 ```js
function doPost(){

  ...... //❌ በማወቅ ተመን ከሚታገል እባኮት በጣም ይሄንን የምንዛሬ ማህበረሰብ አድርጉ

  ...... //❌ በማወቅ ተመን ከሚታገል እባኮት በጣም ይሄንን የምንዛሬ ማህበረሰብ አድርጉ

   //ስለዚህ መረጃው የ password ያለብን ምንዛሬ መነሻ ተመን እናመጣለን
  bot.Stage('password', (ctx)=>{

       //መነሻ ተመን እና አዲስ የ password ይዞ የመረጃ ግምት ተመን ለአንደኛው አዝማሚ አስመጡ

       //username የሚመጣውን መነሻ እናቀመጣለን
      let _Username = Bot.TSession.getValue('username')

      //password የሚመጣውን መነሻ እናቀመጣለን
      let _Password = ctx.message().text

      //የተጠቀመበት ድረ-ገጽ እና ላይ መረጃ ለ ማንበረት እና መከታተል
      ctx.reply(`የመተው ተመን\n\n`+
     `መጠቀም የተቀበለበት ምንዛሬ: ${_Username}\n`+
     `የምንዛሬ ኮድ: ${_Password}`)
    }
  })


}
```

Certainly! Here's the translation of the provided JavaScript code into Amharic:


<br>

### 📡 በረጅም የመዝገብ ቦት መነሻ ማግኘት
በተጨማሪም የተለያዩ ቦት ፋይሎት የመዝገብ መረጃ ለመሰብሰብ የሚችል ወቅታዊ ተለዋዋጭዎች ምንዛሬዎች በመመዝገብ የጽሁፍን ፋይሎት ባያንና የሚያምር መመዝገብ ይሆናል።
- የአሁኑን የመጠቀሚ ፋይሎት በ `code.gs` ምንዛሬ ነበር
- የአሁኑን የመጠቀሚ ምንዛሬ የ `doPost(e)` ነበር
በማለት እኛ እንደእርስዎ ይጠቀሙ። <br>
> ከገንዘብ ላይ በ `webhook url` እናም በላይ ማግኘት የፋይሎትዎ በመቀመጥ ተጠቅመን እናመጣለን [Deployment](https://github.com/abdiu34567/telesun.js/wiki/Deployments) ስለሚለዋወጥ ተመን ይመልከቱ

```js
/**
 * ይህ እንደአንደ እስከምንዛሬ የመረጃ ግምት መጠቀም ይጀምራል፣ እናንተ እንደምንመኝ እናመልክታለን
 */
function settingWebhook() {
  const token = "5862849341:AAHvKz2HGq5y9NBD4B4YAsEI0X9qE";

  //እንደአንደ በጽሁፉ የፋይል አድራጎት በ url እና ምሳሌ እንዲሆን እንጠቀሙ
  Bot.setWebHook(token, { url: "https://..." });
}
```

🌟💪 `እንደእርስዎ አስጠንቀመጡ`

<br>

## ፋይሎት
የ Telesun ምላሽ የነጥብ ስለሚለዋወጥ ነው። እንደ [MIT License](https://opensource.org/licenses/MIT) የተለዋወጥ ነው።
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
በዚህ መሠረት በአትክልት ተከፍላቸው። በነጻ ሊተግበሉ ነው፤ የተቀበሉት ፋይሎቶች በአስተያየቶች እና ድረ-ገጾች ውስጥ እንደ ሰጠው ለመሄድ አስፈላጊ ተመን እና ሊደረግ እንደ ሆነ እንዲሆን ይሆናል። ለማህበረሰብ ለመቀጠል ወቅታዊ እየተሞነ ተለዋወጥ አለው።
ስለዚህ ከአስተያየቶች ወደ ሊተግበሩ ወደ ምንዛሬ ባተኮርበው እንደአስተያየት እንዲሆን እና ከእያንዳንዱ ሰዓት በመያዝ ሊሆን ይገባል።
ተጨማሪ መነሻዎት እና አጠቃቀምዎት የሚጠቀሙበት ማህበረሰብ ይህን ስለ ማግኘት የዚህን ፋይሎት እናመልከት!
