# Glossary

Blockly has a lot of vocabulary for its different visual components. This document breaks down some of the most important ones you need to know to get started with Blockly.

## Workspace

The workspace is the highest level component in Blockly. It contains all of the other components. This is where you do the work of programming!

![image](https://github.com/user-attachments/assets/2ced8c73-2d14-4a8a-aff3-48af426f7396)


## Toolbox

The [toolbox](https://developers.google.com/blockly/guides/configure/web/toolbox) contains the blocks that you use to program. The blocks can be dragged onto the workspace.

There are two main types of toolboxes, flyout toolboxes and category toolboxes. These can both be displayed vertically and horizontally.

### Flyout toolbox

Flyout toolboxes (aka simple toolboxes) have one set of blocks which is displayed at all times.

![image](https://github.com/user-attachments/assets/d311a520-914d-47ab-a13b-ce0ab75923d0)

### Category toolbox

Category toolboxes have multiple sets of blocks.

![image](https://github.com/user-attachments/assets/266027c7-8530-4b1e-bc17-d15e74866c18)

If you click a category item it opens a flyout that displays the blocks in the category.

![image](https://github.com/user-attachments/assets/cfb592b1-cc85-4e5e-bc96-6da902cb4cc4)

## Trashcan

The trashcan lets you delete blocks by dragging and dropping them. You can also click the trashcan to open a flyout containing the blocks you've deleted so you can get them back.

![image](https://github.com/user-attachments/assets/9e6ae8dd-9b9e-4e52-96a3-194a6b8ffd8b)

## Zoom controls

The [zoom controls](https://developers.google.com/blockly/guides/configure/web/zoom) zoom the workspace in and out when you click them.

![image](https://github.com/user-attachments/assets/e54582c1-8d7a-485b-bb00-94df2220dfda)

## Context menu

The [context menu](https://developers.google.com/blockly/guides/configure/web/context-menus) appears when you right-click or long-press on certain elements of the workspace (for example, the workspace background, or blocks). It displays a list of actions you can perform on that element.

![image](https://github.com/user-attachments/assets/5fc62ce9-2253-4f91-b419-1c7e60f282a6)

## Blocks

[Blocks](https://developers.google.com/blockly/guides/create-custom-blocks/define-blocks) are what you use to program. They represent expressions and statements in text-based programming languages.

![image](https://github.com/user-attachments/assets/665811c0-2549-434e-83ba-b3a48b65fd29)

### Block stack

A block stack is any collection of connected blocks. They could be connected horizontally or vertically.

![image](https://github.com/user-attachments/assets/e1f7c922-80d8-4c2b-8908-76a6630eaad3)

### Shadow block

A shadow block is an editable but non-movable block connected to another block. You can drag non-shadow blocks on top of shadow blocks to overwrite them.

![image](https://github.com/user-attachments/assets/7ff8e441-766b-465c-9f51-934f47c527a9)

### Insertion marker

An insertion marker is a preview of where a stack of blocks will be connected if it is dropped. It looks like a grey version of a block.

![image](https://github.com/user-attachments/assets/032fa8a9-e2ff-471c-86fb-ff94892ffa4d)

## Block parts

Blocks have several different parts that you can edit and interact with to program.

### Inputs

An [input](https://developers.google.com/blockly/guides/create-custom-blocks/inputs/overview#inputs) usually represents a row in a block.

| Input | Image |
| --- | --- |
| Dummy | <img src="https://github.com/user-attachments/assets/760bc248-ef94-4891-8c67-93f36f3d4bd2" alt="dummy" style="width:45px;"/> |
| Value | <img src="https://github.com/user-attachments/assets/8d993675-2eae-4807-9516-15d35f644e61" alt="value" style="width:45px;"/> |
| Statement | <img src="https://github.com/user-attachments/assets/8dd362a6-8e46-4d80-a352-471de91c5354" alt="statement" style="width:45px;"/> |

### Connections

A [connection](https://developers.google.com/blockly/guides/create-custom-blocks/inputs/overview#connections) is a place on a block other blocks can connect to.

| Connection | Image |
| --- | --- |
| Output | <img src="https://github.com/user-attachments/assets/2a32af27-2d09-4921-95e7-7164964223e2" alt="output" style="width:45px;"/> |
| Input | <img src="https://github.com/user-attachments/assets/e9f2b70c-a307-4368-bcdf-f3c4f600a535" alt="input" style="width:45px;"/> |
| Previous| <img src="https://github.com/user-attachments/assets/37d83a7f-4fb6-427e-8da0-dda7835cce95" alt="previous" style="width:45px;"/> |
| Next | <img src="https://github.com/user-attachments/assets/58d8654c-77dc-40fa-bb30-3196692594f0" alt="next" style="width:45px;"/> |

### Fields

A [field](https://developers.google.com/blockly/guides/create-custom-blocks/fields/overview) is a visual element that lives on a block. It could be editable (like a text input), or only informational (like a label). A field is always contained by an input.

![image](https://github.com/user-attachments/assets/48068fba-1e56-42f6-b2c0-04e3caaf6f33)

### Icons

An icon is a visual element that lives on a block. They always live in the top-start corner of the block, and they often create bubbles.

![image](https://github.com/user-attachments/assets/9a29f796-7424-449f-8497-aceecad9f79f)

![image](https://github.com/user-attachments/assets/9f7618ea-8834-49a1-bcba-c83775723026)
