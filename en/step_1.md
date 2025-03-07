### Scratch Style Guide

### 1. Settings and Setup
- Use the High Contrast Colour mode for improved readability.
- Always give the project a name
![project name text entry](images/project-name.png)

### 2. Editor Terminology
- Follow provided naming conventions for consistency.
![labeled scratch editor](images/scratch-interface.png)

### 3. Naming Conventions
- **Sprites and Backdrops:** Use descriptive names reflecting their role or appearance. Rename defaults like "sprite1" to "hero" or "player".
- **Case:** Use lower case for all names. Separate words with spaces rather than underscores or capital letters.
- **Variables and Lists:** Choose clear and descriptive names, such as "score" or "enemy list".
```blocks3
change [cat score v] by (1) 
```

### 2. Organisation of Code
- **Scripts Arrangement:** Organise scripts logically, grouping related blocks together to enhance readability and debugging.
- **Use of Comments:** Utilise Scratch's built-in comments on blocks when necessary, particularly in starter projects or instructions, to provide additional clarity.

![scratch block with menu to add comment](images/add-comment.png)

```blocks3
go to x:(0) y:(0) // move to middle of stage
```

### 3. Event Handling
- **Single Event Listener:** Prefer using one `when green flag clicked`{:class="block3events"} block per sprite to initiate actions. Manage multiple behaviours within this script using control blocks.
- **Broadcasting Messages:** Utilise broadcasts to communicate clearly between sprites. Name broadcasts meaningfully.

### 3. Control Structures
- **Loops:** Use `repeat`{:class="block3control"} or `forever`{:class="block3control"} loops appropriately. Ensure loops have clear exit conditions to prevent infinite loops unintentionally.
- **Conditional Statements:** Use `if`{:class="block3control"} and `if-else`{:class="block3control" blocks for clear and simple decision-making logic.

### 4. Motion and Positioning
- **Coordinate System:** Be mindful of Scratch’s coordinate system, where `0, 0`{:class="block3motion"} is the centre. Clearly position sprites using `x`{:class="block3motion"} and `y`{:class="block3motion"} coordinates.
- **Rotation Style:** Set rotation styles appropriately using code (`don't rotate`{:class="block3motion"},`left-right`{:class="block3motion"}, or `all around`{:class="block3motion"}) for expected behaviour during motion.

```blocks3
set rotation style [left-right v]
```

### 5. Looks and Sounds
- **Costume Naming:** Clearly name costumes based on their purpose or action, like "walking 1" or "jumping pose".
- **Sound Management:** Name sounds based on function (e.g., "jump sound", "background music"). Keep audio clips concise to maintain performance.

### 6. Variables and Lists
- **Scope:** Determine appropriate scope (sprite-specific or global) based on usage context.
- **Initialisation:** Always initialise variables at the beginning of scripts to ensure they have defined initial values.

```blocks3
set [player score v] to (0)
```

### 6. My Blocks
- **Purpose:** Use My Blocks only for repetitive code or complex functionalities, promoting modularity. Avoid their use unnecessarily.
- **Naming:** Name My Blocks descriptively, clearly indicating their function, such as "move to start position" or "check collision".

### 7. Instructional style
- **Highlighting** Highlight text that refers to a block using the colour associated with that block. (e.g) `go to x:100 y:50`{:class="block3motion"}, `delete this clone`{:class="block3control"}
- **Scratchblocks** Use [Scratchblocks](https://scratchblocks.github.io/#?style=scratch3&script=) to create PNG code blocks for online use or SVG code blocks for printed use. Save the code used for easy maintenance of the instructions. (Scratchblocks can be saved as a [URL](https://scratchblocks.github.io/#?style=scratch3&script=when%20flag%20clicked%0Ago%20to%20x%3A(0)%20y%3A(0)%0Aturn%20cw%20(15)%20degrees%0Asay%20%5Bhello%5D%0A)