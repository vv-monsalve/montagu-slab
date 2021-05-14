## Fontbakery report

Fontbakery version: 0.7.35

<details>
<summary><b>[8] MontaguSlab16pt-Bold.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Ensure Stylistic Sets have description.</summary>

* [com.google.fonts/check/stylisticset_description](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/stylisticset_description)
<pre>--- Rationale ---
Stylistic sets must provide description text. Programs such as InDesign,
TextEdit and Inkscape use that info to display to the users so that they know
what a given stylistic set offers.</pre>

* 🔥 **FAIL** The stylistic set ss01 lacks a description string on the 'name' table. [code: missing-description]

</details>
<details>
<summary>⚠ <b>WARN:</b> Stricter unitsPerEm criteria for Google Fonts. </summary>

* [com.google.fonts/check/unitsperem_strict](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/unitsperem_strict)
<pre>--- Rationale ---
Even though the OpenType spec allows unitsPerEm to be any value between 16 and
16384, the Google Fonts project aims at a narrower set of reasonable values.
The spec suggests usage of powers of two in order to get some performance
improvements on legacy renderers, so those values are acceptable.
But values of 500 or 1000 are also acceptable, with the added benefit that it
makes upm math easier for designers, while the performance hit of not using a
power of two is most likely negligible nowadays.
Additionally, values above 2048 would likely result in unreasonable filesize
increases.</pre>

* ⚠ **WARN** Font em size (unitsPerEm) is 2200 which may be too large (causing filesize bloat), unless you are sure that the detail level in this font requires that much precision. [code: large-value]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: ampersand	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: two	Contours detected: 2	Expected: 1
Glyph name: less	Contours detected: 0	Expected: 1
Glyph name: greater	Contours detected: 0	Expected: 1
Glyph name: at	Contours detected: 0	Expected: 2
Glyph name: Q	Contours detected: 3	Expected: 2
Glyph name: asciicircum	Contours detected: 0	Expected: 1
Glyph name: asciitilde	Contours detected: 0	Expected: 1
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
Glyph name: currency	Contours detected: 0	Expected: 2
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: copyright	Contours detected: 0	Expected: 3
Glyph name: logicalnot	Contours detected: 0	Expected: 1
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: uni00B2	Contours detected: 2	Expected: 1
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
Glyph name: uni2082	Contours detected: 2	Expected: 1
Glyph name: lira	Contours detected: 0	Expected: 1
Glyph name: uni20AD	Contours detected: 0	Expected: 1
Glyph name: uni20BA	Contours detected: 0	Expected: 1
Glyph name: uni20BC	Contours detected: 0	Expected: 1
Glyph name: approxequal	Contours detected: 0	Expected: 2
Glyph name: notequal	Contours detected: 0	Expected: 1
Glyph name: lessequal	Contours detected: 0	Expected: 2
Glyph name: greaterequal	Contours detected: 0	Expected: 2
Glyph name: uni27E8	Contours detected: 0	Expected: 1
Glyph name: uni27E9	Contours detected: 0	Expected: 1
Glyph name: Q	Contours detected: 3	Expected: 2
Glyph name: ampersand	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: approxequal	Contours detected: 0	Expected: 2
Glyph name: asciicircum	Contours detected: 0	Expected: 1
Glyph name: asciitilde	Contours detected: 0	Expected: 1
Glyph name: at	Contours detected: 0	Expected: 2
Glyph name: copyright	Contours detected: 0	Expected: 3
Glyph name: currency	Contours detected: 0	Expected: 2
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: greater	Contours detected: 0	Expected: 1
Glyph name: greaterequal	Contours detected: 0	Expected: 2
Glyph name: less	Contours detected: 0	Expected: 1
Glyph name: lessequal	Contours detected: 0	Expected: 2
Glyph name: lira	Contours detected: 0	Expected: 1
Glyph name: logicalnot	Contours detected: 0	Expected: 1
Glyph name: notequal	Contours detected: 0	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
Glyph name: two	Contours detected: 2	Expected: 1
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: uni20AD	Contours detected: 0	Expected: 1
Glyph name: uni20BA	Contours detected: 0	Expected: 1
Glyph name: uni20BC	Contours detected: 0	Expected: 1
Glyph name: uni27E8	Contours detected: 0	Expected: 1
Glyph name: uni27E9	Contours detected: 0	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking unitsPerEm value is reasonable.</summary>

