# 300 - Blocks

Based on https://developers.google.com/blockly/guides/get-started/blocks

Blocks are what you use to program. They represent expressions and statements in text-based programming languages.

For more information about blocks and what the parts of them look like, see the [visual glossary](https://developers.google.com/blockly/guides/get-started/workspace-anatomy#blocks).

## 100 - Block Definition

A block definition specifies the puzzle piece connections and fields on your block. Most of the look and style of your blocks is specified in other ways. The string (usually code) your block gets converted to is defined as a [block-code generator](https://developers.google.com/blockly/guides/get-started/code-generation).

The easiest way to define simple blocks is using JSON.

This code snippet defines a "move forward" block with next and previous connections, and one field for the distance.

```javascript
// Create the definition.
const definitions = Blockly.createBlockDefinitionsFromJsonArray([
  {
    // The type is like the "class name" for your block. It is used to construct
    // new instances. E.g. in the toolbox.
    type: 'my_custom_block',
    // The message defines the basic text of your block, and where inputs or
    // fields will be inserted.
    message0: 'move forward %1',
    args0: [
      // Each arg is associated with a %# in the message.
      // This one gets substituted for %1.
      {
        // The type specifies the kind of input or field to be inserted.
        type: 'field_number',
        // The name allows you to reference the field and get its value.
        name: 'FIELD_NAME',
      }
    ],
    // Adds an untyped previous connection to the top of the block.
    previousStatement: null,
    // Adds an untyped next connection to the bottom of the block.
    nextStatement: null,
  }
]);

// Register the definition.
Blockly.defineBlocks(definitions);
```

![image](https://github.com/user-attachments/assets/94c728ec-87cf-4661-a89e-2dd3b10442be)

For more information about how to define your blocks, see [Define blocks](https://developers.google.com/blockly/guides/create-custom-blocks/define-blocks).

For information about how to include your block in your toolbox, see [Toolbox overview](https://developers.google.com/blockly/guides/configure/web/toolbox).
