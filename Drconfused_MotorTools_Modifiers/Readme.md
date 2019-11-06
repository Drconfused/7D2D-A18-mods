Welcome to Drconfuseds madness!
Version 0.06

	Auger and Chainsaw - Power Tool Series

Contents 
* 	ATTACHMENTS
*	TO DO/WISH LIST
*	VERSION HISTORY
*	THANKYOUS
*	MADNESS NOTES
*	MODDERS NEED TO KNOW BASIS

ATTACHMENTS

		-modEngineTurbo1 = 10% increase in speed
		-modEngineTurbo2 = 25% increase in speed
		-modEngineTurbo3 = 50% increase in speed
		
		-modGasTank1 = 25% increase in gas tank size
		-modGasTank2 = 50% increase in gas tank size
		-modGasTank3 = 100% increase in gas tank size
		
		-modReserveGasTank1 = 25% increase in gas tank size
		-modReserveGasTank2 = 50% increase in gas tank size
		-modReserveGasTank3 = 100% increase in gas tank size
		
		-modMotorToolExtension1 = 10% increase in range
		-modMotorToolExtension2 = 25% increase in range
		-modMotorToolExtension3 = 50% increase in range
		
		-modDiamondTip1 = 10% increased block damage but -100% damage to wood
		-modDiamondTip2 = 25% increased block damage but -100% damage to wood
		-modDIamondTip3 = 50% increased block damage but -100% damage to wood
		
		-modMotorToolSilencer = makes it so you can now mine and chop in peace. 
			
		-modChainsawTemperedFrame1 = 
			25% increase in degradation max and lower degradation per use
		-modChainsawTemperedFrame2 = 
			50% increase in degradation max and lower degradation per use
		-modChainsawTemperedFrame3 = 
			75% increase in degradation max and lower degradation per use
			
			
TO DO/WISH LIST
	1. Work towards balance - fun, and challenge
	2. Changing recipes to reflect their nature to make it more immersive
	3. Test the car battery in items.xml effect_group ModSlots to see if the batteries can be affected by a mod_item and if that can carry into the battery bank
	4. Discover if a wider auger can be built and how those attributes work
	5. Carbon Alloy Framing for the motortools to increase durability related values
	6. Figure out how the tools affect the heatmap and if it can be separated from the sound values or if those are intrinsically linked. If it is separate and there is a heat specific value than a heat sink could be developed to soak up the heat rather than the Noise Dampner doing both.
			this is inside of a torch item
			<property name="HeatMapStrength" value="4.05"/>
			<property name="HeatMapTime" value="1200"/>
	7. Considering making a Reserve Fuel Tank attachment that would allow for a 2nd fuel tank attachment for even more fuel. 
	8. Schematic icons built and schematics activated
	9. Recipes built/balanced and added into the progression tables. Considering making unique recipe requirements so that engineering & science are both needed or finding loot to craft these items.
	10. loot.xml additions so the added items can be distributed.
	11. Nail gun additions
	12. Impact Wrench additions if I can get permission from Elucidus.
	13. Get a lawnmower icon in and see if something in hold position could be good candidate for a future model addition of a lawnmower.
	14. Make an sdx version and add a localization for better in game look.

	
	
