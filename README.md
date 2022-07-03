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


## And when trying to install and apply the rollup common js plugin

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/jlengrand/supabase-fail)

or run `$npm install && npm run build`


Here is the error that I get

```
(!) `this` has been rewritten to `undefined`
https://rollupjs.org/guide/en/#error-this-is-undefined
node_modules/@supabase/supabase-js/dist/module/SupabaseClient.js
1: var __awaiter = this && this.__awaiter || function (thisArg, _arguments, P, generator) {
                   ^
2:   function adopt(value) {
3:     return value instanceof P ? value : new P(function (resolve) {
...and 1 other occurrence
node_modules/@supabase/functions-js/dist/module/index.js
1: var __awaiter = this && this.__awaiter || function (thisArg, _arguments, P, generator) {
                   ^
2:   function adopt(value) {
3:     return value instanceof P ? value : new P(function (resolve) {
...and 1 other occurrence
node_modules/@supabase/gotrue-js/dist/module/GoTrueApi.js
1: var __awaiter = this && this.__awaiter || function (thisArg, _arguments, P, generator) {
                   ^
2:   function adopt(value) {
3:     return value instanceof P ? value : new P(function (resolve) {
...and 1 other occurrence

...and 8 other files
[!] (plugin commonjs--resolver) SyntaxError: Unexpected token (2:8)
node_modules/websocket/index.js (2:8)
```
