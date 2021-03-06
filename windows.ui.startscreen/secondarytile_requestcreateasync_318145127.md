---
-api-id: M:Windows.UI.StartScreen.SecondaryTile.RequestCreateAsync(Windows.Foundation.Point)
-api-type: winrt method
-api-device-family-note: xbox
---

<!-- Method syntax
public Windows.Foundation.IAsyncOperation<bool> RequestCreateAsync(Windows.Foundation.Point invocationPoint)
-->

# Windows.UI.StartScreen.SecondaryTile.RequestCreateAsync

## -description
Displays the **Pin to Start**  flyout above a specified location, through which the user can confirm that they want to create the secondary tile, which in turn creates the tile.

> On Windows Phone 8.1, the secondary tile is created through this call without showing the user a flyout, prompting them for confirmation, or allowing them to choose a tile size or title text. Note that when using the [RequestCreateAsync](secondarytile_requestcreateasync.md) method to pin a secondary tile in Windows Phone 8.x app, the app is suspended and the user is taken to the Start screen. This same API call on a PC does not suspend the program. Therefore, be aware that any code called after [RequestCreateAsync](secondarytile_requestcreateasync.md) is not guaranteed to be run before the app is suspended. To avoid this potential issue you should use the OnSuspended event of your app to run any code, such as updating the pinned tile, that should be run before the app suspends. To see an example of this pattern, download and run the [Tile update on suspend sample](http://go.microsoft.com/fwlink/p/?LinkId=394144).

## -parameters
### -param invocationPoint
The point used as the lower-right corner of the **Pin to Start**  flyout.

## -returns
An object that provides information concerning the asynchronous create operation.

## -remarks

## -examples

## -see-also
[RequestCreateAsync](secondarytile_requestcreateasync_1444672734.md), [Secondary tiles sample](http://go.microsoft.com/fwlink/p/?linkid=231487), [Tile Update On Suspend  sample](http://go.microsoft.com/fwlink/p/?LinkId=394144)