VERSION HISTORY
	0.07
		-Added schematic icons for all of the current icons in the mod.
		-adapted some feedback by RussianDood after he test my mod out
			corrected progression file to properly add them into progression.
			corrected a case sensitive error in sounds.xml
		
	0.06
		-added in Reserve Gas Tank with icon and tints that can stack with the other Gas Tank for those that prefer more gas over the other attachments. (Currently keeping both using a percentage increase rather than hard number, but may change that)
		-added tint to the customicon in diamond blades
		-adding the progression file and putting the recipes in to be bound to the gating system.
		-added tint to the gas tank 2, 3
		-added Chainsaw Tempered Frame mod (be careful this is a permanent attachment to your chainsaw and you can't change it out.
		
		
	0.05
		adding in the motor tool silencer with its own icon.

	0.04
		adding in icons for	
			-Engine Turbo mods
			-Gas Tank mods
			-Better Handles 

	0.03
		adding in Better Handles to reduce kickback/recoil
		added in an icon for the augerblade mods (*my original icon feel free to use it as you wish)

		
	0.02
		adding in 2 other version of each mod tool.
		
		-modEngineTurbo1 = 10% increase in speed
		-modEngineTurbo2 = 25% increase in speed
		-modEngineTurbo3 = 50% increase in speed
		
		-modGasTank1 = 25% increase in gas tank size
		-modGasTank2 = 50% increase in gas tank size
		-modGasTank3 = 100% increase in gas tank size
		
		-modMotorToolExtension1 = 10% increase in range
		-modMotorToolExtension2 = 25% increase in range
		-modMotorToolExtension3 = 50% increase in range
		
		-modDiamondTip1 = 10% increased block damage but -100% damage to wood
		-modDiamondTip2 = 25% increased block damage but -100% damage to wood
		-modDIamondTip3 = 50% increased block damage but -100% damage to wood		
	
	0.01
		 Initial build. Established the direction the mod is to take. Simply put, to add attachments to the motor tools/power tools in the game so that immersion with increasing the function of the powertools is less game breaking than just making the tool overall better right from the start.
		 
		 - modEngineTurbo1 - a 40% increase to engine speed when installed into either the chainsaw or auger.
		 - modGasTank1 - a 50% increase in gas capacity when installed into either the chainsaw or auger.
		 - modMotorToolExtension - a 50% increase in range when installed into either the chainsaw or auger.
		 

THANKYOUS

First and foremost JRBARRIO gets my deepest gratitude for some initial correspondence between him and I on his headshots/dismemberment mod was my initial deeper looking into the xml and its different attributes and I have only got deeper in since.

Thank you Mayic/Jayic for getting me even more excited about adding to my mods and gaining deeper insights into the workings of xml and giving a great sense of community.

Xajar because his flagstone frames are my most used block hands down, until I have enough resources and a good stupply of wet flagstone blocks or self upgrading steel or a crap ton of rebar frames.

Stallionden, specifically your mining machine was a game changer for me was interacted with every moment I had. I couldn't just have one, but had to have 10 or so. It was a great addition for basebuilders and will surely be inspiration to future projects I help manifest.

And of course a massive thankyou to the FunPimps for continuing to work on this game.


		

MADNESS NOTES

	-HANDLING VALUES = 
		I spent a bunch of time testing some of the different HANDLING VALUES only to realize that I was running another mod that interacted with those values and it has a 'z' on the start of its name so it was overriding all my tests. Going to have to get into a habit of using exportcurrentconfigs.
		At this time my better handles are going to stay as is, till I grasp better how to balance it with the other attachments, especially if I add in things like the extension causing handling issues.
		I made one of the testing attachments have the same HANDLING values as the rocket launcher and wow it was damn hard to control.
		
	-SORT ORDER = 
		I believe the order of loading is done alphabetically. Makes me kind of wish there was a LOOT (skyrim) type sorter or a load order program for running our mods.
	
	-ITEM_MODIFIERS 
		TAGS =
			installable_tags
				this checks the item when attempting to place the mod into the slot to see if it has the tag if yes than does it currently have something in is modifier_tags already? if no allow insert.
			modifier_tags
				this mainly references the location and is in place to prevent doubling up on modifiers when we only want one modifier to be capable of being added in that slot.
			blocked_tags
				possibly an item has both the installable and modifier tag but is blocked from being able to use this modifier.
			type
				attachment
					can be removed from the slot
				mod
					cannot be removed from the slot 
			rarity
				I believe this is referenced by the loot ?
		PROGRESSION.XML
			Learned that for an items recipe to be added into the progression tables than it needs to have the code  tags="learnable" in its recipe name= line.
			If you put a recipe into 2 different perks you only need one of those perks meeting the requirement to unlock the recipe. I think the way around that would be to make the recipe require 2 or more items that can only be crafted by the specific perks, this way that recipe in theory requires the extra perks for it to be crafted. Or it has to be a team effort, or if the items are in the loot tables then it has to be found.
	
	
MODDERS NEED TO KNOW BASIS

console commands for mod testing and related values
	exportcurrentconfigs



