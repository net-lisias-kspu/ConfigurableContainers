# Configurable Containers :: Change Log

* 2019-1221: 2.4.8 (allista) for KSP 1.8.1
	+ Hangar patch:
		- Added a procedural fuel tank made from Procedural Adapter
	+ In APR ResourceUpdater no longer handles dynamic resources
	+ Corrected LH2O ratio in CryoEngines tank config
	+ Added CryoCooling variant of LH2O tank config
	+ Fixed InvalidOperationException on tank add/remove
* 2019-1130: 2.4.7.1 (allista) for KSP 1.8.1
	+ Updated AT_Utils
* 2019-1114: 2.4.7 (allista) for KSP 1.7.2
	+ Supports KSP-1.8.1
	+ IFS is fully compatible with CC patches
	+ Rebalanced "Snacks and Soil" tank config to keep 1u food to 1u soil
		- as suggested in #30 by @LouisCyfer
	+ Small performance improvements.
* 2019-0617: 2.4.6.0.1 (allista) for KSP 1.7.2
	+ Added patches
		- Mining Expansion
		- Kerbal Planetary Base System
		- ReStock+
		- Streamline - Engines and Tanks
	+ Updated patches
		- Bluedog Design Bureau
		- Mk2 Expansion
		- Mk3 Expansion
		- Near Future Propulsion
		- Mk2.5 Spaceplane Parts
		- Squad
	+ Corrected a typo in squad xenon tanks' names
* 2019-0528: 2.4.5.1 (allista) for KSP 1.7.0
	+ Using latest AT_Utils
* 2019-0514: 2.4.5 (allista) for KSP 1.7.0
	+ Added ability to change UI color scheme at runtime
		- Added "C" button to the tank manager window titlebar which summons the Color Scheme dialog
