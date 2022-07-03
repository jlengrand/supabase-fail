# Supabase fails to install with Open-WC

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/jlengrand/supabase-fail)

or run `$npm install && npm run build`


The error that shows up is 


```
...and 10 other files
(!) Circular dependency
node_modules/@supabase/realtime-js/dist/module/RealtimeSubscription.js -> node_modules/@supabase/realtime-js/dist/module/lib/push.js -> node_modules/@supabase/realtime-js/dist/module/RealtimeSubscription.js
[!] Error: 'w3cwebsocket' is not exported by node_modules/websocket/index.js, imported by node_modules/@supabase/realtime-js/dist/module/RealtimeClient.js
https://rollupjs.org/guide/en/#error-name-is-not-exported-by-module
```

