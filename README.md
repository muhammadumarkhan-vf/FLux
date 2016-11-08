# FLux
Flux is the application architecture that Facebook uses for building client-side web applications. Flux is basically a pattren. it uses to persist states between different components and it follows uni-directional data flow unlinke other framework which support two way data-binding like angularjs.

#### As Flux is pattren, here are many implementations exist, few of them listed blow
Most popular are
  * Relay by facebook
  * Flux by facebook
  * Alt.js 
  * Redux it has more star on github but used for large scale application normally
Other implementation
  * Reflux
  * Flummox 
  * Fluxxor
  * Flux This
  * MartyJS
  * McFly
  * Fluxible
  * Delorean
  * Lux
  * Reflux
  * OmniscientJS
  * Fluxy
  * Material Flux
Each of these has it's pros and cons and it's depend on the type of application you are building
Read this for using which flux should i used https://github.com/kriasoft/react-starter-kit/issues/22
For comparison https://medium.com/social-tables-tech/we-compared-13-top-flux-implementations-you-won-t-believe-who-came-out-on-top-1063db32fe73#.42r112i33 

# Flux in detail
We are going to discuss flux implementation of flux pattren
this is basic of all  implementation.

# Three major parts of flux
* the dispatcher
* the stores
* views

# Flow
Views generate actions. Dispatcher it only exist per application. it is publisher/subscriber sort of things which receive actions and payload then it call registerd callback and pass payload to that action in stores.registered callback exist in store where data updates then store update views by call.

#Flux is probably better explained by explaining its individual components:
```
Actions – Helper methods that facilitate passing data to the Dispatcher
Dispatcher – Receives actions and broadcasts payloads to registered callbacks
Stores – Containers for application state & logic that have callbacks registered to the dispatcher
Controller Views – React Components that grab the state from Stores and pass it down via props to child components.

```
