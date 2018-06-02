# MacBook-Pro-TouchBar-Media-Controls
___
## What is the problem
On new MacBooks with TouchBar, when you open a media app an extra button for media control appears along with 4 fixed shortcuts. But sometimes it does not appear. It is due to system killing "nowPlayingTouchUI" service which is responsible to control the extra button.

<img width="1085" alt="touch bar shot 2018-06-02 at 11 15 45 am" src="https://user-images.githubusercontent.com/19741014/40871579-c8126b4a-665b-11e8-9ebc-71e8effdebc8.png">
<img width="1085" alt="touch bar shot 2018-06-02 at 11 15 50 am" src="https://user-images.githubusercontent.com/19741014/40871595-06257fee-665c-11e8-89f7-61714ea71f70.png">

## How to Use:-
1. Clone/Download the repository.

2. In most of the cases you only need to **double click on 'Start NowPlayingTouchUI'** to start 'nowPlayingTouchUI' service but if the service is already running and you are having problem, run **'Restart NowPlayingTouchUI' and then 'Start NowPlayingTouchUI'**.

## Automator Code
##### Start NowPlayingTouchUI
```applescript
tell application "NowPlayingTouchUI"
	activate
end tell
```
##### Restart NowPlayingTouchUI
```applescript
tell application "NowPlayingTouchUI"
	quit
end tell
```
