# LOCAL STORAGE FOR WEB:
* But they have three potentially dealbreaking :
1. Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.
2. Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
3. Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.

* userData allows web pages to store up to 64 KB of data per domain.
* Flash objects to store up to 100 KB of data per domain.

# what is HTML5 Storage:
* it’s a way for web pages to store named key/value pairs locally, within the client web browser
# USING HTML5 STORAGE:

`JavaScript datatype.

interface Storage {
  getter any getItem(in DOMString key);
  setter creator void setItem(in DOMString key, in any data);
};`

# TRACKING CHANGES TO THE HTML5 STORAGE AREA:
* The storage event is supported everywhere the localStorage object is supported
* you’ll need to check which event mechanism the browser supports.
you can do that with the storage event
`
if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};`


**STORAGEEVENT OBJECT**
|PROPERTY|TYPE|DESCRIPTION|
|-------|------|------|
|key|	string|	the named key that was added, removed, or modified|
|oldValue|	any|	the previous value (now overwritten), or null if a new item was added|
|newValue|	any	|the new value, or null if an item was removed|
|url*	|string	|the page which called a method that triggered this change|



# LIMITATIONS IN CURRENT BROWSERS:
* in order of importance, are “5 megabytes,” “QUOTA_EXCEEDED_ERR,” and “no.” “5 megabytes” is how much storage space each origin gets by default.

# HTML5 STORAGE IN ACTION:
very time a change occurs within the game, we call this function:

`function saveGameState() {
    if (!supportsLocalStorage()) { return false; }
    localStorage["halma.game.in.progress"] = gGameInProgress;
    for (var i = 0; i < kNumPieces; i++) {
	localStorage["halma.piece." + i + ".row"] = gPieces[i].row;
	localStorage["halma.piece." + i + ".column"] = gPieces[i].column;
    }
    localStorage["halma.selectedpiece"] = gSelectedPieceIndex;
    localStorage["halma.selectedpiecehasmoved"] = gSelectedPieceHasMoved;
    localStorage["halma.movecount"] = gMoveCount;
    return true;
}`
