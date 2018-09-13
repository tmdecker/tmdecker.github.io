---
layout: post
title: Adobe Illustrator Color Swatches for Data Science
author: Tim
---

I enjoy annotating my plots and putting them together to a big figure in Adobe Illustrator. However, Illustrator lacks some key color palettes often needed in data science. Luckily, we can built our own color swatches, how palettes are called in Illustrator. I'll show you how to prepare your own color swatch by example of the Otabe & Ito colorblind palette (see [http://jfly.iam.u-tokyo.ac.jp/color/](http://jfly.iam.u-tokyo.ac.jp/color/)).

![otabeitopalette]({{ "assets/img/otabeito.png" | absolute_url }})

<br><br>

## General color swatch management in Illustrator

You'll find the default color swatches in the *Swatches Panel* (Window -> Swatches):

![swatches panel]({{ "assets/img/swatches_panel.png" | absolute_url }})

There are more predefined swatches in the Swatch libraries. Simple click the library button on the lower left of the Swatches Panel and select the library you want. This is also the place were you will find the user-defined swatches or swatches that you imported as .ase or .ai file.   

   

### Change default swatches by using templates (The Easy Way):

1. Open a new file.

2. Drag&drop your favourite swatches into the Swatches Panel.

3. Save the file as template.

4. Always open a new file from this template if you wish to use your own default color swatches.

### Change default swatches by creating a new profile (The Hard Way):

1. Follow steps 1 and 2 of from above.

2. Save the file as .ai file in "/Applications/Adobe Illustrator CC 2018/Support Files/New Document Profiles/en_US/YouNewProfile.ai". *Access to this folder may be denied when saving directly from Illustrator. A workaround would be to save the file in any other location e.g. your Desktop and then drag&drop it to the desired folder.*

3. In Illustrator navigate to Preferences -> General and make sure "Use legacy File New interface" is checked.

4. When you open a new file, you can now select YourNewProfile from the dropdown menu.

   <br><br>

## Build your own color swatch

Our goal is, to save the color palette as an .ase file:

1. Delete the default colors in the Illustrator swatches panel (don't worry, they'll be back when you open a new file). Simply select the colors and hit the 'Delete Swatches' button.   

2. Let's also create a new color group.   

3. For this example we first need to look up the RGB values of the colors we want to add to the colorblind pallet:

> ​	Blue: 0,114,178
>
> ​	Vermillion: 213,94,0
>
> ​	Bluish Green: 0,158,115
>
> ​	Reddish Purple: 204,121,167
>
> ​	Orange: 230,159,0
>
> ​	Yellow: 240,288,66
>
> ​	Black: 0,0,0

4. Open the Color Picker by double-clicking on the current fill color.

5. Enter the RGB values of the first color.

6. Drag-and-drop the new fill color into the new color group we just created in the swatches panel and repeat this for all colors.

7. Open the options menu of the panel and select 'Save swatches library as ASE...'.

You may want to save an additional copy in a folder other than the default one, in case you want easy access to the file. If saved in the default folder, the new palette will be available in the Swatch libraries -> user defined.

<br><br>

## Download Brewer and colorblind palettes

If you don't want to build your own palettes, you can also download .ase files and copy them into the Illustrator Swatches folder (/Applications/Adobe Illustrator CC 2018/Presets/en_US/Swatches).

Download the Okabe & Ito colorblind palette here: [Okabe-Ito-Colorblind.ase]({{ "assets/download/Otabe-Ito-Colorblind.ase" | absolute_url}})

You should also get the collection of Brewer palettes, as they are commonly used in data science. Find the .ase and .ai files on Martin Skrywinski's website: [http://mkweb.bcgsc.ca/brewer/]( http://mkweb.bcgsc.ca/brewer/)

![brewerswatches]({{ "assets/img/brewer-swatches-subset.png" | absolute_url }}) 

*A screenshot of Martin Skrywinski's article on Brewer palettes  ([http://mkweb.bcgsc.ca/brewer/](http://mkweb.bcgsc.ca/brewer/)) that shows a subset of Brewer swatches.*