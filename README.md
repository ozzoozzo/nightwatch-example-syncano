# nightwatch-example-syncano
Nightwatch.js example

## Reading stuff
- http://nightwatchjs.org/
- https://www.syncano.io/blog/testing-syncano/

## Project Setup
- https://www.syncano.io/blog/testing-syncano/
- `npm init`
- `npm install nightwatch --save-dev`
- `npm install selenium-standalone --save-dev`
- edit `package.json` by adding a script `e2e-setup` with the command `selenium-standalone install`
- edit `package.json` by adding a script `e2e-start` with the command `selenium-standalone start`
- `npm run e2e-setup`
- `npm run e2e-start`


```ruby
---
selenium install:
from: https://selenium-release.storage.googleapis.com/2.53/selenium-server-standalone-2.53.1.jar
to: \nightwatch-example-syncano\node_modules\selenium-standalone\.selenium\selenium-server\2.53.1-server.jar
---
chrome install:
from: https://chromedriver.storage.googleapis.com/2.25/chromedriver_win32.zip
to: \nightwatch-example-syncano\node_modules\selenium-standalone\.selenium\chromedriver\2.25-ia32-chromedriver
---
ie install:
from: https://selenium-release.storage.googleapis.com/2.53/IEDriverServer_Win32_2.53.1.zip
to: \nightwatch-example-syncano\node_modules\selenium-standalone\.selenium\iedriver\2.53.1-ia32-IEDriverServer.exe
---
firefox install:
from: https://github.com/mozilla/geckodriver/releases/download/v0.11.1/geckodriver-v0.11.1-win64.zip
to: \nightwatch-example-syncano\node_modules\selenium-standalone\.selenium\geckodriver\0.11.1-ia32-geckodriver
---
```
