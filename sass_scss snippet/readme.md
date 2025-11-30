### **SASS/SCSS-specific snippets** 
Leverage all the powerful features SASS offers beyond regular CSS.

## Key Categories Included:

### 📦 **Variables**
- `svar` - SASS variable
- `svarcol` - Color variables set
- `svartypo` - Typography variables
- `svarspace` - Spacing variables
- `svarbp` - Breakpoint variables

### 🎯 **Nesting & BEM**
- `snest` - Basic nesting
- `sand` - Parent selector (&)
- `sbem` - BEM structure with nesting

### 🔧 **Mixins** (Reusable code blocks)
- `smix` - Basic mixin
- `smixd` - Mixin with default parameters
- `sinc` - Include mixin
- `smixflex` - Flexbox mixin
- `smixfont` - Font mixin
- `smixshadow` - Box shadow mixin
- `smixtrans` - Transition mixin
- `smixbr` - Border radius mixin
- `smixcenter` - Absolute center mixin
- `smixresp` - Responsive breakpoint mixin
- `smixtrunc` - Text truncate mixin
- `smixsize` - Size (width/height) mixin
- `smixpseudo` - Pseudo element mixin

### 🎨 **Functions** (Return values)
- `sfunc` - Basic function
- `sfuncrem` - Convert px to rem
- `sfuncem` - Convert px to em
- `sfunclight` - Lighten color
- `sfuncdark` - Darken color
- `sfuncmix` - Mix colors

### 🔄 **Extends & Placeholders**
- `sext` - Extend class
- `splace` - Placeholder selector
- `sextp` - Extend placeholder

### 🎛️ **Control Directives**
- `sif`, `sifelse`, `sifelseif` - Conditional statements
- `sfor` - For loop
- `seach` - Each loop
- `swhile` - While loop

### 🗺️ **Maps** (Key-value pairs)
- `smap` - Create map
- `smapget` - Get value from map
- `smaphas` - Check if key exists
- `smapmerge` - Merge maps
- `smapeach` - Iterate over map
- `smapcolor` - Color map template
- `smapspace` - Spacing map template

### 📋 **Lists**
- `slist` - Create list
- `slistlen` - List length
- `slistnth` - Get nth item
- `slistapp` - Append to list

### 📁 **Modules & Imports**
- `simp` - Import (old syntax)
- `suse` - Use (new module system)
- `sforward` - Forward module

### 📱 **Media Queries**
- `smq` - Basic media query
- `smqvar` - Media query with variable
- `sresp` - Responsive mixin include

### 🔍 **Debugging**
- `sdebug` - Debug statement
- `swarn` - Warning
- `serror` - Error
- `scont` - Content directive

### 🔤 **Interpolation**
- `sinterp` - Variable interpolation
- `sdynclass` - Dynamic class names

### 🎁 **Advanced Patterns**
- `sbtnvar` - Generate button variants
- `sutil` - Generate spacing utilities (margin/padding)
- `sgrid` - Complete grid system generator
- `stheme` - Theme system with theming function
- `szindex` - Z-index management
- `stypo` - Typography scale generator
- `sreset` - SASS reset

## Installation:
1. Open VSCode
2. Press `Ctrl+Shift+P` / `Cmd+Shift+P`
3. Type "Configure User Snippets"
4. Select `scss.json` (or `sass.json` for indented syntax)
5. Paste the content

## Pro Tips:
- Use **mixins** when you need to include styles (with `@include`)
- Use **functions** when you need to return calculated values
- Use **placeholders** (`%`) for styles you want to extend but not output by themselves
- Use **maps** for organizing related values (colors, spacing, breakpoints)
- Use **loops** to generate utility classes automatically
- The new `@use` and `@forward` are preferred over `@import` for better module organization

These snippets will supercharge your SASS workflow and help you write more maintainable.

 DRY (Don't Repeat Yourself) stylesheets! 🎨✨