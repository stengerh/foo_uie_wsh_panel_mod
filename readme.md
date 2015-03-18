##Overview

I've made a few minor modifications of the original component. Details can be found in the changelog below.

##Downloads

The latest component file can be downloaded on the [releases](https://github.com/marc2k3/foo_uie_wsh_panel_mod/releases) page.

##Changelog
```
v1.5.8
- ADD: fb.IsLibraryEnabled()

v1.5.8 Beta 1
- ADD: fb.ShowLibrarySearchUI(query) opens the Library>Search window populated with the query you set.
- ADD: fb.GetLibraryItems() returns a handle list of all items in library.
- ADD: on_library_changed callback for when library items are added, removed or modified.

v1.5.7.1
- ADD: window.Reload() so you can force a panel reload from your own menus, buttons, functions etc.

v1.5.7
- CHG: Compiled with new SDK. Requires foobar2000 v1.3 or above.
- ADD: Script errors are now displayed in a popup window in addition to the Console like it was previously.
- ADD: Default right click menu now has a "Reload" script option. This saves opening/closing the dialog when working on external files.
- CHG: Remove functions marked as obsolete 2+ years ago. There are newer alternatives for all of them.
	window.WatchMetadb 
	window.UnWatchMetadb
	window.CreateTimerTimeout
	window.CreateTimerInterval
	window.KillTimer
	UpdateFileInfo
- CHG: AppendMenuItem no longer accepts MF_POPUP as a flag. You should be using AppendTo instead.
- CHG: utils.GetAlbumArt removed as corresponding function has been removed from SDK.
- CHG: Safe mode disabled by default. If you're reading this, you're probably going to be using scripts that require this!
- FIX: EstimateLineWrap no longer leaves stray punctuation when wrapping text at end of line.
```

##Compiling

All required files are included using relative paths so it should compile as-is. I used Visual Studio 2013 Community Edition Update 4 which is completely free.
