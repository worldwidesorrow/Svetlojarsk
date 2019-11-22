# Svetlojarsk

* This POI is only to be used on the Chernarus map.

### Install Instructions

1. Click ***[Clone or Download](https://github.com/worldwidesorrow/Svetlojarsk/archive/master.zip)*** the green button on the right side of the Github page.

	> Recommended PBO tool for all "pack", "repack", or "unpack" steps: ***[PBO Manager](http://www.armaholic.com/page.php?id=16369)***
	
2. Unpack your server PBO and place file ***svetlojarsk.sqf*** in directory ***dayz_server\modules***

3. Repack your server PBO.

4. Unpack your mission PBO and open file ***init.sqf***.

	Find this line:
	
	```sqf
	if (isServer) then {
	```
	
	Put this line below it:
	
	```sqf
	call compile preprocessFileLineNumbers "\z\addons\dayz_server\modules\svetlojarsk.sqf";
	```

5. Save the file and repack your mission PBO
