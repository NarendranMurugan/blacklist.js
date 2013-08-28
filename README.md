== BLACKLIST.JS ==

Blacklist.js
-------------

    **Blacklist.js** is a simple jquery plugin for blacklisting unwanted words.
    
    
### Implementation

#### Basic Usage

Include js

``` 
< script src='jquery.js'></script>
< script src='blacklist.min.js'></script>
```
    
```
  $('p').blacklist();
``` 
    
#### Changing Symbols

```
  $('p').blacklist({
    symbol: '@@@@'    
  });
``` 
#### Changing Color

```
  $('p').blacklist({
    color: 'red'
  });
``` 
#### Ignore Blacklist word
```
  $('p').blacklist({
      ignore: ['test', 'test1']
  });
``` 
#### Add to the list for blacklist on your page
```     
  $('p').blacklist({
      add_blacklist: ['ABCD', 'XXX']
  });
``` 
#### Overall customization
``` 
  $(document).ready( function() {
    $('p').blacklist(
      {
        color: '#006699',
        symbol: '$$$$',
        ignore: ['ass', 'jap'],
        add_blacklist: ['Senthil']
      });
  });
``` 