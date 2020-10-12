BasisCore
====

BasisCore library 


## Installation

[![More Info](https://component.jit.su/component-badge.svg)]( https://basiscore.com/en/What-is-BasisCore)

Use 
```
<script src="http://basiscore.net/_js/basiscore.min.js"></script>
```
```
<script src="http://basiscore.net/_js/alasql.min.js"></script>
```

Then set Host setting:

```JavaScript
var host = {

Debug: false,

AutoRender: false , 

OnRendered: onRendered,

OnCallExecuted: onCallExecuted,

OnRendering: onRendering,

Settings: { 

'connection.web.callcommand':'http://127.0.0.1:8080/',

'connection.web.demo_basiscoreapi': 'http://dbsource.basiscore.net/data.json',

'connection.web.demo_userbehaviorapi':'http://dbsource.basiscore.net/data.json',

'default.dbsource.verb': 'post',

'default.call.verb':'get',

'default.viewCommand.groupColumn':'prpid',

'default.dmnid': '23',

'default.binding.regex':'\\{##([^#]*)##\\}' 

}

}
```
For initialization
```JavaScript
$(document).ready(async _ => {         
   await $bc().RenderAsync('.container')
})
```
 also you can set scripts in OnRendered function ro run after rendering
```JavaScript
function onRendered(e){}
```

