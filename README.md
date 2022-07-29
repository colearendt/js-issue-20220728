# Version Conflict in Vuetify Beta dependencies

```
node --version
v16.15.1
npm --version
8.11.0
```

Warning on Install:
```
 WARN  conflicting versions for project dependency "@vitejs/plugin-vue":

       - ^3.0.0 injected by generator "undefined"
       - ^2.0.0 injected by generator "vue-cli-plugin-vuetify"

       Using newer version (^3.0.0), but this may cause build errors.
 WARN  conflicting versions for project dependency "vite":

       - ^3.0.0 injected by generator "undefined"
       - ^2.0.0 injected by generator "vue-cli-plugin-vuetify"

       Using newer version (^3.0.0), but this may cause build errors.
```

And error afterwards on any usage of `npm`:
```
npm ERR! code ERESOLVE
npm ERR! ERESOLVE could not resolve
npm ERR!
npm ERR! While resolving: vuetify@3.0.0-beta.5
npm ERR! Found: vite-plugin-vuetify@1.0.0-alpha.14
npm ERR! node_modules/vite-plugin-vuetify
npm ERR!   dev vite-plugin-vuetify@"^1.0.0-alpha.0" from the root project
npm ERR!
npm ERR! Could not resolve dependency:
npm ERR! peerOptional vite-plugin-vuetify@"1.0.0-alpha.12" from vuetify@3.0.0-beta.5
npm ERR! node_modules/vuetify
npm ERR!   vuetify@"^3.0.0-beta.0" from the root project
npm ERR!   peer vuetify@"^3.0.0-beta.4" from @vuetify/loader-shared@1.5.1
npm ERR!   node_modules/@vuetify/loader-shared
npm ERR!     @vuetify/loader-shared@"^1.5.1" from vite-plugin-vuetify@1.0.0-alpha.14
npm ERR!     node_modules/vite-plugin-vuetify
npm ERR!       dev vite-plugin-vuetify@"^1.0.0-alpha.0" from the root project
npm ERR!   1 more (vite-plugin-vuetify)
npm ERR!
npm ERR! Conflicting peer dependency: vite@2.9.14
npm ERR! node_modules/vite
npm ERR!   peer vite@"^2.7.0" from vite-plugin-vuetify@1.0.0-alpha.12
npm ERR!   node_modules/vite-plugin-vuetify
npm ERR!     peerOptional vite-plugin-vuetify@"1.0.0-alpha.12" from vuetify@3.0.0-beta.5
npm ERR!     node_modules/vuetify
npm ERR!       vuetify@"^3.0.0-beta.0" from the root project
npm ERR!       2 more (@vuetify/loader-shared, vite-plugin-vuetify)
npm ERR!
npm ERR! Fix the upstream dependency conflict, or retry
npm ERR! this command with --force, or --legacy-peer-deps
npm ERR! to accept an incorrect (and potentially broken) dependency resolution.
npm ERR!
npm ERR! See /Users/colearendt/.npm/eresolve-report.txt for a full report.

npm ERR! A complete log of this run can be found in:
npm ERR!     /Users/colearendt/.npm/_logs/2022-07-29T01_34_36_087Z-debug-0.log
```

# Vue 3 + Vite

This template should help get you started developing with Vue 3 in Vite. The template uses Vue 3 `<script setup>` SFCs, check out the [script setup docs](https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup) to learn more.

## Recommended IDE Setup

- [VS Code](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar)
