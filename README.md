
```php
<?php

namespace YourPluginNamespace;

use pocketmine\event\Listener;
use pocketmine\event\player\PlayerInteractEvent;
use pocketmine\Player;
use pocketmine\plugin\PluginBase;
use pocketmine\utils\TextFormat;

class Main extends PluginBase implements Listener {

    public function onEnable() {
        $this->getServer()->getPluginManager()->registerEvents($this, $this);
        $this->getLogger()->info("YourPluginName has been enabled!");
    }

    public function onInteract(PlayerInteractEvent $event): void {
        $player = $event->getPlayer();
        $block = $event->getBlock();
        
        // Check if the player clicked a specific block (e.g., sign)
        if ($block->getId() === /* block ID of the sign */) {
            // You can customize the message here
            $player->sendMessage(TextFormat::GREEN . "Welcome to the PocketMine server! You can join using the Java Edition with the IP: your.server.ip");
        }
    }
}
```



```yaml
name: Geyser MCPE 
version: 1.0.0
api: [3.0.0, 3.14.0]
main: Geyser MCPE\Main
description: A plugin to allow Java Edition players to join the PocketMine server.
author: Harsh the owner of vast
```Yeh kaam karega?

```php
<?php

namespace YourPluginNamespace;

use pocketmine\event\Listener;
use pocketmine\event\player\PlayerInteractEvent;
use pocketmine\Player;
use pocketmine\plugin\PluginBase;
use pocketmine\utils\TextFormat;

class Main extends PluginBase implements Listener {

    public function onEnable() {
        $this->getServer()->getPluginManager()->registerEvents($this, $this);
        $this->getLogger()->info("YourPluginName has been enabled!");
    }

    public function onInteract(PlayerInteractEvent $event): void {
        $player = $event->getPlayer();
        $block = $event->getBlock();
        
        // Check if the player clicked a specific block (e.g., sign)
        if ($block->getId() === /* block ID of the sign */) {
            // You can customize the message here
            $player->sendMessage(TextFormat::GREEN . "Welcome to the PocketMine server! You can join using the Java Edition with the IP: your.server.ip");
        }
    }
}
```



```yaml
name: Geyser MCPE 
version: 1.0.0
api: [3.0.0, 3.14.0]
main: Geyser MCPE\Main
description: A plugin to allow Java Edition players to join the PocketMine server.
author: Harsh the owner of vast
```
