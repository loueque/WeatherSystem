## WeatherSystem
Connect and experience true weather across games from sunny, to rain and snow.

Use this in any game that experiments with a day-cycle like roleplays, simulators, car games, and more! 

## Versions
0.1.0
Created module, instances.

## API

While working with Weather_Systems, there are many classes that are chosen, inserted and deleted whenever cycled throughout a day, or used in seasonal-days like Christmas.

You can configure, change, or even create your own systems inside of the module for dates or type of weather into your game!

Something like this is used in chosing a weather:

```lua

local WeatherClasses = {
	
	["Sunny"] = {
		["Percentage"] = 1;
		["Length"] = math.random(180, 480); -- You can configure math.random() into any number you like.
		["String"] = "Wet, humid in Roblox.";
		Atmosphere = Instance.new "Atmosphere";
		Rays = Instance.new("SunRaysEffect");
		DOF = Instance.new("DepthOfFieldEffect");
		
		["SunnyAmbience"] = {
			["Ambient"] = 1, 1, 1;
			["Brightness"] = 2;
			["EnviornmentDiffuse"] = 1;
			["EnviornmentSpecular"] = 0.5;
			["OutDoor"] = 1, 1, 1;
			["ShadowSoftness"] = 0;
		}
	}
}

```  

### Functions

|Function_Name||Returns|
|---||---|
|Weather.Start()||**Begins the weather.**|
