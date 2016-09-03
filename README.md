# now-go-instance

My personal tinyurl service

## Quick Start

- Start with local `config.json`
```bash
npm run start:local
```

- Start with remote config
```bash
# Make sure there is a remote config.json before run
npm run start:remote
```

#### Deploy to [now.sh](https://now.sh)
```bash
now # deploy current folder to now.sh
now alias set https://long-long-name.now.sh short-name
```

#### Deploy to any server

Create a `index.js`:  

```javascript
const go = require('now-go')
const configLocation = './config.json' // local file or remote url

go(configLocation)
```

Then `pm2 index.js`

## now-go

For more about now-go, checkout https://github.com/amio/now-go
