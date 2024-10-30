# 200 - Toolbox

The toolbox contains the blocks that you use to program. The blocks can be dragged onto the workspace.

For more information about what a toolbox looks like, see the [visual glossary](https://developers.google.com/blockly/guides/get-started/workspace-anatomy#toolbox).

## 100 - Basic definition

A toolbox definition specifies what blocks get included in the toolbox, and in what order. Most of the look and style of your toolbox is specified in other ways.

We recommend defining your toolbox using JSON.

This code snippet defines a flyout toolbox with two blocks:

```
const toolbox = {
  // There are two kinds of toolboxes. The simpler one is a flyout toolbox.
  kind: 'flyoutToolbox',
  // The contents is the blocks and other items that exist in your toolbox.
  contents: [
    {
      kind: 'block',
      type: 'controls_if'
    },
    {
      kind: 'block',
      type: 'controls_whileUntil'
    }
    // You can add more blocks to this array.
  ]
};

// The toolbox gets passed to the configuration struct during injection.
const workspace = Blockly.inject('blocklyDiv', {toolbox: toolbox});
```

![image](https://github.com/user-attachments/assets/35451bb7-5987-47b7-8a50-83e935d89f01)

For more information about how to define and configure your toolbox, see [Toolbox overview](https://developers.google.com/blockly/guides/configure/web/toolbox).

For more information about injection, see [Workspace creation](https://developers.google.com/blockly/guides/get-started/workspace-creation).