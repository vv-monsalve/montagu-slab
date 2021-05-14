## Fontbakery report

Fontbakery version: 0.7.35

<details>
<summary><b>[11] MontaguSlab16pt-Bold.ttf</b></summary>
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
<summary>🔥 <b>FAIL:</b> Checking with fontTools.ttx</summary>

* [com.google.fonts/check/ttx-roundtrip](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/ttx-roundtrip)

* 🔥 **FAIL** TTX had some problem parsing the generated XML file. This most likely mean there's some problem in the font. Please inspect the output of ttx in order to find more on what went wrong. A common problem is the presence of control characteres outside the accepted character range as defined in the XML spec. FontTools has got a bug which causes TTX to generate corrupt XML files in those cases. So, check the entries of the name table and remove any control chars that you find there. The full ttx error message was:
======
not well-formed (invalid token): line 55289, column 14
======

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
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
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
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
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
<summary>⚠ <b>WARN:</b> Check if OS/2 xAvgCharWidth is correct.</summary>

* [com.google.fonts/check/xavgcharwidth](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/os2.html#com.google.fonts/check/xavgcharwidth)

* ⚠ **WARN** OS/2 xAvgCharWidth is 1384 but it should be 1476 which corresponds to the average of the widths of all glyphs in the font. [code: xAvgCharWidth-wrong]

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
	* s: X=720.5,Y=1138.5 (should be at x-height 1140?)
	* t: X=40.0,Y=1142.0 (should be at x-height 1140?)
	* t: X=60.0,Y=1142.0 (should be at x-height 1140?)
	* one.numr: X=301.0,Y=1498.0 (should be at cap-height 1500?)
	* uni00B9: X=301.0,Y=1498.0 (should be at cap-height 1500?)
	* onehalf: X=301.0,Y=1498.0 (should be at cap-height 1500?)
	* onequarter: X=301.0,Y=1498.0 (should be at cap-height 1500?)
	* questiondown: X=436.0,Y=-2.0 (should be at baseline 0?)
	* colonmonetary: X=607.0,Y=-1.0 (should be at baseline 0?) and uni20B2: X=1104.0,Y=1501.0 (should be at cap-height 1500?) [code: found-misalignments]

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
	* Itilde: L<<475.0,1875.0>--<475.0,1875.0>> -> L<<475.0,1875.0>--<475.0,1875.0>>
	* Ntilde: L<<965.0,1875.0>--<965.0,1875.0>> -> L<<965.0,1875.0>--<965.0,1875.0>>
	* Otilde: L<<993.0,1875.0>--<993.0,1875.0>> -> L<<993.0,1875.0>--<993.0,1875.0>>
	* itilde: L<<454.0,1535.0>--<454.0,1535.0>> -> L<<454.0,1535.0>--<454.0,1535.0>>
	* ntilde: L<<798.0,1535.0>--<798.0,1535.0>> -> L<<798.0,1535.0>--<798.0,1535.0>>
	* uni022C: L<<993.0,1875.0>--<993.0,1875.0>> -> L<<993.0,1875.0>--<993.0,1875.0>>
	* uni1EBC: L<<864.0,1875.0>--<864.0,1875.0>> -> L<<864.0,1875.0>--<864.0,1875.0>>
	* uni1EC4: L<<864.0,2285.0>--<864.0,2285.0>> -> L<<864.0,2285.0>--<864.0,2285.0>>
	* uni1ED6: L<<993.0,2285.0>--<993.0,2285.0>> -> L<<993.0,2285.0>--<993.0,2285.0>>
	* uni1EEE: L<<1022.0,1875.0>--<1022.0,1875.0>> -> L<<1022.0,1875.0>--<1022.0,1875.0>> and utilde: L<<803.0,1535.0>--<803.0,1535.0>> -> L<<803.0,1535.0>--<803.0,1535.0>> [code: found-colinear-vectors]

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
	* R: L<<1099.0,696.0>--<1068.0,696.0>>/B<<1068.0,696.0>-<1181.0,680.0>-<1234.0,614.0>> = 8.059103902870945
	* Racute: L<<1099.0,696.0>--<1068.0,696.0>>/B<<1068.0,696.0>-<1181.0,680.0>-<1234.0,614.0>> = 8.059103902870945
	* Rcaron: L<<1099.0,696.0>--<1068.0,696.0>>/B<<1068.0,696.0>-<1181.0,680.0>-<1234.0,614.0>> = 8.059103902870945
	* braceleft.case: B<<544.0,826.0>-<479.0,755.0>-<330.0,750.0>>/B<<330.0,750.0>-<479.0,745.0>-<544.0,674.0>> = 3.843911917862876
	* braceleft: B<<539.0,692.5>-<469.0,645.0>-<340.0,640.0>>/B<<340.0,640.0>-<469.0,635.0>-<539.0,587.5>> = 4.4393111063957145
	* braceright.case: B<<318.5,674.0>-<384.0,745.0>-<532.0,750.0>>/B<<532.0,750.0>-<384.0,755.0>-<318.5,826.0>> = 3.869864619105556
	* braceright: B<<423.5,587.5>-<494.0,635.0>-<622.0,640.0>>/B<<622.0,640.0>-<494.0,645.0>-<423.5,692.5>> = 4.473958126875278
	* eng: L<<591.0,1160.0>--<591.0,893.0>>/B<<591.0,893.0>-<599.0,929.0>-<610.0,961.0>> = 12.528807709151492
	* m: L<<585.0,1160.0>--<585.0,885.0>>/B<<585.0,885.0>-<592.0,927.0>-<604.0,964.0>> = 9.462322208025613
	* n: L<<591.0,1160.0>--<591.0,893.0>>/B<<591.0,893.0>-<599.0,929.0>-<610.0,961.0>> = 12.528807709151492 and 35 more. [code: found-jaggy-segments]

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
<summary><b>[12] MontaguSlab16pt-ExtraLight.ttf</b></summary>
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
<summary>🔥 <b>FAIL:</b> Checking with fontTools.ttx</summary>

* [com.google.fonts/check/ttx-roundtrip](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/ttx-roundtrip)

* 🔥 **FAIL** TTX had some problem parsing the generated XML file. This most likely mean there's some problem in the font. Please inspect the output of ttx in order to find more on what went wrong. A common problem is the presence of control characteres outside the accepted character range as defined in the XML spec. FontTools has got a bug which causes TTX to generate corrupt XML files in those cases. So, check the entries of the name table and remove any control chars that you find there. The full ttx error message was:
======
not well-formed (invalid token): line 51456, column 14
======

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
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
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
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
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
<summary>⚠ <b>WARN:</b> Check if OS/2 xAvgCharWidth is correct.</summary>

* [com.google.fonts/check/xavgcharwidth](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/os2.html#com.google.fonts/check/xavgcharwidth)

* ⚠ **WARN** OS/2 xAvgCharWidth is 1384 but it should be 1345 which corresponds to the average of the widths of all glyphs in the font. [code: xAvgCharWidth-wrong]

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
	* uni1EB4: X=955.0,Y=2160.5 (should be at ascender 2160?)
	* uni1EA4: X=1275.0,Y=2159.0 (should be at ascender 2160?)
	* uni1EA4: X=1369.0,Y=2159.0 (should be at ascender 2160?)
	* uni1EA6: X=1036.0,Y=2159.0 (should be at ascender 2160?)
	* uni1EA6: X=1130.0,Y=2159.0 (should be at ascender 2160?)
	* uni1EAA: X=602.0,Y=2159.0 (should be at ascender 2160?)
	* uni1EAA: X=955.0,Y=2160.5 (should be at ascender 2160?)
	* uni1EBE: X=1211.0,Y=2159.0 (should be at ascender 2160?)
	* uni1EBE: X=1305.0,Y=2159.0 (should be at ascender 2160?) and 82 more. [code: found-misalignments]

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
	* Itilde: L<<378.0,1805.0>--<378.0,1805.0>> -> L<<378.0,1805.0>--<378.0,1805.0>>
	* Ntilde: L<<931.0,1805.0>--<931.0,1805.0>> -> L<<931.0,1805.0>--<931.0,1805.0>>
	* Otilde: L<<926.0,1805.0>--<926.0,1805.0>> -> L<<926.0,1805.0>--<926.0,1805.0>>
	* itilde: L<<346.0,1413.0>--<346.0,1413.0>> -> L<<346.0,1413.0>--<347.0,1413.0>>
	* ntilde: L<<724.0,1413.0>--<724.0,1413.0>> -> L<<724.0,1413.0>--<724.0,1413.0>>
	* uni022C: L<<926.0,1805.0>--<926.0,1805.0>> -> L<<926.0,1805.0>--<926.0,1805.0>>
	* uni1EBC: L<<822.0,1805.0>--<822.0,1805.0>> -> L<<822.0,1805.0>--<822.0,1805.0>>
	* uni1EC4: L<<822.0,2240.0>--<822.0,2240.0>> -> L<<822.0,2240.0>--<822.0,2240.0>>
	* uni1ED6: L<<926.0,2240.0>--<926.0,2240.0>> -> L<<926.0,2240.0>--<926.0,2240.0>>
	* uni1EEE: L<<952.0,1805.0>--<952.0,1805.0>> -> L<<952.0,1805.0>--<952.0,1805.0>> and utilde: L<<682.0,1413.0>--<682.0,1413.0>> -> L<<682.0,1413.0>--<683.0,1413.0>> [code: found-colinear-vectors]

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
	* braceleft: B<<384.0,670.0>-<326.0,636.0>-<243.0,631.0>>/B<<243.0,631.0>-<326.0,627.0>-<384.0,592.5>> = 6.206494510485443
	* braceright.case: B<<423.5,680.5>-<486.0,744.0>-<595.0,750.0>>/B<<595.0,750.0>-<486.0,756.0>-<423.5,819.5>> = 6.301432826535456
	* braceright: B<<517.0,592.5>-<575.0,627.0>-<658.0,631.0>>/B<<658.0,631.0>-<575.0,636.0>-<517.0,670.0>> = 6.206494510485443
	* eth: B<<1067.0,869.0>-<1069.0,866.0>-<1070.0,864.0>>/B<<1070.0,864.0>-<1053.0,936.0>-<1028.0,1000.0>> = 13.280184692175785
	* nine.lf: B<<1107.0,548.0>-<1143.0,726.0>-<1123.0,979.0>>/B<<1123.0,979.0>-<1106.0,792.0>-<982.0,676.5>> = 9.714340022270003
	* nine: B<<1107.0,548.0>-<1143.0,726.0>-<1123.0,979.0>>/B<<1123.0,979.0>-<1106.0,792.0>-<982.0,676.5>> = 9.714340022270003
	* six.lf: B<<263.0,952.0>-<227.0,774.0>-<247.0,521.0>>/B<<247.0,521.0>-<264.0,708.0>-<388.0,823.5>> = 9.714340022270003
	* six: B<<263.0,952.0>-<227.0,774.0>-<247.0,521.0>>/B<<247.0,521.0>-<264.0,708.0>-<388.0,823.5>> = 9.714340022270003 and yen: L<<803.0,592.0>--<669.0,779.0>>/L<<669.0,779.0>--<680.0,761.0>> = 4.194967764236985 [code: found-jaggy-segments]

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
<summary><b>[12] MontaguSlab16pt-Light.ttf</b></summary>
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
<summary>🔥 <b>FAIL:</b> Checking with fontTools.ttx</summary>

* [com.google.fonts/check/ttx-roundtrip](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/ttx-roundtrip)

* 🔥 **FAIL** TTX had some problem parsing the generated XML file. This most likely mean there's some problem in the font. Please inspect the output of ttx in order to find more on what went wrong. A common problem is the presence of control characteres outside the accepted character range as defined in the XML spec. FontTools has got a bug which causes TTX to generate corrupt XML files in those cases. So, check the entries of the name table and remove any control chars that you find there. The full ttx error message was:
======
not well-formed (invalid token): line 51406, column 14
======

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
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
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
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
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
<summary>⚠ <b>WARN:</b> Check if OS/2 xAvgCharWidth is correct.</summary>

* [com.google.fonts/check/xavgcharwidth](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/os2.html#com.google.fonts/check/xavgcharwidth)

* ⚠ **WARN** OS/2 xAvgCharWidth is 1384 but it should be 1365 which corresponds to the average of the widths of all glyphs in the font. [code: xAvgCharWidth-wrong]

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
	* Racute: X=1005.0,Y=1502.0 (should be at cap-height 1500?) and 30 more. [code: found-misalignments]

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
	* four.lf: L<<824.0,1500.0>--<824.0,1500.0>> -> L<<824.0,1500.0>--<970.0,1500.0>>
	* four: L<<824.0,1500.0>--<824.0,1500.0>> -> L<<824.0,1500.0>--<970.0,1500.0>>
	* uni1EC4: L<<829.0,2247.0>--<829.0,2247.0>> -> L<<829.0,2247.0>--<829.0,2247.0>> and uni1ED6: L<<936.0,2247.0>--<936.0,2247.0>> -> L<<936.0,2247.0>--<937.0,2247.0>> [code: found-colinear-vectors]

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
	* braceleft.case: B<<420.5,820.5>-<358.0,756.0>-<242.0,750.0>>/B<<242.0,750.0>-<358.0,744.0>-<420.5,679.5>> = 5.921872268327562
	* braceleft: B<<407.5,674.0>-<348.0,638.0>-<258.0,633.0>>/B<<258.0,633.0>-<348.0,628.0>-<407.5,591.5>> = 6.359660239728424
	* braceright.case: B<<408.0,679.5>-<471.0,744.0>-<586.0,750.0>>/B<<586.0,750.0>-<471.0,756.0>-<408.0,820.5>> = 5.973273980950297
	* braceright: B<<502.5,591.5>-<563.0,628.0>-<652.0,633.0>>/B<<652.0,633.0>-<563.0,638.0>-<502.5,674.0>> = 6.430967983496417
	* nine.lf: B<<1085.0,542.5>-<1119.0,709.0>-<1102.0,945.0>>/B<<1102.0,945.0>-<1080.0,772.0>-<961.0,665.0>> = 11.367390806004797
	* nine: B<<1085.0,542.5>-<1119.0,709.0>-<1102.0,945.0>>/B<<1102.0,945.0>-<1080.0,772.0>-<961.0,665.0>> = 11.367390806004797
	* six.lf: B<<304.0,957.5>-<270.0,791.0>-<287.0,555.0>>/B<<287.0,555.0>-<309.0,728.0>-<428.0,835.0>> = 11.367390806004797 and six: B<<304.0,957.5>-<270.0,791.0>-<287.0,555.0>>/B<<287.0,555.0>-<309.0,728.0>-<428.0,835.0>> = 11.367390806004797 [code: found-jaggy-segments]

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
<summary><b>[11] MontaguSlab16pt-Medium.ttf</b></summary>
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
<summary>🔥 <b>FAIL:</b> Checking with fontTools.ttx</summary>

* [com.google.fonts/check/ttx-roundtrip](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/ttx-roundtrip)

* 🔥 **FAIL** TTX had some problem parsing the generated XML file. This most likely mean there's some problem in the font. Please inspect the output of ttx in order to find more on what went wrong. A common problem is the presence of control characteres outside the accepted character range as defined in the XML spec. FontTools has got a bug which causes TTX to generate corrupt XML files in those cases. So, check the entries of the name table and remove any control chars that you find there. The full ttx error message was:
======
not well-formed (invalid token): line 53615, column 14
======

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
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
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
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
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
<summary>⚠ <b>WARN:</b> Check if OS/2 xAvgCharWidth is correct.</summary>

* [com.google.fonts/check/xavgcharwidth](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/os2.html#com.google.fonts/check/xavgcharwidth)

* ⚠ **WARN** OS/2 xAvgCharWidth is 1384 but it should be 1423 which corresponds to the average of the widths of all glyphs in the font. [code: xAvgCharWidth-wrong]

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
	* f: X=56.0,Y=1139.0 (should be at x-height 1140?)
	* f: X=308.0,Y=1139.0 (should be at x-height 1140?)
	* f: X=589.0,Y=1139.0 (should be at x-height 1140?)
	* f: X=947.0,Y=1139.0 (should be at x-height 1140?)
	* g: X=324.0,Y=2.0 (should be at baseline 0?) and 72 more. [code: found-misalignments]

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
	* Itilde: L<<436.0,1847.0>--<436.0,1847.0>> -> L<<436.0,1847.0>--<436.0,1847.0>>
	* Ntilde: L<<951.0,1847.0>--<951.0,1847.0>> -> L<<951.0,1847.0>--<951.0,1847.0>>
	* Otilde: L<<966.0,1847.0>--<966.0,1847.0>> -> L<<966.0,1847.0>--<966.0,1847.0>>
	* four.lf: L<<759.0,1500.0>--<759.0,1500.0>> -> L<<759.0,1500.0>--<1030.0,1500.0>>
	* four: L<<759.0,1500.0>--<759.0,1500.0>> -> L<<759.0,1500.0>--<1030.0,1500.0>>
	* itilde: L<<411.0,1486.0>--<411.0,1486.0>> -> L<<411.0,1486.0>--<411.0,1486.0>>
	* ntilde: L<<768.0,1486.0>--<768.0,1486.0>> -> L<<768.0,1486.0>--<769.0,1486.0>>
	* uni022C: L<<966.0,1847.0>--<966.0,1847.0>> -> L<<966.0,1847.0>--<966.0,1847.0>>
	* uni1EBC: L<<847.0,1847.0>--<847.0,1847.0>> -> L<<847.0,1847.0>--<847.0,1847.0>>
	* uni1EC4: L<<847.0,2267.0>--<847.0,2267.0>> -> L<<847.0,2267.0>--<847.0,2267.0>> and 3 more. [code: found-colinear-vectors]

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
	* R: L<<1055.0,698.0>--<1007.0,698.0>>/B<<1007.0,698.0>-<1106.0,678.0>-<1158.0,617.0>> = 11.421186274999258
	* Racute: L<<1055.0,698.0>--<1007.0,698.0>>/B<<1007.0,698.0>-<1106.0,678.0>-<1158.0,617.0>> = 11.421186274999258
	* Rcaron: L<<1055.0,698.0>--<1007.0,698.0>>/B<<1007.0,698.0>-<1106.0,678.0>-<1158.0,617.0>> = 11.421186274999258
	* braceleft.case: B<<485.5,823.0>-<422.0,755.0>-<288.0,750.0>>/B<<288.0,750.0>-<422.0,745.0>-<485.5,677.0>> = 4.273821707514343
	* braceleft: B<<477.0,684.0>-<412.0,642.0>-<301.0,637.0>>/B<<301.0,637.0>-<412.0,632.0>-<477.0,589.5>> = 5.158295000566781
	* braceright.case: B<<360.5,677.0>-<425.0,745.0>-<557.0,750.0>>/B<<557.0,750.0>-<425.0,755.0>-<360.5,823.0>> = 4.338515179456888
	* braceright: B<<461.0,589.5>-<527.0,632.0>-<636.0,637.0>>/B<<636.0,637.0>-<527.0,642.0>-<461.0,684.0>> = 5.252811276581354
	* eth: B<<848.0,1054.0>-<947.0,998.0>-<1001.0,877.0>>/B<<1001.0,877.0>-<989.0,944.0>-<970.0,1004.0>> = 13.896031949404886
	* m: L<<509.0,1139.0>--<509.0,889.0>>/B<<509.0,889.0>-<517.0,922.0>-<528.0,950.0>> = 13.62699485989153
	* uni0156: L<<1055.0,698.0>--<1007.0,698.0>>/B<<1007.0,698.0>-<1106.0,678.0>-<1158.0,617.0>> = 11.421186274999258 and 5 more. [code: found-jaggy-segments]

</details>
<br>
</details>
<details>
<summary><b>[11] MontaguSlab16pt-Regular.ttf</b></summary>
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
<summary>🔥 <b>FAIL:</b> Checking with fontTools.ttx</summary>

* [com.google.fonts/check/ttx-roundtrip](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/ttx-roundtrip)

* 🔥 **FAIL** TTX had some problem parsing the generated XML file. This most likely mean there's some problem in the font. Please inspect the output of ttx in order to find more on what went wrong. A common problem is the presence of control characteres outside the accepted character range as defined in the XML spec. FontTools has got a bug which causes TTX to generate corrupt XML files in those cases. So, check the entries of the name table and remove any control chars that you find there. The full ttx error message was:
======
not well-formed (invalid token): line 54844, column 14
======

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
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
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
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
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
<summary>⚠ <b>WARN:</b> Check if OS/2 xAvgCharWidth is correct.</summary>

* [com.google.fonts/check/xavgcharwidth](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/os2.html#com.google.fonts/check/xavgcharwidth)

* ⚠ **WARN** OS/2 xAvgCharWidth is 1384 but it should be 1395 which corresponds to the average of the widths of all glyphs in the font. [code: xAvgCharWidth-wrong]

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
	* Uogonek: X=1155.0,Y=2.0 (should be at baseline 0?)
	* adieresis: X=351.5,Y=1498.0 (should be at cap-height 1500?)
	* adieresis: X=532.5,Y=1498.0 (should be at cap-height 1500?)
	* adieresis: X=804.5,Y=1498.0 (should be at cap-height 1500?)
	* adieresis: X=984.5,Y=1498.0 (should be at cap-height 1500?)
	* uni0203: X=433.5,Y=1500.5 (should be at cap-height 1500?)
	* uni0203: X=905.5,Y=1500.5 (should be at cap-height 1500?)
	* edieresis: X=335.0,Y=1498.0 (should be at cap-height 1500?)
	* edieresis: X=515.5,Y=1498.0 (should be at cap-height 1500?)
	* edieresis: X=788.0,Y=1498.0 (should be at cap-height 1500?) and 49 more. [code: found-misalignments]

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
	* bracketleft.case: L<<222.0,-60.0>--<222.0,1433.0>> -> L<<222.0,1433.0>--<222.0,1560.0>>
	* four.lf: L<<791.0,1500.0>--<791.0,1500.0>> -> L<<791.0,1500.0>--<1000.0,1500.0>>
	* four: L<<791.0,1500.0>--<791.0,1500.0>> -> L<<791.0,1500.0>--<1000.0,1500.0>>
	* itilde: L<<387.0,1459.0>--<387.0,1459.0>> -> L<<387.0,1459.0>--<387.0,1459.0>>
	* ntilde: L<<752.0,1459.0>--<752.0,1459.0>> -> L<<752.0,1459.0>--<752.0,1459.0>>
	* uni1EC4: L<<838.0,2257.0>--<838.0,2257.0>> -> L<<838.0,2257.0>--<838.0,2257.0>>
	* uni1ED6: L<<951.0,2257.0>--<952.0,2257.0>> -> L<<952.0,2257.0>--<952.0,2257.0>> and utilde: L<<728.0,1459.0>--<728.0,1459.0>> -> L<<728.0,1459.0>--<728.0,1459.0>> [code: found-colinear-vectors]

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
	* R: L<<1031.0,699.0>--<972.0,699.0>>/B<<972.0,699.0>-<1065.0,678.0>-<1116.0,619.0>> = 12.724355685422363
	* Racute: L<<1031.0,699.0>--<972.0,699.0>>/B<<972.0,699.0>-<1065.0,678.0>-<1116.0,619.0>> = 12.724355685422363
	* Rcaron: L<<1031.0,699.0>--<972.0,699.0>>/B<<972.0,699.0>-<1065.0,678.0>-<1116.0,619.0>> = 12.724355685422363
	* braceleft.case: B<<453.5,822.0>-<390.0,756.0>-<266.0,750.0>>/B<<266.0,750.0>-<390.0,744.0>-<453.5,678.0>> = 5.540431594400349
	* braceleft: B<<442.5,679.0>-<380.0,640.0>-<280.0,635.0>>/B<<280.0,635.0>-<380.0,630.0>-<442.5,590.5>> = 5.72481045222338
	* braceright.case: B<<383.5,678.0>-<447.0,744.0>-<571.0,750.0>>/B<<571.0,750.0>-<447.0,756.0>-<383.5,822.0>> = 5.540431594400349
	* braceright: B<<481.0,590.5>-<544.0,630.0>-<644.0,635.0>>/B<<644.0,635.0>-<544.0,640.0>-<481.0,679.0>> = 5.72481045222338
	* eth: B<<866.0,1054.0>-<969.0,996.0>-<1026.0,872.0>>/B<<1026.0,872.0>-<1012.0,941.0>-<991.0,1002.0>> = 13.217643396925702
	* uni0156: L<<1031.0,699.0>--<972.0,699.0>>/B<<972.0,699.0>-<1065.0,678.0>-<1116.0,619.0>> = 12.724355685422363
	* uni0210: L<<1031.0,699.0>--<972.0,699.0>>/B<<972.0,699.0>-<1065.0,678.0>-<1116.0,619.0>> = 12.724355685422363 and 3 more. [code: found-jaggy-segments]

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
 * k: L<<258.0,123.0>--<259.0,1446.0>> [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[12] MontaguSlab16pt-SemiBold.ttf</b></summary>
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
<summary>🔥 <b>FAIL:</b> Checking with fontTools.ttx</summary>

* [com.google.fonts/check/ttx-roundtrip](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/ttx-roundtrip)

* 🔥 **FAIL** TTX had some problem parsing the generated XML file. This most likely mean there's some problem in the font. Please inspect the output of ttx in order to find more on what went wrong. A common problem is the presence of control characteres outside the accepted character range as defined in the XML spec. FontTools has got a bug which causes TTX to generate corrupt XML files in those cases. So, check the entries of the name table and remove any control chars that you find there. The full ttx error message was:
======
not well-formed (invalid token): line 56637, column 14
======

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
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
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
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
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
<summary>⚠ <b>WARN:</b> Check if OS/2 xAvgCharWidth is correct.</summary>

* [com.google.fonts/check/xavgcharwidth](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/os2.html#com.google.fonts/check/xavgcharwidth)

* ⚠ **WARN** OS/2 xAvgCharWidth is 1384 but it should be 1448 which corresponds to the average of the widths of all glyphs in the font. [code: xAvgCharWidth-wrong]

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
	* a: X=459.5,Y=1141.5 (should be at x-height 1140?)
	* v: X=559.0,Y=-2.0 (should be at baseline 0?)
	* v: X=841.0,Y=-2.0 (should be at baseline 0?)
	* w: X=1236.0,Y=-2.0 (should be at baseline 0?)
	* w: X=793.0,Y=-2.0 (should be at baseline 0?)
	* w: X=520.0,Y=-2.0 (should be at baseline 0?)
	* w: X=1507.0,Y=-2.0 (should be at baseline 0?)
	* wacute: X=1236.0,Y=-2.0 (should be at baseline 0?)
	* wacute: X=793.0,Y=-2.0 (should be at baseline 0?) and 30 more. [code: found-misalignments]

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
	* Itilde: L<<454.0,1860.0>--<454.0,1860.0>> -> L<<454.0,1860.0>--<454.0,1860.0>>
	* Ntilde: L<<957.0,1860.0>--<958.0,1860.0>> -> L<<958.0,1860.0>--<958.0,1860.0>>
	* Otilde: L<<978.0,1860.0>--<979.0,1860.0>> -> L<<979.0,1860.0>--<979.0,1860.0>>
	* four.lf: L<<732.0,1500.0>--<732.0,1500.0>> -> L<<732.0,1500.0>--<1055.0,1500.0>>
	* four: L<<732.0,1500.0>--<732.0,1500.0>> -> L<<732.0,1500.0>--<1055.0,1500.0>>
	* itilde: L<<431.0,1509.0>--<431.0,1509.0>> -> L<<431.0,1509.0>--<431.0,1509.0>>
	* ntilde: L<<782.0,1509.0>--<782.0,1509.0>> -> L<<782.0,1509.0>--<782.0,1509.0>>
	* uhorn: L<<813.0,1149.0>--<1253.0,1149.0>> -> L<<1253.0,1149.0>--<1253.0,1149.0>>
	* uni022C: L<<978.0,1860.0>--<979.0,1860.0>> -> L<<979.0,1860.0>--<979.0,1860.0>>
	* uni1EBC: L<<855.0,1860.0>--<855.0,1860.0>> -> L<<855.0,1860.0>--<855.0,1860.0>> and 9 more. [code: found-colinear-vectors]

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
	* R: L<<1075.0,697.0>--<1036.0,697.0>>/B<<1036.0,697.0>-<1141.0,679.0>-<1193.0,615.0>> = 9.727578551401587
	* Racute: L<<1075.0,697.0>--<1036.0,697.0>>/B<<1036.0,697.0>-<1141.0,679.0>-<1193.0,615.0>> = 9.727578551401587
	* Rcaron: L<<1075.0,697.0>--<1036.0,697.0>>/B<<1036.0,697.0>-<1141.0,679.0>-<1193.0,615.0>> = 9.727578551401587
	* braceleft.case: B<<512.5,824.5>-<448.0,755.0>-<308.0,750.0>>/B<<308.0,750.0>-<448.0,745.0>-<512.5,675.5>> = 4.0908169777744545
	* braceleft: B<<505.5,687.5>-<438.0,643.0>-<319.0,638.0>>/B<<319.0,638.0>-<438.0,633.0>-<505.5,588.5>> = 4.8119410332905534
	* braceright.case: B<<341.0,675.5>-<406.0,745.0>-<546.0,750.0>>/B<<546.0,750.0>-<406.0,755.0>-<341.0,824.5>> = 4.0908169777744545
	* braceright: B<<444.0,588.5>-<512.0,633.0>-<630.0,638.0>>/B<<630.0,638.0>-<512.0,643.0>-<444.0,687.5>> = 4.85267166320457
	* eng: L<<549.0,1149.0>--<549.0,876.0>>/B<<549.0,876.0>-<558.0,913.0>-<570.0,946.0>> = 13.67130713219584
	* eth: B<<834.0,1053.0>-<928.0,1000.0>-<981.0,880.0>>/B<<981.0,880.0>-<969.0,946.0>-<952.0,1005.0>> = 13.524603009198803
	* h: L<<579.0,1576.0>--<579.0,927.0>>/B<<579.0,927.0>-<581.0,935.0>-<584.0,942.0>> = 14.036243467926484 and 47 more. [code: found-jaggy-segments]

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
<summary><b>[12] MontaguSlab16pt-Thin.ttf</b></summary>
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
<summary>🔥 <b>FAIL:</b> Checking with fontTools.ttx</summary>

* [com.google.fonts/check/ttx-roundtrip](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/ttx-roundtrip)

* 🔥 **FAIL** TTX had some problem parsing the generated XML file. This most likely mean there's some problem in the font. Please inspect the output of ttx in order to find more on what went wrong. A common problem is the presence of control characteres outside the accepted character range as defined in the XML spec. FontTools has got a bug which causes TTX to generate corrupt XML files in those cases. So, check the entries of the name table and remove any control chars that you find there. The full ttx error message was:
======
not well-formed (invalid token): line 50848, column 14
======

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
Glyph name: uni00B5	Contours detected: 0	Expected: 1
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: germandbls	Contours detected: 0	Expected: 1
Glyph name: uni018F	Contours detected: 0	Expected: 2
Glyph name: uni1E9E	Contours detected: 0	Expected: 1
Glyph name: dagger	Contours detected: 0	Expected: 1 or 2
Glyph name: daggerdbl	Contours detected: 0	Expected: 1 or 3
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
Glyph name: paragraph	Contours detected: 0	Expected: 1, 2 or 3
Glyph name: registered	Contours detected: 0	Expected: 3 or 4
Glyph name: section	Contours detected: 0	Expected: 2
Glyph name: sterling	Contours detected: 0	Expected: 1 or 2
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
<summary>⚠ <b>WARN:</b> Check if OS/2 xAvgCharWidth is correct.</summary>

* [com.google.fonts/check/xavgcharwidth](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/os2.html#com.google.fonts/check/xavgcharwidth)

* ⚠ **WARN** OS/2 xAvgCharWidth is 1384 but it should be 1325 which corresponds to the average of the widths of all glyphs in the font. [code: xAvgCharWidth-wrong]

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
	* Uogonek: X=1123.0,Y=-2.0 (should be at baseline 0?)
	* uni1EA3: X=774.0,Y=1498.0 (should be at cap-height 1500?)
	* uni1EA3: X=554.0,Y=1498.0 (should be at cap-height 1500?)
	* uni1EBB: X=778.0,Y=1498.0 (should be at cap-height 1500?)
	* uni1EBB: X=558.0,Y=1498.0 (should be at cap-height 1500?) and 27 more. [code: found-misalignments]

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
	* Itilde: L<<363.0,1794.0>--<363.0,1794.0>> -> L<<363.0,1794.0>--<363.0,1794.0>>
	* Ntilde: L<<926.0,1794.0>--<926.0,1794.0>> -> L<<926.0,1794.0>--<926.0,1794.0>>
	* Otilde: L<<916.0,1794.0>--<916.0,1794.0>> -> L<<916.0,1794.0>--<916.0,1794.0>>
	* itilde: L<<330.0,1394.0>--<330.0,1394.0>> -> L<<330.0,1394.0>--<330.0,1394.0>>
	* ntilde: L<<713.0,1394.0>--<713.0,1394.0>> -> L<<713.0,1394.0>--<713.0,1394.0>>
	* uni022C: L<<916.0,1794.0>--<916.0,1794.0>> -> L<<916.0,1794.0>--<916.0,1794.0>>
	* uni1EBC: L<<816.0,1794.0>--<816.0,1794.0>> -> L<<816.0,1794.0>--<816.0,1794.0>>
	* uni1EC4: L<<816.0,2233.0>--<816.0,2233.0>> -> L<<816.0,2233.0>--<816.0,2233.0>>
	* uni1ED6: L<<916.0,2233.0>--<916.0,2233.0>> -> L<<916.0,2233.0>--<916.0,2233.0>>
	* uni1EEE: L<<941.0,1794.0>--<941.0,1794.0>> -> L<<941.0,1794.0>--<941.0,1794.0>> and utilde: L<<664.0,1394.0>--<664.0,1394.0>> -> L<<664.0,1394.0>--<664.0,1394.0>> [code: found-colinear-vectors]

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
	* braceleft: B<<360.0,667.0>-<304.0,635.0>-<228.0,630.0>>/B<<228.0,630.0>-<304.0,626.0>-<360.0,593.5>> = 6.7768223690890075
	* braceright.case: B<<440.0,681.5>-<502.0,744.0>-<605.0,750.0>>/B<<605.0,750.0>-<502.0,756.0>-<440.0,818.5>> = 6.667701323073103
	* braceright: B<<531.5,593.5>-<588.0,626.0>-<663.0,630.0>>/B<<663.0,630.0>-<588.0,635.0>-<531.5,667.0>> = 6.866957349082688
	* eth: B<<1084.0,868.0>-<1086.0,864.0>-<1088.0,860.0>>/B<<1088.0,860.0>-<1070.0,933.0>-<1043.0,999.0>> = 12.713632163272937
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
| 0 | 14 | 67 | 666 | 43 | 548 | 0 |
| 0% | 1% | 5% | 50% | 3% | 41% | 0% |

**Note:** The following loglevels were omitted in this report:
* **SKIP**
* **INFO**
* **PASS**
* **DEBUG**
