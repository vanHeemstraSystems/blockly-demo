# 200 - Load the Code

Once you've gotten the code, there are several ways you can access it from your code.

## Script tags

```
<!-- Load Blockly core -->
<script src="./my-lib-directory/blockly/blockly_compressed.js"></script>
<!-- Load the default blocks -->
<script src="./my-lib-directory/blockly/blocks_compressed.js"></script>
<!-- Load a generator -->
<script src="./my-lib-directory/blockly/javascript_compressed.js"></script>
<!-- Load a message file -->
<script src="./my-lib-directory/blockly/msg/en.js"></script>
```

When using script tags, you can access imports from the global namespace:

```
// Access Blockly.
Blockly.thing;

// Access the default blocks.
Blockly.libraryBlocks['block_type'];

// Access the generator.
javascript.javascriptGenerator;
```

**Note**: When using script tags you cannot have multiple message files because the messages get applied directly to the Blockly.Msg array.

## Imports



MORE