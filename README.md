# eventbus_js
simple event bus for node.js

# how to use it.

```js

import EventBus from 'eventbus_js';

var myGlobalEvtBus = new EventBus();

myGlobalEvtBus.subscribe("TODO_ADD_EVENT", function(obj){
    console.log(1, obj.done);
});

myGlobalEvtBus.subscribe("TODO_ADD_EVENT", function(obj){
    console.log(2, obj.title);
});

myGlobalEvtBus.publish("TODO_ADD_EVENT", {done:false, title:"write JS"})

```
