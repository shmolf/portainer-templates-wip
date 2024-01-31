# Forking from my other repo
```sh
git clone git@github.com:shmolf/portainer-templates.git portainer-templates-wip
cd portainter-templates-wip
# Now, set the upstream for this WIP project
git remote add upstream https://github.com/shmolf/portainer-templates.git
# Now, set the new origin URL. This should match the URL of fresh Repo you'll need to create in Github.
git remote set-url origin https://github.com/shmolf/portainer-templates-wip.git
```

The purpose of this, is that Portainer doesn't allow references to branches of a repo.
So all changes must be merged with the `main` branch before being able to perform an end-to-end test.

This project was created to consume all the trash PRs and changes, and port over the successfull changes to the main repo.

# App Templates

This repository hosts the official templates (**'Apps Templates'**) definitions for Portainer.

For more information about the template definition format and how to deploy your own templates, see the [relevant documentation section](https://documentation.portainer.io/v2.0/templates/deploy_stack/).
https://docs.portainer.io/advanced/app-templates/format


I highly recommend using [Lissy93's templates](https://github.com/Lissy93/portainer-templates).
But if you want to use this repo's templates, you'll want to reference the following URL in the Portainer template settings:
```
https://raw.githubusercontent.com/shmolf/portainer-templates-wip/main/templates-2.0.json
```

## Category List
<!--
Acquired by pasting the template JSON into browser DevTools, then running:
```js
console.log('- ' + Array.from(new Set(json.templates.flatMap((t) => t.categories))).sort().join('\n- '))
```
-->
- backup
- docker
- games
- graphic design
- pdf
- photos
- tools

## Application List
<!--
Acquired by pasting the template JSON into browser DevTools, then running:
```js
console.log('- ' + Array.from(new Set(json.templates.map((t) => t.title))).sort().join('\n- '))
```
-->
- Immich
- Penpot (http)
- Stirling PDF
- Terraria Server
- Watchtower
