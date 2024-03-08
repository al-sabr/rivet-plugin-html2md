<h1 align="center"><img src="https://rivet.ironcladapp.com/img/logo-banner-wide.png" alt="Rivet Logo"></h1>

# Converts HTML files to Markdown

## Using the plugin

### In Rivet

To use this plugin in Rivet:

1. Navigate to the Project tab in the left sidebar. You will see a + button next to `Plugins`,
   click it to open the Add Plugin modal.
2. Chose the `HTML to Markdown` plugin and click add
3. There is a new group `Documents to Markdown`and a new `HTML to Markdown` node
4. Just chose a directory or activate the input and give it a path to your pdf file

### In Code

Load your plugin and Rivet into your application:

```ts
import * as Rivet from "@ironclad/rivet-core";
import html2md from "rivet-plugin-html2md";
```

Register your plugin with Rivet be using the `globalRivetNodeRegistry` or creating a new `NodeRegistration` and registering with that:

```ts
Rivet.globalRivetNodeRegistry.registerPlugin(html2md(Rivet));
```
