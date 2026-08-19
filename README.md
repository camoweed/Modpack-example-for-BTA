# BTA! Example Modpack 

Combines [packwiz](https://packwiz.infra.link/) and [unsup](https://git.sleeping.town/exa/unsup) to provide a single self-updating instance which can be managed from a git repository.

## How to modpack

- Follow the installation tutorial for packwiz: https://packwiz.infra.link/installation/
- Click "use this template".
- Give it a creative name. Its fine if you set it to private for now.
- Clone the repository. I use github desktop but any method should work fine.
- It does not have to be a github repository. Local git repos are fine too, as long as its publically accessible.

## Creating the instance

- Download and extract the instance in [releases](https://github.com/camoweed/Modpack-example-for-BTA/releases).
- Change the instance icon and instance.cfg to match your use case.

unsup uses a launch argument to function, so make sure that remains intact.

- In the /instance/minecraft/ folder edit "source" in ``unsup.ini`` to point at your pack.toml
- You can create your own "branding" icon at this website: https://qoi.y2k.diy/ (check convert to Base64)
- In order for the instance to see the pack.toml it must be publically accesible.
- Once you have set the source, branding, and instance confifguration you can add the contents of the /instance/ folder to a zip.

## Managing the pack

- See full reference for packwiz: https://packwiz.infra.link/reference/commands/packwiz/
- Open the /pack/ folder in a terminal and use

``packwiz url add "Name" <URL>``

then

``packwiz refresh``
- You can use this to add a mod, texturepack, really any file thats on the internet.
- Now that you have made changes locally and refreshed packwiz, you can add and commit your changes.