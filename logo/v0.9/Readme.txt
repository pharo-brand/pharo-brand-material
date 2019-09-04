Pharo Logo SVG
==============

HowTo
-----

- Download pharo-logos.zip from http://www.pharo-project.org/pharo-download/media-files
- Import pharo-0.8.1.pdf into Inkscape (vector graphic program)
- Ungroup all SVG-elements + Recalculate relative to absolute coordinates (it's a little bit tricky in Inkscape)
- Split SVG-elements if necessary (Pharo letter glare effekt)
- (Re-)Group associated parts
- Replace all bitmap-parts with vektor only equivalents, in particular shadow
- Reorganice references between shapes and color-gradients or filters, eleminate duplications
- Shorten too long coordinate system numbers e.g. 25.772936550317932 --> 25.77 with https://petercollingridge.appspot.com/svg_optimiser
- Name SVG-elements with "speaking" names
- Export from Inkscape without Inkscape-specific XML-elements/attributes
- Finishing with common Texteditor (UTF-8 capable)


Nested composition
------------------

- Pharo_Logo contains Pharo_Icon which contains Pharo_Beacon (beacon is used as favicon for website)

<g id="logo">
	...
	<g id="icon">
		...
		<g id="beacon">
			...
		</g>
	</g>
</g>


Version
-------

- 2013-04-29 Pharo_Logo_v0.9.svg
	- "water-splashes" and "flare" of the icon-part are coming out of the stylized "o" (it's a minimal intervention)
	- for use as Pharo_Icon_v0.9.svg
		- set "background"'s fill-opacity:0 --> fill-opacity:1
		- set "flare"'s opacity:0.5 --> opacity:0.7 for better contrast




