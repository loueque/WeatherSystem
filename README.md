## WeatherSystem
Connect and experience true weather across games from sunny, to rain and snow.

Use this in any game that experiments with a day-cycle like roleplays, simulators, car games, and more! 

## Versions
0.1.0
Created module, instances.

## Why making this?

Well, I found the motivation and work to make a Weather Module since there aren't many weather systems or plugins out there on Roblox that can make such a system as it is, so, I wanted to create this for all developers and users to explore and experiment with it.

Using this inside of a game such as Westover Islands, High-School games, and a game like Jailbreak could be helpful and resourceful to have rotated weather around a game such as a snowy weather, cloudy during the day and night, or more.

Yes, you can mishape these. :)

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

|Function|Returns|Description|
|-|-|-|
|Weather:OnPrint()|**N/A**|Prints a string or text found in a weather table.|

|Function|Returns|Description|
|-|-|-|
|Weather:GetMeterFromWeathers()|**N/A**|Finds a event or bindable function.|

### Events

|Function|Returns|Description|
|-|-|-|
|Weather.New()|**N/A**|Begins a new weather + dialogs a new weather system.|

|Function|Returns|Description|
|-|-|-|
|Weather.Start()|**N/A**|Starts the weather, any type of weather.|

|Function|Returns|Description|
|-|-|-|
|Weather.End()|**N/A**|Ends the weather, starts a new process with Weather.Start() / Weather.New()|

|Function|Returns|Description|
|-|-|-|
|Weather.Cycle()|**N/A**|With Weather.Start(), it'll cycle from day-to-night.|

|Function|Returns|Description|
|-|-|-|
|Weather.ChooseRandom()|**N/A**|Chooses a random weather, like Sunny or Snowy.|
