DrsA18Tools_Auger

Installing
 In the 7 days to die root directory you need to have a folder named Mods. Put the mod you want into that folder and start game.
 
0.01
	playing around with the auger.
	Hope to incrase the radius of damage
	Values changed:
		<property name="Tags" value="melee,heavy,tool,motorTool,attStrength,perkMiner69r,perkMotherLode,miningTool,perkSalvageOperations,canHaveCosmetic"/>
		<property class="Action0">
		
		<property class="Action0">	
			<property name="ToolCategory.Disassemble" value="1" param1="1"/>
			
		<effect_group name="meleeToolAuger">
			<passive_effect name="RoundRayCount" operation="base_set" value="4"/>
			<passive_effect name="MaxRange" operation="base_set" value="2.5"/>
			<passive_effect name="ModSlots" operation="base_set" value="3,4,5,6,7,8" tier="1,2,3,4,5,6"/>
			<passive_effect name="MaxRange" operation="base_set" value="4"/>
			<passive_effect name="BlockRange" operation="base_set" value="6"/>
			<passive_effect name="HarvestCount" operation="base_set" value="1" tags="salvageHarvest"/>


