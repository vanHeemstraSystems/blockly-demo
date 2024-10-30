# 100 - Workspace Creation

A Blockly workspace is the highest level component of Blockly. It is the UI that you use to program with blocks.

For more information about the workspace and its subcomponents, see the [visual glossary](https://developers.google.com/blockly/guides/get-started/workspace-anatomy).

## 100 - Injection div

A Blockly workspace must be injected into a ```<div>```, called the "injection div".

The injection div can be sized [statically](https://google.github.io/blockly-samples/examples/fixed-demo/index.html) or [dynamically](https://google.github.io/blockly-samples/examples/resizable-demo/index.html). Blockly elements within the div update their size when the window resizes.

The following code snippet shows the HTML for a statically sized injection div:

```
<div id="blocklyDiv" style="height: 480px; width: 600px;"></div>
```

## 200 - Injection

Injection creates all of the HTML sub-elements that make up the UI of a workspace. It also does all of the initialization needed to get the workspace ready for use.

The injection function can take in the ID of the injection div, or the injection div itself:

```
// Passes the ID.
const workspace = Blockly.inject('blocklyDiv', { /* config */ });

// Passes the injection div.
const workspace = Blockly.inject(
    document.getElementById('blocklyDiv'), { /* config */ });
```

## 300 - Configuration

The workspace can be configured with numerous options (such as layout and style) during injection.

For more information about configuration options, see [Configuration options](https://developers.google.com/blockly/guides/configure/web/configuration_struct).