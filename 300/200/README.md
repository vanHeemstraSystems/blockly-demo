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

**Note**: Using imports of our package targets requires you to be using a bundler (like webpack), since Blockly is packaged as a UMD, rather than an ESM.

```
// Import Blockly core.
import * as Blockly from 'blockly/core';
// Import the default blocks.
import * as libraryBlocks from 'blockly/blocks';
// Import a generator.
import {javascriptGenerator} from 'blockly/javascript';
// Import a message file.
import * as En from 'blockly/msg/en';
```

When you import the message files, you also need to apply them.

```
Blockly.setLocale(En);
```

## Requires

```
// Require Blockly core.
const Blockly = require('blockly/core');
// Require the default blocks.
const libraryBlocks = require('blockly/blocks');
// Require a generator.
const {javascriptGenerator} =  require('blockly/javascript');
// Require a message file.
const En = require('blockly/msg/en');
```

When you require the message files, you also need to apply them.

```
Blockly.setLocale(En);
```