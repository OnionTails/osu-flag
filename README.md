# osu-flag
Use this repository like a mirror for osu flags.
```js
(async () => {
  var countryCode = 'VN'
  const fetch = require('node-fetch');
  const fs = require('fs');
  var flag = await fetch(`https://raw.githubusercontent.com/CuSO4-c3c/osu-flag/master/${countryCode}.png`);
  var flag = await flag.buffer();
  await fs.writeFileSync('./flag.png', flag)
})();
```
The response is:

<img src = https://raw.githubusercontent.com/CuSO4-c3c/osu-flag/master/VN.png>
