# Local Storage:
## Introducing HTML5 Storage:

What I will refer to as “HTML5 Storage” is a specification named Web Storage.

**So what is HTML5 Storage?** Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser.

Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you.
  

## Using HTML5 Storage:

HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like `parseInt()` or `parseFloat()` to coerce your retrieved data into the expected JavaScript datatype.

`interface Storage {`

  `getter any getItem(in DOMString key);`

  `setter creator void setItem(in DOMString key, in any data);`

`};`

## Tracking Changes to the HTML5 Storage Area:

If you want to keep track programmatically of when the storage area changes, you can trap the storage event.

The storage event is fired on the window object whenever `setItem()`, `removeItem()`, or `clear()` is called and actually changes something. For example, if you set an item to its existing value or call `clear()` when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area. 

> `if (window.addEventListener) {`
>
> `window.addEventListener("storage", handle_storage, false);`
>
>`} else {`
>
>`window.attachEvent("onstorage", handle_storage);`
>
>`};`

> `function handle_storage(e) {`
>
>  `if (!e) { e = window.event; }`
>
>`}`

-------

StorageEvent Object

| Property | Type | Description|
| ------------ | ------------- | ------------- |
| key | string | the named key that was added, removed, or modified |
| oldValue | any | the previous value (now overwritten), or null if a new item was added |
| newValue | any | the new value, or null if an item was removed |
| url* | string | the page which called a method that triggered this change |

	
					 

-----

## HTML5 Storage in Action:

How does it work? Every time a change occurs within the game, we call this function:


`function saveGameState() {`

`if (!supportsLocalStorage()){ return false; }`

`localStorage["halma.game.in.progress"] = gGameInProgress;`

` for (var i = 0; i < kNumPieces; i++) {`

`localStorage["halma.piece." + i + ".row"] = gPieces[i].row;`

`localStorage["halma.piece." + i + ".column"] = gPieces[i].column;}`

`localStorage["halma.selectedpiece"] = gSelectedPieceIndex;`

`localStorage["halma.selectedpiecehasmoved"] =gSelectedPieceHasMoved;`

`localStorage["halma.movecount"] = gMoveCount;`

`return true;`
`}`

**To more info please :[ Visit This Page](http://diveinto.html5doctor.com/storage.html)**