* [com.google.fonts/check/unitsperem](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/head.html#com.google.fonts/check/unitsperem)
<pre>--- Rationale ---
According to the OpenType spec:
The value of unitsPerEm at the head table must be a value between 16 and 16384.
Any value in this range is valid.
In fonts that have TrueType outlines, a power of 2 is recommended as this allows
performance optimizations in some rasterizers.
But 1000 is a commonly used value. And 2000 may become increasingly more common
on Variable Fonts.</pre>

* ⚠ **WARN** In order to optimize performance on some legacy renderers, the value of unitsPerEm at the head table should idealy be a power of between 16 to 16384. And values of 1000 and 2000 are also common and may be just fine as well. But we got 2200 instead. [code: suboptimal]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* Eng: X=1308.0,Y=-2.0 (should be at baseline 0?)
	* one.numr: X=301.0,Y=1498.0 (should be at cap-height 1500?)
	* uni00B9: X=301.0,Y=1498.0 (should be at cap-height 1500?)
	* onehalf: X=301.0,Y=1498.0 (should be at cap-height 1500?)
	* onequarter: X=301.0,Y=1498.0 (should be at cap-height 1500?)
	* questiondown: X=436.0,Y=-2.0 (should be at baseline 0?)
	* colonmonetary: X=607.0,Y=-1.0 (should be at baseline 0?)
	* dollar: X=902.0,Y=1499.0 (should be at cap-height 1500?) and uni20B2: X=1104.0,Y=-2.0 (should be at baseline 0?) [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* R: L<<1099.0,696.0>--<1065.0,696.0>>/B<<1065.0,696.0>-<1196.0,677.0>-<1250.5,591.5>> = 8.252529047136063
	* Racute: L<<1099.0,696.0>--<1065.0,696.0>>/B<<1065.0,696.0>-<1196.0,677.0>-<1250.5,591.5>> = 8.252529047136063
	* Rcaron: L<<1099.0,696.0>--<1065.0,696.0>>/B<<1065.0,696.0>-<1196.0,677.0>-<1250.5,591.5>> = 8.252529047136063
	* braceleft.case: B<<544.0,826.0>-<479.0,755.0>-<330.0,750.0>>/B<<330.0,750.0>-<479.0,745.0>-<544.0,674.0>> = 3.843911917862876
	* braceleft: B<<598.0,750.5>-<533.0,648.0>-<340.0,640.0>>/B<<340.0,640.0>-<533.0,633.0>-<598.0,530.0>> = 4.450770567399401
	* braceright.case: B<<318.5,674.0>-<384.0,745.0>-<532.0,750.0>>/B<<532.0,750.0>-<384.0,755.0>-<318.5,826.0>> = 3.869864619105556
	* braceright: B<<364.0,530.0>-<429.0,633.0>-<622.0,640.0>>/B<<622.0,640.0>-<429.0,648.0>-<364.0,750.5>> = 4.450770567399401
	* eng: L<<591.0,1160.0>--<591.0,900.0>>/B<<591.0,900.0>-<620.0,1030.0>-<711.5,1104.5>> = 12.575465499744425
	* eth: B<<813.5,1055.5>-<906.0,1005.0>-<956.0,886.0>>/B<<956.0,886.0>-<939.0,993.0>-<908.0,1083.0>> = 13.762977891069923
	* m: L<<585.0,1160.0>--<585.0,891.0>>/B<<585.0,891.0>-<609.0,1025.0>-<692.5,1101.5>> = 10.154266580200266 and 36 more. [code: found-jaggy-segments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * k: L<<222.0,210.0>--<223.0,1370.0>>
 * k: L<<623.0,1580.0>--<622.0,633.0>>
 * uni0137: L<<222.0,210.0>--<223.0,1370.0>> and uni0137: L<<623.0,1580.0>--<622.0,633.0>> [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[9] MontaguSlab16pt-ExtraLight.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Ensure Stylistic Sets have description.</summary>

* [com.google.fonts/check/stylisticset_description](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/stylisticset_description)
<pre>--- Rationale ---
Stylistic sets must provide description text. Programs such as InDesign,
TextEdit and Inkscape use that info to display to the users so that they know
what a given stylistic set offers.</pre>

* 🔥 **FAIL** The stylistic set ss01 lacks a description string on the 'name' table. [code: missing-description]

</details>
<details>
<summary>⚠ <b>WARN:</b> Stricter unitsPerEm criteria for Google Fonts. </summary>

* [com.google.fonts/check/unitsperem_strict](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/unitsperem_strict)
<pre>--- Rationale ---
Even though the OpenType spec allows unitsPerEm to be any value between 16 and
16384, the Google Fonts project aims at a narrower set of reasonable values.
The spec suggests usage of powers of two in order to get some performance
improvements on legacy renderers, so those values are acceptable.
But values of 500 or 1000 are also acceptable, with the added benefit that it
makes upm math easier for designers, while the performance hit of not using a
power of two is most likely negligible nowadays.
Additionally, values above 2048 would likely result in unreasonable filesize
increases.</pre>

* ⚠ **WARN** Font em size (unitsPerEm) is 2200 which may be too large (causing filesize bloat), unless you are sure that the detail level in this font requires that much precision. [code: large-value]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: ampersand	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: two	Contours detected: 2	Expected: 1
Glyph name: less	Contours detected: 0	Expected: 1
Glyph name: greater	Contours detected: 0	Expected: 1
Glyph name: at	Contours detected: 0	Expected: 2
Glyph name: Q	Contours detected: 3	Expected: 2
Glyph name: asciicircum	Contours detected: 0	Expected: 1
Glyph name: asciitilde	Contours detected: 0	Expected: 1
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
Glyph name: currency	Contours detected: 0	Expected: 2
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: copyright	Contours detected: 0	Expected: 3
Glyph name: logicalnot	Contours detected: 0	Expected: 1
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: uni00B2	Contours detected: 2	Expected: 1
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
Glyph name: uni2082	Contours detected: 2	Expected: 1
Glyph name: lira	Contours detected: 0	Expected: 1
Glyph name: uni20A9	Contours detected: 6	Expected: 1, 3, 4 or 7
Glyph name: uni20AD	Contours detected: 0	Expected: 1
Glyph name: uni20BA	Contours detected: 0	Expected: 1
Glyph name: uni20BC	Contours detected: 0	Expected: 1
Glyph name: approxequal	Contours detected: 0	Expected: 2
Glyph name: notequal	Contours detected: 0	Expected: 1
Glyph name: lessequal	Contours detected: 0	Expected: 2
Glyph name: greaterequal	Contours detected: 0	Expected: 2
Glyph name: uni27E8	Contours detected: 0	Expected: 1
Glyph name: uni27E9	Contours detected: 0	Expected: 1
Glyph name: Q	Contours detected: 3	Expected: 2
Glyph name: ampersand	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: approxequal	Contours detected: 0	Expected: 2
Glyph name: asciicircum	Contours detected: 0	Expected: 1
Glyph name: asciitilde	Contours detected: 0	Expected: 1
Glyph name: at	Contours detected: 0	Expected: 2
Glyph name: copyright	Contours detected: 0	Expected: 3
Glyph name: currency	Contours detected: 0	Expected: 2
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: greater	Contours detected: 0	Expected: 1
Glyph name: greaterequal	Contours detected: 0	Expected: 2
Glyph name: less	Contours detected: 0	Expected: 1
Glyph name: lessequal	Contours detected: 0	Expected: 2
Glyph name: lira	Contours detected: 0	Expected: 1
Glyph name: logicalnot	Contours detected: 0	Expected: 1
Glyph name: notequal	Contours detected: 0	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
Glyph name: two	Contours detected: 2	Expected: 1
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: uni20A9	Contours detected: 6	Expected: 1, 3, 4 or 7
Glyph name: uni20AD	Contours detected: 0	Expected: 1
Glyph name: uni20BA	Contours detected: 0	Expected: 1
Glyph name: uni20BC	Contours detected: 0	Expected: 1
Glyph name: uni27E8	Contours detected: 0	Expected: 1
Glyph name: uni27E9	Contours detected: 0	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Combined length of family and style must not exceed 27 characters.</summary>

* [com.google.fonts/check/name/family_and_style_max_length](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/family_and_style_max_length)
<pre>--- Rationale ---
According to a GlyphsApp tutorial [1], in order to make sure all versions of
Windows recognize it as a valid font file, we must make sure that the
concatenated length of the familyname (NameID.FONT_FAMILY_NAME) and style
(NameID.FONT_SUBFAMILY_NAME) strings in the name table do not exceed 20
characters.
After discussing the problem in more detail at `FontBakery issue #2179 [2] we
decided that allowing up to 27 chars would still be on the safe side, though.
[1] https://glyphsapp.com/tutorials/multiple-masters-part-3-setting-up-instances
[2] https://github.com/googlefonts/fontbakery/issues/2179</pre>

* ⚠ **WARN** The combined length of family and style exceeds 27 chars in the following 'WINDOWS' entries:
 FONT_FAMILY_NAME = 'Montagu Slab 16pt ExtraLight' / SUBFAMILY_NAME = 'Regular'

Please take a look at the conversation at https://github.com/googlefonts/fontbakery/issues/2179 in order to understand the reasoning behind these name table records max-length criteria. [code: too-long]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking unitsPerEm value is reasonable.</summary>

* [com.google.fonts/check/unitsperem](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/head.html#com.google.fonts/check/unitsperem)
<pre>--- Rationale ---
According to the OpenType spec:
The value of unitsPerEm at the head table must be a value between 16 and 16384.
Any value in this range is valid.
In fonts that have TrueType outlines, a power of 2 is recommended as this allows
performance optimizations in some rasterizers.
But 1000 is a commonly used value. And 2000 may become increasingly more common
on Variable Fonts.</pre>

* ⚠ **WARN** In order to optimize performance on some legacy renderers, the value of unitsPerEm at the head table should idealy be a power of between 16 to 16384. And values of 1000 and 2000 are also common and may be just fine as well. But we got 2200 instead. [code: suboptimal]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* uni1EB4: X=602.0,Y=2159.0 (should be at ascender 2160?)
	* uni1EB4: X=954.5,Y=2160.5 (should be at ascender 2160?)
	* uni1EA4: X=1275.0,Y=2159.0 (should be at ascender 2160?)
	* uni1EA4: X=1369.0,Y=2159.0 (should be at ascender 2160?)
	* uni1EA6: X=1036.0,Y=2159.0 (should be at ascender 2160?)
	* uni1EA6: X=1130.0,Y=2159.0 (should be at ascender 2160?)
	* uni1EAA: X=602.0,Y=2159.0 (should be at ascender 2160?)
	* uni1EAA: X=954.5,Y=2160.5 (should be at ascender 2160?)
	* uni1EBE: X=1212.0,Y=2159.0 (should be at ascender 2160?)
	* uni1EBE: X=1305.0,Y=2159.0 (should be at ascender 2160?) and 80 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* braceleft.case: B<<398.0,819.5>-<336.0,756.0>-<226.0,750.0>>/B<<226.0,750.0>-<336.0,744.0>-<398.0,680.5>> = 6.244260924231415
	* braceleft: B<<435.0,713.0>-<367.0,638.0>-<243.0,631.0>>/B<<243.0,631.0>-<367.0,624.0>-<435.0,549.5>> = 6.462019800736384
	* braceright.case: B<<423.5,680.5>-<486.0,744.0>-<595.0,750.0>>/B<<595.0,750.0>-<486.0,756.0>-<423.5,819.5>> = 6.301432826535456
	* braceright: B<<466.0,549.5>-<534.0,624.0>-<658.0,631.0>>/B<<658.0,631.0>-<534.0,638.0>-<466.0,713.0>> = 6.462019800736384
	* eth: B<<897.5,1054.0>-<1008.0,993.0>-<1068.0,867.0>>/B<<1068.0,867.0>-<1035.0,1004.0>-<974.0,1116.0>> = 11.920168419426853
	* nine.lf: B<<1106.5,548.0>-<1142.0,726.0>-<1123.0,979.0>>/B<<1123.0,979.0>-<1106.0,791.0>-<982.0,676.0>> = 9.461732176690402
	* nine: B<<1106.5,548.0>-<1142.0,726.0>-<1123.0,979.0>>/B<<1123.0,979.0>-<1106.0,791.0>-<982.0,676.0>> = 9.461732176690402
	* six.lf: B<<263.5,952.0>-<228.0,774.0>-<247.0,521.0>>/B<<247.0,521.0>-<264.0,709.0>-<388.0,824.0>> = 9.461732176690402
	* six: B<<263.5,952.0>-<228.0,774.0>-<247.0,521.0>>/B<<247.0,521.0>-<264.0,709.0>-<388.0,824.0>> = 9.461732176690402 and yen: L<<803.0,592.0>--<668.0,780.0>>/L<<668.0,780.0>--<680.0,761.0>> = 3.405920114930088 [code: found-jaggy-segments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * dotlessi.ss01: L<<265.0,222.0>--<268.0,1040.0>>
 * i.loclTRK.ss01: L<<265.0,222.0>--<268.0,1040.0>>
 * i.ss01: L<<265.0,222.0>--<268.0,1040.0>>
 * iacute.ss01: L<<265.0,222.0>--<268.0,1040.0>>
 * icircumflex.ss01: L<<265.0,222.0>--<268.0,1040.0>>
 * idieresis.ss01: L<<265.0,222.0>--<268.0,1040.0>>
 * igrave.ss01: L<<265.0,222.0>--<268.0,1040.0>>
 * imacron.ss01: L<<265.0,222.0>--<268.0,1040.0>>
 * l.ss01: L<<258.0,232.0>--<262.0,1494.0>>
 * lacute.ss01: L<<258.0,232.0>--<262.0,1494.0>> and 5 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[9] MontaguSlab16pt-Light.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Ensure Stylistic Sets have description.</summary>

* [com.google.fonts/check/stylisticset_description](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/stylisticset_description)
<pre>--- Rationale ---
Stylistic sets must provide description text. Programs such as InDesign,
TextEdit and Inkscape use that info to display to the users so that they know
what a given stylistic set offers.</pre>

* 🔥 **FAIL** The stylistic set ss01 lacks a description string on the 'name' table. [code: missing-description]

</details>
<details>
<summary>⚠ <b>WARN:</b> Stricter unitsPerEm criteria for Google Fonts. </summary>

* [com.google.fonts/check/unitsperem_strict](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/unitsperem_strict)
<pre>--- Rationale ---
Even though the OpenType spec allows unitsPerEm to be any value between 16 and
16384, the Google Fonts project aims at a narrower set of reasonable values.
The spec suggests usage of powers of two in order to get some performance
improvements on legacy renderers, so those values are acceptable.
But values of 500 or 1000 are also acceptable, with the added benefit that it
makes upm math easier for designers, while the performance hit of not using a
power of two is most likely negligible nowadays.
Additionally, values above 2048 would likely result in unreasonable filesize
increases.</pre>

* ⚠ **WARN** Font em size (unitsPerEm) is 2200 which may be too large (causing filesize bloat), unless you are sure that the detail level in this font requires that much precision. [code: large-value]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: ampersand	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: two	Contours detected: 2	Expected: 1
Glyph name: less	Contours detected: 0	Expected: 1
Glyph name: greater	Contours detected: 0	Expected: 1
Glyph name: at	Contours detected: 0	Expected: 2
Glyph name: Q	Contours detected: 3	Expected: 2
Glyph name: asciicircum	Contours detected: 0	Expected: 1
Glyph name: asciitilde	Contours detected: 0	Expected: 1
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
Glyph name: currency	Contours detected: 0	Expected: 2
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: copyright	Contours detected: 0	Expected: 3
Glyph name: logicalnot	Contours detected: 0	Expected: 1
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: uni00B2	Contours detected: 2	Expected: 1
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
Glyph name: uni2082	Contours detected: 2	Expected: 1
Glyph name: lira	Contours detected: 0	Expected: 1
Glyph name: uni20A6	Contours detected: 4	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
Glyph name: uni20AD	Contours detected: 0	Expected: 1
Glyph name: uni20BA	Contours detected: 0	Expected: 1
Glyph name: uni20BC	Contours detected: 0	Expected: 1
Glyph name: approxequal	Contours detected: 0	Expected: 2
Glyph name: notequal	Contours detected: 0	Expected: 1
Glyph name: lessequal	Contours detected: 0	Expected: 2
Glyph name: greaterequal	Contours detected: 0	Expected: 2
Glyph name: uni27E8	Contours detected: 0	Expected: 1
Glyph name: uni27E9	Contours detected: 0	Expected: 1
Glyph name: Q	Contours detected: 3	Expected: 2
Glyph name: ampersand	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: approxequal	Contours detected: 0	Expected: 2
Glyph name: asciicircum	Contours detected: 0	Expected: 1
Glyph name: asciitilde	Contours detected: 0	Expected: 1
Glyph name: at	Contours detected: 0	Expected: 2
Glyph name: copyright	Contours detected: 0	Expected: 3
Glyph name: currency	Contours detected: 0	Expected: 2
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: greater	Contours detected: 0	Expected: 1
Glyph name: greaterequal	Contours detected: 0	Expected: 2
Glyph name: less	Contours detected: 0	Expected: 1
Glyph name: lessequal	Contours detected: 0	Expected: 2
Glyph name: lira	Contours detected: 0	Expected: 1
Glyph name: logicalnot	Contours detected: 0	Expected: 1
Glyph name: notequal	Contours detected: 0	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
Glyph name: two	Contours detected: 2	Expected: 1
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: uni20A6	Contours detected: 4	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
Glyph name: uni20AD	Contours detected: 0	Expected: 1
Glyph name: uni20BA	Contours detected: 0	Expected: 1
Glyph name: uni20BC	Contours detected: 0	Expected: 1
Glyph name: uni27E8	Contours detected: 0	Expected: 1
Glyph name: uni27E9	Contours detected: 0	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Combined length of family and style must not exceed 27 characters.</summary>

* [com.google.fonts/check/name/family_and_style_max_length](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/family_and_style_max_length)
<pre>--- Rationale ---
According to a GlyphsApp tutorial [1], in order to make sure all versions of
Windows recognize it as a valid font file, we must make sure that the
concatenated length of the familyname (NameID.FONT_FAMILY_NAME) and style
(NameID.FONT_SUBFAMILY_NAME) strings in the name table do not exceed 20
characters.
After discussing the problem in more detail at `FontBakery issue #2179 [2] we
decided that allowing up to 27 chars would still be on the safe side, though.
[1] https://glyphsapp.com/tutorials/multiple-masters-part-3-setting-up-instances
[2] https://github.com/googlefonts/fontbakery/issues/2179</pre>

* ⚠ **WARN** The combined length of family and style exceeds 27 chars in the following 'WINDOWS' entries:
 FONT_FAMILY_NAME = 'Montagu Slab 16pt Light' / SUBFAMILY_NAME = 'Regular'

Please take a look at the conversation at https://github.com/googlefonts/fontbakery/issues/2179 in order to understand the reasoning behind these name table records max-length criteria. [code: too-long]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking unitsPerEm value is reasonable.</summary>

* [com.google.fonts/check/unitsperem](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/head.html#com.google.fonts/check/unitsperem)
<pre>--- Rationale ---
According to the OpenType spec:
The value of unitsPerEm at the head table must be a value between 16 and 16384.
Any value in this range is valid.
In fonts that have TrueType outlines, a power of 2 is recommended as this allows
performance optimizations in some rasterizers.
But 1000 is a commonly used value. And 2000 may become increasingly more common
on Variable Fonts.</pre>

* ⚠ **WARN** In order to optimize performance on some legacy renderers, the value of unitsPerEm at the head table should idealy be a power of between 16 to 16384. And values of 1000 and 2000 are also common and may be just fine as well. But we got 2200 instead. [code: suboptimal]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* Ohorn: X=1649.5,Y=1498.5 (should be at cap-height 1500?)
	* uni1EDA: X=1649.5,Y=1498.5 (should be at cap-height 1500?)
	* uni1EE2: X=1649.5,Y=1498.5 (should be at cap-height 1500?)
	* uni1EDC: X=1649.5,Y=1498.5 (should be at cap-height 1500?)
	* uni1EDE: X=1649.5,Y=1498.5 (should be at cap-height 1500?)
	* uni1EE0: X=1649.5,Y=1498.5 (should be at cap-height 1500?)
	* R: X=77.0,Y=1502.0 (should be at cap-height 1500?)
	* R: X=1005.0,Y=1502.0 (should be at cap-height 1500?)
	* Racute: X=77.0,Y=1502.0 (should be at cap-height 1500?)
	* Racute: X=1005.0,Y=1502.0 (should be at cap-height 1500?) and 27 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* R: L<<1006.0,700.0>--<932.0,700.0>>/B<<932.0,700.0>-<1050.0,670.0>-<1103.0,581.0>> = 14.264512298079882
	* Racute: L<<1006.0,700.0>--<932.0,700.0>>/B<<932.0,700.0>-<1050.0,670.0>-<1103.0,581.0>> = 14.264512298079882
	* Rcaron: L<<1006.0,700.0>--<932.0,700.0>>/B<<932.0,700.0>-<1050.0,670.0>-<1103.0,581.0>> = 14.264512298079882
	* braceleft.case: B<<420.5,820.5>-<358.0,756.0>-<242.0,750.0>>/B<<242.0,750.0>-<358.0,744.0>-<420.5,679.5>> = 5.921872268327562
	* braceleft: B<<460.0,719.0>-<392.0,640.0>-<258.0,633.0>>/B<<258.0,633.0>-<392.0,626.0>-<460.0,547.0>> = 5.980689950330773
	* braceright.case: B<<407.5,679.5>-<470.0,744.0>-<586.0,750.0>>/B<<586.0,750.0>-<470.0,756.0>-<407.5,820.5>> = 5.921872268327562
	* braceright: B<<450.0,547.0>-<518.0,626.0>-<652.0,633.0>>/B<<652.0,633.0>-<518.0,640.0>-<450.0,719.0>> = 5.980689950330773
	* eth: B<<884.5,1054.0>-<992.0,995.0>-<1050.0,870.0>>/B<<1050.0,870.0>-<1020.0,1003.0>-<964.5,1111.5>> = 12.18016755933628
	* nine.lf: B<<1085.0,542.5>-<1119.0,709.0>-<1102.0,945.0>>/B<<1102.0,945.0>-<1080.0,772.0>-<961.0,665.0>> = 11.367390806004797
	* nine: B<<1085.0,542.5>-<1119.0,709.0>-<1102.0,945.0>>/B<<1102.0,945.0>-<1080.0,772.0>-<961.0,665.0>> = 11.367390806004797 and 7 more. [code: found-jaggy-segments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * dotlessi.ss01: L<<262.0,241.0>--<268.0,1026.0>>
 * i.loclTRK.ss01: L<<262.0,241.0>--<268.0,1026.0>>
 * i.ss01: L<<262.0,241.0>--<268.0,1026.0>>
 * iacute.ss01: L<<262.0,241.0>--<268.0,1026.0>>
 * icircumflex.ss01: L<<262.0,241.0>--<268.0,1026.0>>
 * idieresis.ss01: L<<262.0,241.0>--<268.0,1026.0>>
 * igrave.ss01: L<<262.0,241.0>--<268.0,1026.0>>
 * imacron.ss01: L<<262.0,241.0>--<268.0,1026.0>>
 * l.ss01: L<<248.0,258.0>--<256.0,1475.0>>
 * lacute.ss01: L<<248.0,258.0>--<256.0,1475.0>> and 4 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[9] MontaguSlab16pt-Medium.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Ensure Stylistic Sets have description.</summary>

* [com.google.fonts/check/stylisticset_description](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/stylisticset_description)
<pre>--- Rationale ---
Stylistic sets must provide description text. Programs such as InDesign,
TextEdit and Inkscape use that info to display to the users so that they know
what a given stylistic set offers.</pre>

* 🔥 **FAIL** The stylistic set ss01 lacks a description string on the 'name' table. [code: missing-description]

</details>
<details>
<summary>⚠ <b>WARN:</b> Stricter unitsPerEm criteria for Google Fonts. </summary>

* [com.google.fonts/check/unitsperem_strict](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/unitsperem_strict)
<pre>--- Rationale ---
Even though the OpenType spec allows unitsPerEm to be any value between 16 and
16384, the Google Fonts project aims at a narrower set of reasonable values.
The spec suggests usage of powers of two in order to get some performance
improvements on legacy renderers, so those values are acceptable.
But values of 500 or 1000 are also acceptable, with the added benefit that it
makes upm math easier for designers, while the performance hit of not using a
power of two is most likely negligible nowadays.
Additionally, values above 2048 would likely result in unreasonable filesize
increases.</pre>

* ⚠ **WARN** Font em size (unitsPerEm) is 2200 which may be too large (causing filesize bloat), unless you are sure that the detail level in this font requires that much precision. [code: large-value]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: ampersand	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: two	Contours detected: 2	Expected: 1
Glyph name: less	Contours detected: 0	Expected: 1
Glyph name: greater	Contours detected: 0	Expected: 1
Glyph name: at	Contours detected: 0	Expected: 2
Glyph name: Q	Contours detected: 3	Expected: 2
Glyph name: asciicircum	Contours detected: 0	Expected: 1
Glyph name: asciitilde	Contours detected: 0	Expected: 1
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
Glyph name: currency	Contours detected: 0	Expected: 2
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: copyright	Contours detected: 0	Expected: 3
Glyph name: logicalnot	Contours detected: 0	Expected: 1
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: uni00B2	Contours detected: 2	Expected: 1
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
Glyph name: uni2082	Contours detected: 2	Expected: 1
Glyph name: lira	Contours detected: 0	Expected: 1
Glyph name: uni20AD	Contours detected: 0	Expected: 1
Glyph name: uni20BA	Contours detected: 0	Expected: 1
Glyph name: uni20BC	Contours detected: 0	Expected: 1
Glyph name: approxequal	Contours detected: 0	Expected: 2
Glyph name: notequal	Contours detected: 0	Expected: 1
Glyph name: lessequal	Contours detected: 0	Expected: 2
Glyph name: greaterequal	Contours detected: 0	Expected: 2
Glyph name: uni27E8	Contours detected: 0	Expected: 1
Glyph name: uni27E9	Contours detected: 0	Expected: 1
Glyph name: Q	Contours detected: 3	Expected: 2
Glyph name: ampersand	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: approxequal	Contours detected: 0	Expected: 2
Glyph name: asciicircum	Contours detected: 0	Expected: 1
Glyph name: asciitilde	Contours detected: 0	Expected: 1
Glyph name: at	Contours detected: 0	Expected: 2
Glyph name: copyright	Contours detected: 0	Expected: 3
Glyph name: currency	Contours detected: 0	Expected: 2
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: greater	Contours detected: 0	Expected: 1
Glyph name: greaterequal	Contours detected: 0	Expected: 2
Glyph name: less	Contours detected: 0	Expected: 1
Glyph name: lessequal	Contours detected: 0	Expected: 2
Glyph name: lira	Contours detected: 0	Expected: 1
Glyph name: logicalnot	Contours detected: 0	Expected: 1
Glyph name: notequal	Contours detected: 0	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
Glyph name: two	Contours detected: 2	Expected: 1
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: uni20AD	Contours detected: 0	Expected: 1
Glyph name: uni20BA	Contours detected: 0	Expected: 1
Glyph name: uni20BC	Contours detected: 0	Expected: 1
Glyph name: uni27E8	Contours detected: 0	Expected: 1
Glyph name: uni27E9	Contours detected: 0	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Combined length of family and style must not exceed 27 characters.</summary>

* [com.google.fonts/check/name/family_and_style_max_length](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/family_and_style_max_length)
<pre>--- Rationale ---
According to a GlyphsApp tutorial [1], in order to make sure all versions of
Windows recognize it as a valid font file, we must make sure that the
concatenated length of the familyname (NameID.FONT_FAMILY_NAME) and style
(NameID.FONT_SUBFAMILY_NAME) strings in the name table do not exceed 20
characters.
After discussing the problem in more detail at `FontBakery issue #2179 [2] we
decided that allowing up to 27 chars would still be on the safe side, though.
[1] https://glyphsapp.com/tutorials/multiple-masters-part-3-setting-up-instances
[2] https://github.com/googlefonts/fontbakery/issues/2179</pre>

* ⚠ **WARN** The combined length of family and style exceeds 27 chars in the following 'WINDOWS' entries:
 FONT_FAMILY_NAME = 'Montagu Slab 16pt Medium' / SUBFAMILY_NAME = 'Regular'

Please take a look at the conversation at https://github.com/googlefonts/fontbakery/issues/2179 in order to understand the reasoning behind these name table records max-length criteria. [code: too-long]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking unitsPerEm value is reasonable.</summary>

* [com.google.fonts/check/unitsperem](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/head.html#com.google.fonts/check/unitsperem)
<pre>--- Rationale ---
According to the OpenType spec:
The value of unitsPerEm at the head table must be a value between 16 and 16384.
Any value in this range is valid.
In fonts that have TrueType outlines, a power of 2 is recommended as this allows
performance optimizations in some rasterizers.
But 1000 is a commonly used value. And 2000 may become increasingly more common
on Variable Fonts.</pre>

* ⚠ **WARN** In order to optimize performance on some legacy renderers, the value of unitsPerEm at the head table should idealy be a power of between 16 to 16384. And values of 1000 and 2000 are also common and may be just fine as well. But we got 2200 instead. [code: suboptimal]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* uni1EA8: X=1075.0,Y=2159.0 (should be at ascender 2160?)
	* uni1EC2: X=993.0,Y=2159.0 (should be at ascender 2160?)
	* uni1ED4: X=1112.0,Y=2159.0 (should be at ascender 2160?)
	* uni1EA3: X=550.0,Y=1501.0 (should be at cap-height 1500?)
	* uni1EBB: X=525.0,Y=1501.0 (should be at cap-height 1500?)
	* g: X=932.0,Y=-1.0 (should be at baseline 0?)
	* g: X=454.0,Y=-1.0 (should be at baseline 0?)
	* gbreve: X=932.0,Y=-1.0 (should be at baseline 0?)
	* gbreve: X=454.0,Y=-1.0 (should be at baseline 0?)
	* gcaron: X=932.0,Y=-1.0 (should be at baseline 0?) and 21 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are any segments inordinately short?</summary>

* [com.google.fonts/check/outline_short_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_short_segments)
<pre>--- Rationale ---
This check looks for outline segments which seem particularly short (less than
0.006%% of the overall path length).
This check is not run for variable fonts, as they may legitimately have short
segments. As this check is liable to generate significant numbers of false
positives, it will pass if there are more than 100 reported short segments.</pre>

* ⚠ **WARN** The following glyphs have segments which seem very short:
	* Aogonek contains a short segment B<<1541.0,-297.0>-<1568.0,-297.0>-<1586.5,-290.5>>
	* Aogonek contains a short segment B<<1586.5,-290.5>-<1605.0,-284.0>-<1626.0,-271.0>>
	* Ccedilla contains a short segment B<<944.0,-259.0>-<944.0,-232.0>-<925.0,-219.0>>
	* Ccedilla contains a short segment B<<925.0,-219.0>-<906.0,-206.0>-<876.0,-206.0>>
	* Ccedilla contains a short segment L<<903.0,-104.0>--<918.0,-104.0>>
	* Eogonek contains a short segment B<<1281.0,-207.0>-<1281.0,-250.0>-<1308.0,-273.5>>
	* Eogonek contains a short segment B<<1308.0,-273.5>-<1335.0,-297.0>-<1378.0,-297.0>>
	* Eogonek contains a short segment B<<1378.0,-297.0>-<1404.0,-297.0>-<1422.5,-290.5>>
	* Eogonek contains a short segment B<<1422.5,-290.5>-<1441.0,-284.0>-<1463.0,-271.0>>
	* Scedilla contains a short segment B<<929.0,-25.0>-<914.0,-25.0>-<900.0,-25.0>> and 68 more. [code: found-short-segments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* R: L<<1055.0,698.0>--<1005.0,698.0>>/B<<1005.0,698.0>-<1128.0,673.0>-<1181.5,586.0>> = 11.488981202159193
	* Racute: L<<1055.0,698.0>--<1005.0,698.0>>/B<<1005.0,698.0>-<1128.0,673.0>-<1181.5,586.0>> = 11.488981202159193
	* Rcaron: L<<1055.0,698.0>--<1005.0,698.0>>/B<<1005.0,698.0>-<1128.0,673.0>-<1181.5,586.0>> = 11.488981202159193
	* braceleft.case: B<<485.0,823.5>-<421.0,756.0>-<288.0,750.0>>/B<<288.0,750.0>-<421.0,744.0>-<485.0,676.5>> = 5.166041337270114
	* braceleft: B<<532.5,735.5>-<466.0,644.0>-<301.0,637.0>>/B<<301.0,637.0>-<466.0,629.0>-<532.5,537.5>> = 5.205076772283028
	* braceright.case: B<<360.0,676.5>-<424.0,744.0>-<557.0,750.0>>/B<<557.0,750.0>-<424.0,756.0>-<360.0,823.5>> = 5.166041337270114
	* braceright: B<<404.5,537.5>-<471.0,629.0>-<636.0,637.0>>/B<<636.0,637.0>-<471.0,644.0>-<404.5,735.5>> = 5.205076772283028
	* eng: L<<513.0,1140.0>--<513.0,862.0>>/B<<513.0,862.0>-<549.0,1007.0>-<649.5,1082.5>> = 13.943230920553672
	* eth: B<<846.5,1055.0>-<946.0,1001.0>-<1000.0,879.0>>/B<<1000.0,879.0>-<977.0,998.0>-<935.5,1096.5>> = 12.936189670735347
	* m: L<<509.0,1139.0>--<509.0,891.0>>/B<<509.0,891.0>-<540.0,1019.0>-<626.0,1088.0>> = 13.614182744829332 and 36 more. [code: found-jaggy-segments]

</details>
<br>
</details>
<details>
<summary><b>[9] MontaguSlab16pt-Regular.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Ensure Stylistic Sets have description.</summary>

* [com.google.fonts/check/stylisticset_description](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/stylisticset_description)
<pre>--- Rationale ---
Stylistic sets must provide description text. Programs such as InDesign,
TextEdit and Inkscape use that info to display to the users so that they know
what a given stylistic set offers.</pre>

* 🔥 **FAIL** The stylistic set ss01 lacks a description string on the 'name' table. [code: missing-description]

</details>
<details>
<summary>⚠ <b>WARN:</b> Stricter unitsPerEm criteria for Google Fonts. </summary>

* [com.google.fonts/check/unitsperem_strict](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/unitsperem_strict)
<pre>--- Rationale ---
Even though the OpenType spec allows unitsPerEm to be any value between 16 and
16384, the Google Fonts project aims at a narrower set of reasonable values.
The spec suggests usage of powers of two in order to get some performance
improvements on legacy renderers, so those values are acceptable.
But values of 500 or 1000 are also acceptable, with the added benefit that it
makes upm math easier for designers, while the performance hit of not using a
power of two is most likely negligible nowadays.
Additionally, values above 2048 would likely result in unreasonable filesize
increases.</pre>

* ⚠ **WARN** Font em size (unitsPerEm) is 2200 which may be too large (causing filesize bloat), unless you are sure that the detail level in this font requires that much precision. [code: large-value]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: ampersand	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: two	Contours detected: 2	Expected: 1
Glyph name: less	Contours detected: 0	Expected: 1
Glyph name: greater	Contours detected: 0	Expected: 1
Glyph name: at	Contours detected: 0	Expected: 2
Glyph name: Q	Contours detected: 3	Expected: 2
Glyph name: asciicircum	Contours detected: 0	Expected: 1
Glyph name: asciitilde	Contours detected: 0	Expected: 1
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
Glyph name: currency	Contours detected: 0	Expected: 2
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: copyright	Contours detected: 0	Expected: 3
Glyph name: logicalnot	Contours detected: 0	Expected: 1
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: uni00B2	Contours detected: 2	Expected: 1
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
Glyph name: uni2082	Contours detected: 2	Expected: 1
Glyph name: lira	Contours detected: 0	Expected: 1
Glyph name: uni20AD	Contours detected: 0	Expected: 1
Glyph name: uni20BA	Contours detected: 0	Expected: 1
Glyph name: uni20BC	Contours detected: 0	Expected: 1
Glyph name: approxequal	Contours detected: 0	Expected: 2
Glyph name: notequal	Contours detected: 0	Expected: 1
Glyph name: lessequal	Contours detected: 0	Expected: 2
Glyph name: greaterequal	Contours detected: 0	Expected: 2
Glyph name: uni27E8	Contours detected: 0	Expected: 1
Glyph name: uni27E9	Contours detected: 0	Expected: 1
Glyph name: Q	Contours detected: 3	Expected: 2
Glyph name: ampersand	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: approxequal	Contours detected: 0	Expected: 2
Glyph name: asciicircum	Contours detected: 0	Expected: 1
Glyph name: asciitilde	Contours detected: 0	Expected: 1
Glyph name: at	Contours detected: 0	Expected: 2
Glyph name: copyright	Contours detected: 0	Expected: 3
Glyph name: currency	Contours detected: 0	Expected: 2
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: greater	Contours detected: 0	Expected: 1
Glyph name: greaterequal	Contours detected: 0	Expected: 2
Glyph name: less	Contours detected: 0	Expected: 1
Glyph name: lessequal	Contours detected: 0	Expected: 2
Glyph name: lira	Contours detected: 0	Expected: 1
Glyph name: logicalnot	Contours detected: 0	Expected: 1
Glyph name: notequal	Contours detected: 0	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
Glyph name: two	Contours detected: 2	Expected: 1
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: uni20AD	Contours detected: 0	Expected: 1
Glyph name: uni20BA	Contours detected: 0	Expected: 1
Glyph name: uni20BC	Contours detected: 0	Expected: 1
Glyph name: uni27E8	Contours detected: 0	Expected: 1
Glyph name: uni27E9	Contours detected: 0	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking unitsPerEm value is reasonable.</summary>

* [com.google.fonts/check/unitsperem](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/head.html#com.google.fonts/check/unitsperem)
<pre>--- Rationale ---
According to the OpenType spec:
The value of unitsPerEm at the head table must be a value between 16 and 16384.
Any value in this range is valid.
In fonts that have TrueType outlines, a power of 2 is recommended as this allows
performance optimizations in some rasterizers.
But 1000 is a commonly used value. And 2000 may become increasingly more common
on Variable Fonts.</pre>

* ⚠ **WARN** In order to optimize performance on some legacy renderers, the value of unitsPerEm at the head table should idealy be a power of between 16 to 16384. And values of 1000 and 2000 are also common and may be just fine as well. But we got 2200 instead. [code: suboptimal]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* adieresis: X=804.5,Y=1498.5 (should be at cap-height 1500?)
	* adieresis: X=985.0,Y=1498.5 (should be at cap-height 1500?)
	* adieresis: X=351.5,Y=1498.5 (should be at cap-height 1500?)
	* adieresis: X=532.5,Y=1498.5 (should be at cap-height 1500?)
	* edieresis: X=788.0,Y=1498.5 (should be at cap-height 1500?)
	* edieresis: X=968.0,Y=1498.5 (should be at cap-height 1500?)
	* edieresis: X=335.0,Y=1498.5 (should be at cap-height 1500?)
	* edieresis: X=515.5,Y=1498.5 (should be at cap-height 1500?)
	* eogonek: X=848.0,Y=2.0 (should be at baseline 0?)
	* uni0123: X=670.0,Y=1499.0 (should be at cap-height 1500?) and 32 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are any segments inordinately short?</summary>

* [com.google.fonts/check/outline_short_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_short_segments)
<pre>--- Rationale ---
This check looks for outline segments which seem particularly short (less than
0.006%% of the overall path length).
This check is not run for variable fonts, as they may legitimately have short
segments. As this check is liable to generate significant numbers of false
positives, it will pass if there are more than 100 reported short segments.</pre>

* ⚠ **WARN** The following glyphs have segments which seem very short:
	* Ccedilla contains a short segment B<<959.0,-262.0>-<959.0,-231.0>-<936.5,-215.5>>
	* Ccedilla contains a short segment B<<936.5,-215.5>-<914.0,-200.0>-<880.0,-200.0>>
	* Ccedilla contains a short segment L<<892.0,-115.0>--<911.0,-115.0>>
	* Eogonek contains a short segment B<<1352.0,-314.0>-<1382.0,-314.0>-<1402.5,-306.0>>
	* Eogonek contains a short segment B<<1402.5,-306.0>-<1423.0,-298.0>-<1448.0,-282.0>>
	* Scedilla contains a short segment B<<918.0,-25.0>-<901.0,-25.0>-<885.0,-24.0>>
	* Scedilla contains a short segment L<<873.0,-115.0>--<893.0,-115.0>>
	* Scedilla contains a short segment B<<940.0,-262.0>-<940.0,-231.0>-<917.5,-215.5>>
	* Scedilla contains a short segment B<<917.5,-215.5>-<895.0,-200.0>-<861.0,-200.0>>
	* uni0162 contains a short segment L<<902.0,-115.0>--<922.0,-115.0>> and 71 more. [code: found-short-segments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* R: L<<1031.0,699.0>--<970.0,699.0>>/B<<970.0,699.0>-<1090.0,671.0>-<1143.0,583.0>> = 13.134022306396327
	* Racute: L<<1031.0,699.0>--<970.0,699.0>>/B<<970.0,699.0>-<1090.0,671.0>-<1143.0,583.0>> = 13.134022306396327
	* Rcaron: L<<1031.0,699.0>--<970.0,699.0>>/B<<970.0,699.0>-<1090.0,671.0>-<1143.0,583.0>> = 13.134022306396327
	* braceleft.case: B<<453.5,822.0>-<390.0,756.0>-<266.0,750.0>>/B<<266.0,750.0>-<390.0,744.0>-<453.5,678.0>> = 5.540431594400349
	* braceleft: B<<497.0,727.5>-<430.0,642.0>-<280.0,635.0>>/B<<280.0,635.0>-<430.0,628.0>-<497.0,542.5>> = 5.343729186545131
	* braceright.case: B<<383.5,678.0>-<447.0,744.0>-<571.0,750.0>>/B<<571.0,750.0>-<447.0,756.0>-<383.5,822.0>> = 5.540431594400349
	* braceright: B<<427.0,542.5>-<494.0,628.0>-<644.0,635.0>>/B<<644.0,635.0>-<494.0,642.0>-<427.0,727.5>> = 5.343729186545131
	* eth: B<<865.0,1054.5>-<968.0,998.0>-<1025.0,875.0>>/B<<1025.0,875.0>-<998.0,1000.0>-<950.0,1103.5>> = 12.675063369819934
	* uni0156: L<<1031.0,699.0>--<970.0,699.0>>/B<<970.0,699.0>-<1090.0,671.0>-<1143.0,583.0>> = 13.134022306396327
	* uni0210: L<<1031.0,699.0>--<970.0,699.0>>/B<<970.0,699.0>-<1090.0,671.0>-<1143.0,583.0>> = 13.134022306396327 and 3 more. [code: found-jaggy-segments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * k: L<<258.0,123.0>--<259.0,1446.0>> and uni0137: L<<258.0,123.0>--<259.0,1446.0>> [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[10] MontaguSlab16pt-SemiBold.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Ensure Stylistic Sets have description.</summary>

* [com.google.fonts/check/stylisticset_description](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/stylisticset_description)
<pre>--- Rationale ---
Stylistic sets must provide description text. Programs such as InDesign,
TextEdit and Inkscape use that info to display to the users so that they know
what a given stylistic set offers.</pre>

* 🔥 **FAIL** The stylistic set ss01 lacks a description string on the 'name' table. [code: missing-description]

</details>
<details>
<summary>⚠ <b>WARN:</b> Stricter unitsPerEm criteria for Google Fonts. </summary>

* [com.google.fonts/check/unitsperem_strict](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/unitsperem_strict)
<pre>--- Rationale ---
Even though the OpenType spec allows unitsPerEm to be any value between 16 and
16384, the Google Fonts project aims at a narrower set of reasonable values.
The spec suggests usage of powers of two in order to get some performance
improvements on legacy renderers, so those values are acceptable.
But values of 500 or 1000 are also acceptable, with the added benefit that it
makes upm math easier for designers, while the performance hit of not using a
power of two is most likely negligible nowadays.
Additionally, values above 2048 would likely result in unreasonable filesize
increases.</pre>

* ⚠ **WARN** Font em size (unitsPerEm) is 2200 which may be too large (causing filesize bloat), unless you are sure that the detail level in this font requires that much precision. [code: large-value]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: ampersand	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: two	Contours detected: 2	Expected: 1
Glyph name: less	Contours detected: 0	Expected: 1
Glyph name: greater	Contours detected: 0	Expected: 1
Glyph name: at	Contours detected: 0	Expected: 2
Glyph name: Q	Contours detected: 3	Expected: 2
Glyph name: asciicircum	Contours detected: 0	Expected: 1
Glyph name: asciitilde	Contours detected: 0	Expected: 1
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
Glyph name: currency	Contours detected: 0	Expected: 2
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: copyright	Contours detected: 0	Expected: 3
Glyph name: logicalnot	Contours detected: 0	Expected: 1
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: uni00B2	Contours detected: 2	Expected: 1
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
Glyph name: uni2082	Contours detected: 2	Expected: 1
Glyph name: lira	Contours detected: 0	Expected: 1
Glyph name: uni20A6	Contours detected: 4	Expected: 1, 3 or 5
Glyph name: uni20AD	Contours detected: 0	Expected: 1
Glyph name: uni20BA	Contours detected: 0	Expected: 1
Glyph name: uni20BC	Contours detected: 0	Expected: 1
Glyph name: approxequal	Contours detected: 0	Expected: 2
Glyph name: notequal	Contours detected: 0	Expected: 1
Glyph name: lessequal	Contours detected: 0	Expected: 2
Glyph name: greaterequal	Contours detected: 0	Expected: 2
Glyph name: uni27E8	Contours detected: 0	Expected: 1
Glyph name: uni27E9	Contours detected: 0	Expected: 1
Glyph name: Q	Contours detected: 3	Expected: 2
Glyph name: ampersand	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: approxequal	Contours detected: 0	Expected: 2
Glyph name: asciicircum	Contours detected: 0	Expected: 1
Glyph name: asciitilde	Contours detected: 0	Expected: 1
Glyph name: at	Contours detected: 0	Expected: 2
Glyph name: copyright	Contours detected: 0	Expected: 3
Glyph name: currency	Contours detected: 0	Expected: 2
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: greater	Contours detected: 0	Expected: 1
Glyph name: greaterequal	Contours detected: 0	Expected: 2
Glyph name: less	Contours detected: 0	Expected: 1
Glyph name: lessequal	Contours detected: 0	Expected: 2
Glyph name: lira	Contours detected: 0	Expected: 1
Glyph name: logicalnot	Contours detected: 0	Expected: 1
Glyph name: notequal	Contours detected: 0	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
Glyph name: two	Contours detected: 2	Expected: 1
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: uni20A6	Contours detected: 4	Expected: 1, 3 or 5
Glyph name: uni20AD	Contours detected: 0	Expected: 1
Glyph name: uni20BA	Contours detected: 0	Expected: 1
Glyph name: uni20BC	Contours detected: 0	Expected: 1
Glyph name: uni27E8	Contours detected: 0	Expected: 1
Glyph name: uni27E9	Contours detected: 0	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Combined length of family and style must not exceed 27 characters.</summary>

* [com.google.fonts/check/name/family_and_style_max_length](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/family_and_style_max_length)
<pre>--- Rationale ---
According to a GlyphsApp tutorial [1], in order to make sure all versions of
Windows recognize it as a valid font file, we must make sure that the
concatenated length of the familyname (NameID.FONT_FAMILY_NAME) and style
(NameID.FONT_SUBFAMILY_NAME) strings in the name table do not exceed 20
characters.
After discussing the problem in more detail at `FontBakery issue #2179 [2] we
decided that allowing up to 27 chars would still be on the safe side, though.
[1] https://glyphsapp.com/tutorials/multiple-masters-part-3-setting-up-instances
[2] https://github.com/googlefonts/fontbakery/issues/2179</pre>

* ⚠ **WARN** The combined length of family and style exceeds 27 chars in the following 'WINDOWS' entries:
 FONT_FAMILY_NAME = 'Montagu Slab 16pt SemiBold' / SUBFAMILY_NAME = 'Regular'

Please take a look at the conversation at https://github.com/googlefonts/fontbakery/issues/2179 in order to understand the reasoning behind these name table records max-length criteria. [code: too-long]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking unitsPerEm value is reasonable.</summary>

* [com.google.fonts/check/unitsperem](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/head.html#com.google.fonts/check/unitsperem)
<pre>--- Rationale ---
According to the OpenType spec:
The value of unitsPerEm at the head table must be a value between 16 and 16384.
Any value in this range is valid.
In fonts that have TrueType outlines, a power of 2 is recommended as this allows
performance optimizations in some rasterizers.
But 1000 is a commonly used value. And 2000 may become increasingly more common
on Variable Fonts.</pre>

* ⚠ **WARN** In order to optimize performance on some legacy renderers, the value of unitsPerEm at the head table should idealy be a power of between 16 to 16384. And values of 1000 and 2000 are also common and may be just fine as well. But we got 2200 instead. [code: suboptimal]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* Eng: X=1335.0,Y=-2.0 (should be at baseline 0?)
	* eth: X=624.5,Y=1498.0 (should be at cap-height 1500?)
	* v: X=559.0,Y=-2.0 (should be at baseline 0?)
	* v: X=841.0,Y=-2.0 (should be at baseline 0?)
	* w: X=520.0,Y=-2.0 (should be at baseline 0?)
	* w: X=1507.0,Y=-2.0 (should be at baseline 0?)
	* w: X=1236.0,Y=-2.0 (should be at baseline 0?)
	* w: X=793.0,Y=-2.0 (should be at baseline 0?)
	* wacute: X=520.0,Y=-2.0 (should be at baseline 0?)
	* wacute: X=1507.0,Y=-2.0 (should be at baseline 0?) and 27 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---
This check looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.
This check is not run for variable fonts, as they may legitimately have colinear
vectors.</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* uhorn: L<<813.0,1149.0>--<1253.0,1149.0>> -> L<<1253.0,1149.0>--<1253.0,1149.0>>
	* uni1EE9: L<<813.0,1149.0>--<1253.0,1149.0>> -> L<<1253.0,1149.0>--<1253.0,1149.0>>
	* uni1EEB: L<<813.0,1149.0>--<1253.0,1149.0>> -> L<<1253.0,1149.0>--<1253.0,1149.0>>
	* uni1EED: L<<813.0,1149.0>--<1253.0,1149.0>> -> L<<1253.0,1149.0>--<1253.0,1149.0>>
	* uni1EEF: L<<813.0,1149.0>--<1253.0,1149.0>> -> L<<1253.0,1149.0>--<1253.0,1149.0>> and uni1EF1: L<<813.0,1149.0>--<1253.0,1149.0>> -> L<<1253.0,1149.0>--<1253.0,1149.0>> [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* R: L<<1075.0,697.0>--<1034.0,697.0>>/B<<1034.0,697.0>-<1160.0,675.0>-<1213.5,588.5>> = 9.904183212973862
	* Racute: L<<1075.0,697.0>--<1034.0,697.0>>/B<<1034.0,697.0>-<1160.0,675.0>-<1213.5,588.5>> = 9.904183212973862
	* Rcaron: L<<1075.0,697.0>--<1034.0,697.0>>/B<<1034.0,697.0>-<1160.0,675.0>-<1213.5,588.5>> = 9.904183212973862
	* braceleft.case: B<<512.5,824.5>-<448.0,755.0>-<308.0,750.0>>/B<<308.0,750.0>-<448.0,745.0>-<512.5,675.5>> = 4.0908169777744545
	* braceleft: B<<563.0,742.0>-<497.0,645.0>-<319.0,638.0>>/B<<319.0,638.0>-<497.0,631.0>-<563.0,534.5>> = 4.504088690805056
	* braceright.case: B<<341.0,675.5>-<406.0,745.0>-<546.0,750.0>>/B<<546.0,750.0>-<406.0,755.0>-<341.0,824.5>> = 4.0908169777744545
	* braceright: B<<386.0,534.5>-<452.0,631.0>-<630.0,638.0>>/B<<630.0,638.0>-<452.0,645.0>-<386.0,742.0>> = 4.504088690805056
	* eng: L<<549.0,1149.0>--<549.0,880.0>>/B<<549.0,880.0>-<582.0,1018.0>-<678.0,1093.0>> = 13.448615051686525
	* eth: B<<831.0,1055.5>-<927.0,1003.0>-<980.0,882.0>>/B<<980.0,882.0>-<960.0,996.0>-<923.5,1090.5>> = 13.703586662958596
	* m: L<<544.0,1149.0>--<544.0,892.0>>/B<<544.0,892.0>-<572.0,1022.0>-<657.0,1094.0>> = 12.154941697222226 and 36 more. [code: found-jaggy-segments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * k: L<<235.0,180.0>--<236.0,1397.0>>
 * k: L<<572.0,1576.0>--<571.0,601.0>>
 * uni0137: L<<235.0,180.0>--<236.0,1397.0>> and uni0137: L<<572.0,1576.0>--<571.0,601.0>> [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[9] MontaguSlab16pt-Thin.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Ensure Stylistic Sets have description.</summary>

* [com.google.fonts/check/stylisticset_description](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/stylisticset_description)
<pre>--- Rationale ---
Stylistic sets must provide description text. Programs such as InDesign,
TextEdit and Inkscape use that info to display to the users so that they know
what a given stylistic set offers.</pre>

* 🔥 **FAIL** The stylistic set ss01 lacks a description string on the 'name' table. [code: missing-description]

</details>
<details>
<summary>⚠ <b>WARN:</b> Stricter unitsPerEm criteria for Google Fonts. </summary>

* [com.google.fonts/check/unitsperem_strict](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/unitsperem_strict)
<pre>--- Rationale ---
Even though the OpenType spec allows unitsPerEm to be any value between 16 and
16384, the Google Fonts project aims at a narrower set of reasonable values.
The spec suggests usage of powers of two in order to get some performance
improvements on legacy renderers, so those values are acceptable.
But values of 500 or 1000 are also acceptable, with the added benefit that it
makes upm math easier for designers, while the performance hit of not using a
power of two is most likely negligible nowadays.
Additionally, values above 2048 would likely result in unreasonable filesize
increases.</pre>

* ⚠ **WARN** Font em size (unitsPerEm) is 2200 which may be too large (causing filesize bloat), unless you are sure that the detail level in this font requires that much precision. [code: large-value]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: ampersand	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: two	Contours detected: 2	Expected: 1
Glyph name: less	Contours detected: 0	Expected: 1
Glyph name: greater	Contours detected: 0	Expected: 1
Glyph name: at	Contours detected: 0	Expected: 2
Glyph name: Q	Contours detected: 3	Expected: 2
Glyph name: asciicircum	Contours detected: 0	Expected: 1
Glyph name: asciitilde	Contours detected: 0	Expected: 1
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
Glyph name: currency	Contours detected: 0	Expected: 2
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: copyright	Contours detected: 0	Expected: 3
Glyph name: logicalnot	Contours detected: 0	Expected: 1
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: uni00B2	Contours detected: 2	Expected: 1
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
Glyph name: uni2082	Contours detected: 2	Expected: 1
Glyph name: lira	Contours detected: 0	Expected: 1
Glyph name: uni20AD	Contours detected: 0	Expected: 1
Glyph name: uni20BA	Contours detected: 0	Expected: 1
Glyph name: uni20BC	Contours detected: 0	Expected: 1
Glyph name: approxequal	Contours detected: 0	Expected: 2
Glyph name: notequal	Contours detected: 0	Expected: 1
Glyph name: lessequal	Contours detected: 0	Expected: 2
Glyph name: greaterequal	Contours detected: 0	Expected: 2
Glyph name: uni27E8	Contours detected: 0	Expected: 1
Glyph name: uni27E9	Contours detected: 0	Expected: 1
Glyph name: Q	Contours detected: 3	Expected: 2
Glyph name: ampersand	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: approxequal	Contours detected: 0	Expected: 2
Glyph name: asciicircum	Contours detected: 0	Expected: 1
Glyph name: asciitilde	Contours detected: 0	Expected: 1
Glyph name: at	Contours detected: 0	Expected: 2
Glyph name: copyright	Contours detected: 0	Expected: 3
Glyph name: currency	Contours detected: 0	Expected: 2
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: greater	Contours detected: 0	Expected: 1
Glyph name: greaterequal	Contours detected: 0	Expected: 2
Glyph name: less	Contours detected: 0	Expected: 1
Glyph name: lessequal	Contours detected: 0	Expected: 2
Glyph name: lira	Contours detected: 0	Expected: 1
Glyph name: logicalnot	Contours detected: 0	Expected: 1
Glyph name: notequal	Contours detected: 0	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
Glyph name: two	Contours detected: 2	Expected: 1
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: uni20AD	Contours detected: 0	Expected: 1
Glyph name: uni20BA	Contours detected: 0	Expected: 1
Glyph name: uni20BC	Contours detected: 0	Expected: 1
Glyph name: uni27E8	Contours detected: 0	Expected: 1
Glyph name: uni27E9	Contours detected: 0	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Combined length of family and style must not exceed 27 characters.</summary>

* [com.google.fonts/check/name/family_and_style_max_length](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/family_and_style_max_length)
<pre>--- Rationale ---
According to a GlyphsApp tutorial [1], in order to make sure all versions of
Windows recognize it as a valid font file, we must make sure that the
concatenated length of the familyname (NameID.FONT_FAMILY_NAME) and style
(NameID.FONT_SUBFAMILY_NAME) strings in the name table do not exceed 20
characters.
After discussing the problem in more detail at `FontBakery issue #2179 [2] we
decided that allowing up to 27 chars would still be on the safe side, though.
[1] https://glyphsapp.com/tutorials/multiple-masters-part-3-setting-up-instances
[2] https://github.com/googlefonts/fontbakery/issues/2179</pre>

* ⚠ **WARN** The combined length of family and style exceeds 27 chars in the following 'WINDOWS' entries:
 FONT_FAMILY_NAME = 'Montagu Slab 16pt Thin' / SUBFAMILY_NAME = 'Regular'

Please take a look at the conversation at https://github.com/googlefonts/fontbakery/issues/2179 in order to understand the reasoning behind these name table records max-length criteria. [code: too-long]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking unitsPerEm value is reasonable.</summary>

* [com.google.fonts/check/unitsperem](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/head.html#com.google.fonts/check/unitsperem)
<pre>--- Rationale ---
According to the OpenType spec:
The value of unitsPerEm at the head table must be a value between 16 and 16384.
Any value in this range is valid.
In fonts that have TrueType outlines, a power of 2 is recommended as this allows
performance optimizations in some rasterizers.
But 1000 is a commonly used value. And 2000 may become increasingly more common
on Variable Fonts.</pre>

* ⚠ **WARN** In order to optimize performance on some legacy renderers, the value of unitsPerEm at the head table should idealy be a power of between 16 to 16384. And values of 1000 and 2000 are also common and may be just fine as well. But we got 2200 instead. [code: suboptimal]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there any misaligned on-curve points?</summary>

* [com.google.fonts/check/outline_alignment_miss](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_alignment_miss)
<pre>--- Rationale ---
This check heuristically looks for on-curve points which are close to, but do
not sit on, significant boundary coordinates. For example, a point which has a
Y-coordinate of 1 or -1 might be a misplaced baseline point. As well as the
baseline, here we also check for points near the x-height (but only for lower
case Latin letters), cap-height, ascender and descender Y coordinates.
Not all such misaligned curve points are a mistake, and sometimes the design may
call for points in locations near the boundaries. As this check is liable to
generate significant numbers of false positives, it will pass if there are more
than 100 reported misalignments.</pre>

* ⚠ **WARN** The following glyphs have on-curve points which have potentially incorrect y coordinates:
	* uni1EB4: X=650.0,Y=2158.0 (should be at ascender 2160?)
	* uni1EAA: X=650.0,Y=2158.0 (should be at ascender 2160?)
	* uni1EC4: X=591.0,Y=2158.0 (should be at ascender 2160?)
	* uni1ED6: X=691.0,Y=2158.0 (should be at ascender 2160?)
	* Q: X=1154.0,Y=-2.0 (should be at baseline 0?)
	* Uogonek: X=1124.0,Y=-1.0 (should be at baseline 0?)
	* uni1EA3: X=774.0,Y=1498.0 (should be at cap-height 1500?)
	* uni1EA3: X=554.0,Y=1498.0 (should be at cap-height 1500?)
	* uni1EBB: X=778.0,Y=1498.0 (should be at cap-height 1500?)
	* uni1EBB: X=558.0,Y=1498.0 (should be at cap-height 1500?) and 39 more. [code: found-misalignments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* braceleft.case: B<<375.5,818.5>-<314.0,756.0>-<210.0,750.0>>/B<<210.0,750.0>-<314.0,744.0>-<375.5,681.5>> = 6.603731348869935
	* braceleft: B<<409.5,707.5>-<341.0,637.0>-<228.0,630.0>>/B<<228.0,630.0>-<341.0,623.0>-<409.5,553.0>> = 7.089532911189703
	* braceright.case: B<<440.0,681.5>-<502.0,744.0>-<605.0,750.0>>/B<<605.0,750.0>-<502.0,756.0>-<440.0,818.5>> = 6.667701323073103
	* braceright: B<<481.5,553.0>-<550.0,623.0>-<663.0,630.0>>/B<<663.0,630.0>-<550.0,637.0>-<481.5,707.5>> = 7.089532911189703
	* eth: B<<910.5,1053.5>-<1024.0,991.0>-<1085.0,864.0>>/B<<1085.0,864.0>-<1049.0,1006.0>-<982.5,1121.5>> = 11.42970682912706
	* nine.dnom: B<<582.0,204.5>-<618.0,295.0>-<610.0,439.0>>/B<<610.0,439.0>-<600.0,369.0>-<536.0,315.5>> = 11.309932474020162
	* nine.lf: B<<1128.5,553.5>-<1166.0,742.0>-<1145.0,1014.0>>/B<<1145.0,1014.0>-<1132.0,811.0>-<1003.0,687.0>> = 8.078997569467882
	* nine.numr: B<<582.0,981.5>-<618.0,1072.0>-<610.0,1216.0>>/B<<610.0,1216.0>-<600.0,1146.0>-<536.0,1092.5>> = 11.309932474020162
	* nine: B<<1128.5,553.5>-<1166.0,742.0>-<1145.0,1014.0>>/B<<1145.0,1014.0>-<1132.0,811.0>-<1003.0,687.0>> = 8.078997569467882
	* six.dnom: B<<167.5,518.5>-<132.0,428.0>-<140.0,284.0>>/B<<140.0,284.0>-<151.0,354.0>-<214.5,407.5>> = 12.110420220283205 and 8 more. [code: found-jaggy-segments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * dotlessi.ss01: L<<268.0,203.0>--<269.0,1054.0>>
 * i.loclTRK.ss01: L<<268.0,203.0>--<269.0,1054.0>>
 * i.ss01: L<<268.0,203.0>--<269.0,1054.0>>
 * iacute.ss01: L<<268.0,203.0>--<269.0,1054.0>>
 * icircumflex.ss01: L<<268.0,203.0>--<269.0,1054.0>>
 * idieresis.ss01: L<<268.0,203.0>--<269.0,1054.0>>
 * igrave.ss01: L<<268.0,203.0>--<269.0,1054.0>>
 * imacron.ss01: L<<268.0,203.0>--<269.0,1054.0>>
 * l.ss01: L<<268.0,205.0>--<269.0,1513.0>>
 * lacute.ss01: L<<268.0,205.0>--<269.0,1513.0>> and 12 more. [code: found-semi-vertical]

</details>
<br>
</details>

### Summary

| 💔 ERROR | 🔥 FAIL | ⚠ WARN | 💤 SKIP | ℹ INFO | 🍞 PASS | 🔎 DEBUG |
|:-----:|:----:|:----:|:----:|:----:|:----:|:----:|
| 0 | 7 | 56 | 673 | 43 | 559 | 0 |
| 0% | 1% | 4% | 50% | 3% | 42% | 0% |

**Note:** The following loglevels were omitted in this report:
* **SKIP**
* **INFO**
* **PASS**
* **DEBUG**
