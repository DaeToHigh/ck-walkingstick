This is my walking stick resource for the QBCore framework

# Dependencies:
qb-core: https://github.com/qbcore-framework/qb-core
qb-inventory: https://github.com/qbcore-framework/qb-inventory

# Add to qb-core > shared > items.lua
```
['walking_stick'] 				 	 = {['name'] = 'walking_stick', 			  	  	['label'] = 'Walking Stick', 				['weight'] = 1, 		['type'] = 'item', 		['image'] = 'walking_stick.png', 			['unique'] = false, 	['useable'] = true, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'Walking Stick'},
```

# Add to qb-ambulancejob > config.lua
```
Config.Items = {
    label = Lang:t('info.safe'),
    slots = 30,
    items = {
        [1] = {
            name = "walking_stick",
            price = 0,
            amount = 50,
            info = {},
            type = "item",
            slot = 1,
        },
    }
}
```
