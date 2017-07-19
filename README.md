# The Complete 2D Game Artist
Our upcoming Udemy course will teach you all you need to know to create all 2D art assets for video games, from sprites and textures to backgrounds and marketing images.

You're welcome to download, fork or do whatever else legal with all the files!

## How To Use These Files
You can download the latest state of this section, or go to **Commits** then download to get our project as it was at the end of any lecture.

## Section 3 - Animated Sprites - Lecture List AS_GMP
Here are the lectures of the course for this section...

### 1 Bonus Section Introduction
+ Michael Introduces what it coming up in Section 3

### 2 What is Animation
+ Animation is an illusion of motion
+ Images are our Frames
+ The images are shown to us at a regular iterval, called frames per second.

### 3 Setting Up Gimp For Animation
+ Layer Order
+ Previewing the animation
+ Exporting as a GIF

### 4 Deciding On Frame Rate
+ Direct impact on output
+ Yes can be changed later and in game
+ Higher FPS means inserting frames, lowers means cutting them to keep the same animation.

### 5 Layer Animation Parameters
#### Different Layer Options

+ (ms) eg (100ms) : Time that the frame will be showed for.
+ (combine) : Mixes the current frame with the one before it- useful with alpha layers
+ (replace) Replaces the previous frame regardless of any layers having an alpha layer

Note, the order matters as do the brackets and spacing
Recommended Example:  LayerName (100ms)(replace)

### 6 Layer Boundaries

+ Controlling and optimising layer boundaries

### 7 Squash And Stretch
+ We won’t cover them all in this section.
+ Recommended book: Disney Animation: The Illusion of Life
+ Start with squash and stretch and apply that to an animation.

### 8 Making a Bouncing Ball
+ Create a 2 second animation, at 10fps.
+ Ball falling off a ledge and hitting the ground

### 9 Multi Layer Images And Animation
+ You can have a layered animation by using Layer Groups
+ Layer Groups respect previous layer visibilities

### 10 Straight Ahead And Pose To Pose
+ Neither of these techniques are exclusive, mixing them is fine.
+ Picking the appropriate one can be a huge time saver

#### Straight Ahead
+ Very goof for unpredictable animation like flames water and smoke
+ Works because it requires the previous frame for the current one

#### Pose To Pose
+ Gives the most control
+ Get a good idea of the whole scene early on, catching any issues
+ Helps keep consistency throughout an animation
+ Your character or object ends up in the right place

### 11 GIFs And Layer Groups
+ How to organise layergroups so that your animations can be layered
+ Workflow ideas to speed up multi-layer animations

### 12 Slow In And Out
+ How to make animation seem less robotic and more natural
+ Techniques for creating more convincing movement

### 13 Two Different Feeling Animations
+ Steady vs Fast

### 14 Colour Change Over Time
+ Smudge Tool
+ Workflow thoughts
+ Using Opacity
+ Preventing out of memory errors

### 15 Making An Animated Sunset
+ Creating An Animated Sunset

### 16 What Is A Sprite Sheet
#### What Is A Sprite?
+ Sprite: an image that’s integrated into a larger scene
+ Sprite sheet: many of sprites combined in one image
+ Typically associated with 2D animations and GUI elements.
+ A “texture atlas” is essentially the same thing but has a different use
#### What Is Power Of Two?
+ Talking specifically about the pixel x pixel size
+ In brief 2^n, where n is a positive integer
+ Typical ranges in graphics are from 2^0 or 1px to 2^12 which is 4096px
+ The X and Y dimensions can be different
+ Usually not necessary, but recommended to prevent uncontrolled blurring or border issues
+ Not Power Of Two is referred to as NPOT
#### Packing Sprites
+ Go for ease of use and organisation rather than all optimisation.
+ How is your sprite sheet is going to be read?
+ Know your target platform’s maximum texture size
+ Recommend no larger than 2048 x 2048 in general
+ Avoid mixing different sprite sizes

#### Aligning Your Work
+ Power of two image/sprite isn’t necessary.
+ Be aware that NPOT sprites can bleed into one another and have border issues
+ Consider packing sprites into POT cells or with extra padding
+ For sanity recommend sticking with POT sprites and sprite sheets, then everything fits in properly!

### 17 Creating A Basic Sprite Sheet
+ Make your first sprite sheet
+ Share it with us!

### 18 Too Many File Types

#### What Is Your Output?
+ Think of your output first, that filters back to everything else.
+ Where is your image ending up?
+ In Game?
+ On the Web?
+ In Print- Box Art and Manuals?

#### Types Of Images
+ RAW- Uncompressed eg data straight from a camera sensor.
+ Uncompressed (lossless): e.g. BMP, TIFF, TGA...
+ Compressed
+ Lossy: e.g. JPG
+ Lossless: e.g. PNG, GIF*
+ GIF is an 8bit indexed (per frame), has transparency (either ON/OFF)

#### Program Specific Files
+ XCF - Gimps own format, Game Engines and most other programs do NOT understand this file type
+ PSD - Photoshop document

#### When To Convert Image Types
+ Creating all of your images as PNGs will make your project consistent and save space
+ Avoid resaving a JPG, each time you do that you will lose more information
+ Converting JPG to PNG is great if you need to edit
+ If you are having an issue with PNGs
+ If the target destination needs it in another format

### 19a Checking Your Sprite Sheet Works
#### Testing Our Sprite Sheet
+ This lecture is all about testing your work straight away.
+ We’ll search for a tool
+ Use it to test that our sprite sheet behaves as expected.

### 20 Manually Installing GIMP Add Ons
+ How and where to install script and python files
+ Mac installation at 3 mins
+ Challenge at 5 mins

### 21 Add On: Fuse Layers
+ How to use the fuse layer filter we just added
+ The caveats and things to watch out for when using it

### 22 Add On Sprite Sheet
+ How to use the sprite sheet filter we have added
+ Really easy to use, but just makes one long strip, which might be problematic
