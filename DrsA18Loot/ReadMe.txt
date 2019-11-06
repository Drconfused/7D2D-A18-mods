DrsA18Loot

Installing
 In the 7 days to die root directory you need to have a folder named Mods. Put the mod you want into that folder and start game.


Carbboard boxes = construction loot
tool boxes = tool loot
coffee maker
microwave
toaster

		<block name="cntMedicalPileSmall" prob=".8"/>
		<block name="cntMedicalPileMedium" prob=".2"/>
		<block name="cntAmmoPileSmall" prob=".8"/>
		<block name="cntAmmoPileMedium" prob=".2"/>
		<block name="cntFoodPileSmall" prob=".4"/>
		<block name="cntFoodPileMedium" prob=".1"/>





 0.04
	-added blood loot box to the medicine group of loot 
	-reworked the Trader Reweard Loot as a hook for other mods of mine.
	-lowered the chance for the powered version of the doors and hatches to be in the loot.
		was at prob=".1" and is now at prob=".01"
 
 0.03
	-rearranged the loot and added more items to the possible findings to hopefully a more reasonable level. I am thinking that some will want it further nerfed and some would prefer the monty haul it was before. 
	-added in a chance for some boxes to not be lootable, so if you come across some that don't have an E to pickup that is because it spawned as a regular pallet without pickup chance.
	
 0.02
	-added destroy event to the pallet brown boxes so destroying them adds the loot box to your inventory.
	-expanded the loot obtained by each of the loot boxes, closer to being happy with the loot balance. Minor adjustments may be made in the future.
	
 0.01
	Define loot boxes to add to the game.
			
		Pallet Loot Boxes				
			Cardboard Boxes Loot
				3 grades A, B, C
				A will have the most valuable loot.
			Foodboxes
			Ammoboxes
				
		
For each Loot box the following documents must have additions in;
1. items.xml
	-this defines the item itself and what the items it turns into when 'consumed'
	-if the loot in question is a fixed amount you can avoid making it into a quest by using the following property
		<property name="Create_item" value="ItemInQuestion*"/>
		<property name="Create_item_count" value="setAmount*"/>
		*multiple items can be defined using a comma, you also need to give the count amount in the same order so that it would look like this
			<property name="Create_item" value="Item1,Item2,Item3"/>
			<property name="Create_item_count" value="2,5,1"/>
			This would give the following amounts for the items;
				Item1 = 2 
				Item2 = 5
				Item3 = 1
			The list can be as long as you want and is not random.
	-must define the icon that the item is going to use. Either an existing item/block name or one has to be made and put into the 	UIAtlases/ItemIconAtlas folder in the Mod.
	
2. quests.xml
	The loot boxes work on the basis of a quest which allows for a fine tuned and random content being listed for rewards. 
	
3. loot.xml
	-loot tables can defined for each Loot Box type, consider that the existing loot groups may already be standard enough to utilize and you may not need to define a new loot group for a given loot box.
	-Using the loot group alone with the count="all" does not work for quests for some reason.
	-Will have to define each loot group and use that in the quest field rather than just a single call to the loot.xml

4. blocks.xml
	-if replacing an existing block like I did with the cardboard pallets the proper block will need to be found and its variants defined in blocks.xml and then be used in the blockplaceholders.xml so that on generation they are randomly placed.
		Blocks I want to replace
			-Pallets - cardboard boxes become construction loot
			-Tool boxes - tool loot boxes
			-ammo piles - ammo loot boxes
			
	
5. blockplaceholders.xml
	-defines the types of blocks that an existing block that is placed during generation can be converted into.

What are each of the categories that we would expect to see in construction related loot boxes?
		Blocks and or bars
			Awning
				awningBlockVariantHelper
			Wood Frame
				woodFrameBlockVariantHelper
			Iron Frame
				scrapIronFrameBlockVariantHelper
			Rebar Frame
				rebarFrameBlockVariantHelper
			Trussing
				metalTrussingIBeamBlockVariantHelper
			Concrete
				pouredConcreteBlockVariantHelper
			Flagstone
				flagstoneBlockVariantHelper
			Brick
				brickBlockVariantHelper
			Glass
				glassBlockVariantHelper
				glassBulletproofBlockVariantHelper
			Sandbag
				sandbagBlockVariantHelper
			Fence
				metalFenceRailingTrellisSheetBlockVariantHelper
				woodFenceRailingTrellisSheetBlockVariantHelper
			Catwalk
				woodCatwalkBlockVariantHelper
			*steel frames
				plan to make the framework for steelframe blocks that with an x amount of forged steel can 
			Bars
				woodBars
				woodBarsCentered
				ironBarsCentered
				ironBars
			
			Doors and hatches
				woodHatch1_v1
				
				secureDoorWooden

			
		Materials
			Steel
				resourceForgedSteel
			Iron
				resourceForgedIron
				resourceScrapIron
			Wood
				resourceWood
			Cobblestone
				resourceCobblestones
			Cement
				resourceCement
			Concrete
				resourceConcreteMix
			Sand
			
			Clay
				resourceClayLump
			Rock
				resourceRockSmall				
			Lead
				
			Brass
				resourceScrapBrass
			Metal Pipe
				resourceMetalPipe
			Nails
				resourceNail
			Mechanical Parts
				resourceMechanicalParts
			Scrap Polymers
				resourceScrapPolymers
			Electrical Parts
				
			Duct Tape
				resourceDuctTape
			
		Tools
			power
				nailgun
					
				auger
					
				chainsaw
					
			hand held
				Hammer
					meleeToolClawHammer
				Wrench
					meleeToolWrench
				Wiretool
					meleeToolWireTool
				Sledgehammer
					
				Shovel
					
				Pickaxe
					
				Axe
					
				Fireaxe
				
				Paint Tool
					meleeToolPaintTool
				
			Tooparts
				toolParts
		Electrical
			Lighting
				ceilingLight01_player
				industrialLight01_player
				industrialLight02_player
				lanternLight_player
				spotlightPlayer
			Relays
				electricwirerelay
				electrictimerrelay
			Generators or Battery banks
				solarbank
				solarCell
				batterybank
				generatorbank
		Trap
		Literature
			make a specific category of construction related books
			bladeTrap
			autoTurret
			barbedFence
			barbedWireSheet
			dartTrap
			shotgunTurret
			trapSpikesIronDmg0
			trapSpikesWoodDmg0
			electricfencepost
		Furniture
			woodFurnitureBlockVariantHelper
			toiletBlockVariantHelper
		Signs
			woodSignBlockVariantHelper
			metalSignLetterNumberBlockVariantHelper