* 2019-0428: 2.4.4 (allista) for KSP 1.4.5
	+ Compatible with KSP-1.7
	+ Fixed MM Warnings (multiple NEEDS)
	+ Fixed in-editor part cloning/symmetry bug (issue #31)
* 2018-1016: 2.4.3.4 (allista) for KSP 1.4.5
	+ Version bump due to an update of AT_Utils.
* 2018-0913: 2.4.3.3 (allista) for KSP 1.4.5
	+ Using latest AT_Utils
* 2018-0831: 2.4.3.2 (allista) for KSP 1.4.3
	+ Recompiled against KSP-1.4.5
	+ Added Machinery to Components tank type when Ground Construction is installed.
* 2018-0615: 2.4.3.1 (allista) for KSP 1.4.3
	+ Recompiled against the new version of AT_Utils
	+ SpecializedParts are also used by GC now
* 2018-0510: 2.4.3 (allista) for KSP 1.4.1
	+ Added patches for Bluedog Design Bureau and Making History Expansion.
	+ Recompiled for KSP-1.4.3
* 2018-0327: 2.4.2 (allista) for KSP 1.3.1
	+ Compatible with KSP-1.4.1
	+ Twealscaled tanks retain volume on load.
		- Removed support for ProceduralParts =(
	+ Added SpareParts to Components TankType for DangIt.
	+ Updater Squad patch
	+ Supporting KWRocketryRebalanced. Can't support multiple KWR flavors and this one is the first to support KSP-1.4.1.
			- Well, it's possible with multiple .ckans, but I don't have the time =(
	+ Updated patches for Mk2/Mk3Exp, FTPlus, Mk2PlaneParts
* 2017-1220: 2.4.1.2 (allista) for KSP 1.3.1
	+ Compatibility patch for MM-3.+
* 2017-1111: 2.4.1.1 (allista) for KSP 1.3.1
	+ Fixed Cryogenic/CryoCooling NEEDS, fixed KarbonitePlus requirement for Metal.
	+ Update TankTypes.cfg
		- added Snacks support (Snacks --> Food, Soil --> Soil)
		- modified KolonyTools support --> ColonySupplies are visible/usable/transferable even if USI-LS is not installed
	+ Added Chemicals to LiquidChemicals for KolonyTools.
	+ Attempt to fix #10 using the patch suggested by @Starwaster.
	+ Fixed issues:
		- 16 - Attempting to change configuration when none exists results in NullReferenceException
		- 18 - Tweakscaled tank saved prior to installation of CC gets capacity reset to un-scaled value
		- 20 - Lag/freeze when placing tanks in VAB
* 2017-0622: 2.4.1 (allista) for KSP 1.3.0
	+ All tanks except high-pressure now use TankManager. Wings use IncludeTankType to restrict contents to liquid chemicals.
	+ Updated patches:
			- Stock
			- FuleTanks+
			- ModularRockeSystems
			- NearFuture
			- KWRocketry
			- Mk3 Expansion
		- Added patches:
			- Mk2.5 spaceplane parts
			- Fuel Tank Expansion
			- B9 Procedural Wings
		- Added patch for B9 mods made by ShadyAct to *IntrusivePatches* optional folder. See the archive structure and the included readme file for details.
	+ Part info now respects Include/ExcludeTankTypes options.
	+ CC modules are now properly initialized when they're added to existing parts (in flight) by MM. This should fix most of incompatibility with other fuel switches.
* 2017-0605: 2.4.0.6 (allista) for KSP 1.2.2
	+ Compatible with KSP-1.3
	+ Fixed Metal tank type as pointed out by TheKurgan.
	+ Removed Plutonium-238 as it is internal resource for USI
* 2017-0222: 2.4.0.5 (allista) for KSP 1.2.2
	+ Corrected CKAN metadata.
	+ Small bugfixes.
* 2017-0205: 2.4.0.4 (allista) for KSP 1.2.2
	+ Added patch for GPOSpeedFuelPump for time being.
* 2017-0115: 2.4.0.3 (allista) for KSP 1.2.2
	+ Added FindTankType by resource_name method to TankType library.
	+ Added ForceSwitchResource method to SwitchableTank.
	+ GroundConstruction will be using MaterialKits, so added it to Components TankType users.
	+ Using round-trip format for the volume field.
* 2017-0104: 2.4.0.2 (allista) for KSP 1.2.2
	+ Fixed TankManager initialization with disabled AddRemove capability.
	+ Fixed TankManager initialization using empty config.
	+ Fixed in-flight tank creation.
* 2016-1230: 2.4.0.1 (allista) for KSP 1.2.2
	+ Added patch for OPT Spaceplane Parts made by octarine-noise
	+ Small bugfixes.
* 2016-1219: 2.4.0 (allista) for KSP 1.2.2
	+ Compiled against KSP-1.2.2.
	+ Added boiloff and active cooling for cryogenic resources based on simple thermodynamics.
	+ Added CryoCooling tank type.
	+ Added KSPIE resources to TankTypes.cfg.
	+ Added tooltips with Info to TankType choosers.
	+ Replaced Tank Type dropdown list with the LeftRightChooser.
* 2016-1113: 2.3.1 (allista) for KSP 1.2
	+ Corrected Cryogenic tank type parameters.
	+ Fixed Food tank type.
	+ In Editor automatically remove current resource when trying to switch it or the tank type.
	+ Fixed Soil TANKTYPE definition.
	+ Fixed installation directive in CC-Core.netkan
	+ Fixed ProceduralParts bug and return to VAB bug. Closed #3 and #4.
* 2016-1026: 2.3.0 (allista) for KSP 1.2
	+ Added per-tank volume editing and volume definition in % along with m3.
	+ Added support for:
		- Tweak Scale
		- Procedural Parts
		- Parts ++with stock resources++ converted:
				- Stock
				- KW Rocketry
				- Mk2 Expansion
				- Mk3 Expansion
				- SpaceY-Lifters
				- SpaceY-Expanded
				- Fuel Tanks Plus
				- Modular Rocket Systems
				- Standard Propulsion Systems
				- Near Future Propulsion
				- Spherical and Toroidal Tank Pack
		- Supported resources:
				- Stock
				- TAC Life Support
				- Extrapalentary Launchapads
				- Near Future Propulsion
				- All USI
					- Some* of KSPIE
	+ Different TankTypes can now have different additional mass
	+ Added Tank Types:
		- Battery
		- Cryogenic
	+ Added Tank Setups:
		- TAC Life Support -- with food, water and oxigen. Made by Bit Fiddler.
		- LH2O -- with Liquid Hydrogen and Oxidizer for CryoEngines.
	+ Corrected unit/volume ratios for:
		- Monopropellant
		- Argon Gas
		- Liquid Hydrogen
		- Liquid Methane (which mod uses it?)
		- Karbonite
* 2016-1015: 2.2.0 (allista) for KSP 1.2
	+ No changelog provided
