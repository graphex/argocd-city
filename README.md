ArgoCD-City
===========

This is just a demo repo showing an example of a wrapped chart. I follow this pattern when using ArgoCD to deploy
everything in my cluster, including ArgoCD itself. I like this pattern because it provides a place to define my own
values file and add my own templates, if desired. It also works well with Jetbrains IDEs which have plugins that support
showing me the `charts/<chartname>-<chartversion>.tgz` file, so there is a reference values.yaml file to go from. For
the better-made charts, Jetbrains IDE even does code completion and live linting for values.yaml.

Sometimes it is a pain trying to figure out what URL to put in Chart.yaml `dependencies.repository` or what versions exist,
but the Jetbrains tooling also helps with this if the repository is loaded it will show you all the versions in the index.yaml
of the repository so you don't have to manually look through them or hope docs are updated.

