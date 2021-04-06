## Fontbakery report

Fontbakery version: 0.7.34

<details>
<summary><b>[7] BonaNova-Bold.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Are there caret positions declared for every ligature?</summary>

* [com.google.fonts/check/ligature_carets](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/ligature_carets)
<pre>--- Rationale ---

All ligatures in a font must have corresponding caret (text cursor) positions
defined in the GDEF table, otherwhise, users may experience issues with caret
rendering.

If using GlyphsApp, ligature carets can be set directly on canvas by accessing
the `Glyph -&gt; Set Anchors` menu option or by pressing the `Cmd+U` keyboard
shortcut.

If designing with UFOs, (as of Oct 2020) ligature carets are not yet compiled
by ufo2ft, and therefore will not build via FontMake. See
googlefonts/ufo2ft/issues/329


</pre>

* 🔥 **FAIL** Failed to lookup ligatures. This font file seems to be malformed. For more info, read: https://github.com/googlefonts/fontbakery/issues/1596 [code: malformed]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---

Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).


</pre>

* 🔥 **FAIL** Failed to lookup ligatures. This font file seems to be malformed. For more info, read: https://github.com/googlefonts/fontbakery/issues/1596 [code: malformed]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---

Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is
stored in the achVendID field of the OS/2 table.

Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:

https://docs.microsoft.com/en-us/typography/vendors/

This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.

Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.


</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---

Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will
only differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.

However, a quotedbl should have 2 contours, unless the font belongs to a
display family.

This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.


</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: registered	Contours detected: 2	Expected: 3 or 4
Glyph name: Eth	Contours detected: 3	Expected: 2
Glyph name: Dcroat	Contours detected: 3	Expected: 2
Glyph name: dcroat	Contours detected: 3	Expected: 2
Glyph name: hbar	Contours detected: 2	Expected: 1
Glyph name: oe	Contours detected: 4	Expected: 3
Glyph name: Racute	Contours detected: 2	Expected: 3
Glyph name: uni0156	Contours detected: 2	Expected: 3
Glyph name: Rcaron	Contours detected: 2	Expected: 3
Glyph name: Uogonek	Contours detected: 2	Expected: 1
Glyph name: uni0180	Contours detected: 3	Expected: 2
Glyph name: ohorn	Contours detected: 3	Expected: 2
Glyph name: uni01EA	Contours detected: 3	Expected: 2
Glyph name: uni01EB	Contours detected: 3	Expected: 2
Glyph name: uni0210	Contours detected: 3	Expected: 4
Glyph name: uni0212	Contours detected: 2	Expected: 3
Glyph name: uni0228	Contours detected: 2	Expected: 1
Glyph name: uni0229	Contours detected: 3	Expected: 2
Glyph name: uni042F	Contours detected: 1	Expected: 2
Glyph name: uni044F	Contours detected: 1	Expected: 2
Glyph name: uni045B	Contours detected: 2	Expected: 1
Glyph name: uni1E08	Contours detected: 3	Expected: 2
Glyph name: uni1E09	Contours detected: 3	Expected: 2
Glyph name: uni1E1C	Contours detected: 3	Expected: 2
Glyph name: uni1E1D	Contours detected: 4	Expected: 3
Glyph name: uni1E5A	Contours detected: 2	Expected: 3
Glyph name: uni1E5E	Contours detected: 2	Expected: 3
Glyph name: uni1EDB	Contours detected: 4	Expected: 3
Glyph name: uni1EDD	Contours detected: 4	Expected: 3
Glyph name: uni1EDF	Contours detected: 4	Expected: 3
Glyph name: uni1EE1	Contours detected: 4	Expected: 3
Glyph name: uni1EE3	Contours detected: 4	Expected: 3
Glyph name: uni2076	Contours detected: 1	Expected: 2
Glyph name: uni2079	Contours detected: 1	Expected: 2
Glyph name: uni2086	Contours detected: 1	Expected: 2
Glyph name: uni2089	Contours detected: 1	Expected: 2
Glyph name: uni20B1	Contours detected: 3	Expected: 1, 2 or 4
Glyph name: uni2159	Contours detected: 3	Expected: 4
Glyph name: uni215A	Contours detected: 3	Expected: 4
Glyph name: Dcroat	Contours detected: 3	Expected: 2
Glyph name: Eth	Contours detected: 3	Expected: 2
Glyph name: Racute	Contours detected: 2	Expected: 3
Glyph name: Rcaron	Contours detected: 2	Expected: 3
Glyph name: Uogonek	Contours detected: 2	Expected: 1
Glyph name: dcroat	Contours detected: 3	Expected: 2
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2
Glyph name: hbar	Contours detected: 2	Expected: 1
Glyph name: oe	Contours detected: 4	Expected: 3
Glyph name: ohorn	Contours detected: 3	Expected: 2
Glyph name: registered	Contours detected: 2	Expected: 3 or 4
Glyph name: uni0156	Contours detected: 2	Expected: 3
Glyph name: uni0180	Contours detected: 3	Expected: 2
Glyph name: uni0228	Contours detected: 2	Expected: 1
Glyph name: uni0229	Contours detected: 3	Expected: 2
Glyph name: uni042F	Contours detected: 1	Expected: 2
Glyph name: uni044F	Contours detected: 1	Expected: 2
Glyph name: uni045B	Contours detected: 2	Expected: 1
Glyph name: uni1E08	Contours detected: 3	Expected: 2
Glyph name: uni1E09	Contours detected: 3	Expected: 2
Glyph name: uni1E1C	Contours detected: 3	Expected: 2
Glyph name: uni1E1D	Contours detected: 4	Expected: 3
Glyph name: uni1E5A	Contours detected: 2	Expected: 3
Glyph name: uni1E5E	Contours detected: 2	Expected: 3
Glyph name: uni1EDB	Contours detected: 4	Expected: 3
Glyph name: uni1EDD	Contours detected: 4	Expected: 3
Glyph name: uni1EDF	Contours detected: 4	Expected: 3
Glyph name: uni1EE1	Contours detected: 4	Expected: 3
Glyph name: uni1EE3	Contours detected: 4	Expected: 3
Glyph name: uni20B1	Contours detected: 3	Expected: 1, 2 or 4 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---

This test looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.

This test is not run for variable fonts, as they may legitimately have colinear
vectors.


</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* eta: L<<260.0,349.0>--<260.0,345.0>> -> L<<260.0,345.0>--<260.0,0.0>>
	* etatonos: L<<260.0,349.0>--<260.0,345.0>> -> L<<260.0,345.0>--<260.0,0.0>>
	* uni00B5: L<<333.0,110.0>--<333.0,115.0>> -> L<<333.0,115.0>--<333.0,460.0>>
	* uni00B5: L<<45.0,-240.0>--<48.0,109.0>> -> L<<48.0,109.0>--<48.0,460.0>>
	* uni03BC: L<<333.0,110.0>--<333.0,115.0>> -> L<<333.0,115.0>--<333.0,460.0>>
	* uni03BC: L<<45.0,-240.0>--<48.0,109.0>> -> L<<48.0,109.0>--<48.0,460.0>>
	* uniFEBA: L<<1113.0,140.0>--<1140.0,142.0>> -> L<<1140.0,142.0>--<1207.0,142.0>>
	* uniFEBC: L<<746.0,140.0>--<776.0,142.0>> -> L<<776.0,142.0>--<830.0,142.0>>
	* uniFEBE: L<<1113.0,140.0>--<1140.0,142.0>> -> L<<1140.0,142.0>--<1207.0,142.0>> and uniFEC0: L<<746.0,140.0>--<776.0,142.0>> -> L<<776.0,142.0>--<830.0,142.0>> [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---

This test heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed
up by manual inspection.


</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* A_H: B<<217.0,197.0>-<214.0,191.0>-<209.0,183.0>>/L<<209.0,183.0>--<217.0,197.0>> = 2.260501911141034
	* A_H: L<<209.0,183.0>--<217.0,197.0>>/B<<217.0,197.0>-<214.0,191.0>-<209.0,183.0>> = 3.1798301198640497
	* sigma: B<<453.5,347.5>-<428.0,355.0>-<402.0,364.0>>/B<<402.0,364.0>-<433.0,347.0>-<461.0,321.5>> = 9.646303291202416
	* uni0452: L<<233.0,343.0>--<232.0,355.0>>/L<<232.0,355.0>--<232.0,110.0>> = 4.763641690726144
	* uni05D0: B<<496.5,260.5>-<492.0,244.0>-<509.0,229.0>>/L<<509.0,229.0>--<494.0,242.0>> = 0.5092824049768564
	* uni05D0: L<<509.0,229.0>--<494.0,242.0>>/L<<494.0,242.0>--<609.0,138.0>> = 1.2101630959891547
	* uniFB2E: B<<496.5,260.5>-<492.0,244.0>-<509.0,229.0>>/L<<509.0,229.0>--<494.0,242.0>> = 0.5092824049768564
	* uniFB2E: L<<509.0,229.0>--<494.0,242.0>>/L<<494.0,242.0>--<609.0,138.0>> = 1.2101630959891547
	* uniFB2F: B<<496.5,260.5>-<492.0,244.0>-<509.0,229.0>>/L<<509.0,229.0>--<494.0,242.0>> = 0.5092824049768564
	* uniFB2F: L<<509.0,229.0>--<494.0,242.0>>/L<<494.0,242.0>--<609.0,138.0>> = 1.2101630959891547 and 4 more. [code: found-jaggy-segments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---

This test detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.

This test is disabled for italic styles, which often contain nearly-upright
lines.


</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
	* arrowupdn: L<<207.0,153.0>--<208.0,512.0>>
	* braceleftbt: L<<93.0,791.0>--<228.0,790.0>>
	* bracelefttp: L<<228.0,-221.0>--<93.0,-222.0>>
	* bracerightbt: L<<93.0,789.0>--<228.0,790.0>>
	* bracerighttp: L<<228.0,-225.0>--<93.0,-224.0>>
	* eng.sc: L<<514.0,217.0>--<515.0,425.0>>
	* estimated: L<<603.0,398.0>--<602.0,551.0>>
	* four.lf: L<<481.0,665.0>--<480.0,255.0>>
	* four.osf: L<<457.0,493.0>--<456.0,120.0>>
	* four.sc: L<<419.0,532.0>--<418.0,204.0>> and 15 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[6] BonaNova-Italic.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Are there caret positions declared for every ligature?</summary>

* [com.google.fonts/check/ligature_carets](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/ligature_carets)
<pre>--- Rationale ---

All ligatures in a font must have corresponding caret (text cursor) positions
defined in the GDEF table, otherwhise, users may experience issues with caret
rendering.

If using GlyphsApp, ligature carets can be set directly on canvas by accessing
the `Glyph -&gt; Set Anchors` menu option or by pressing the `Cmd+U` keyboard
shortcut.

If designing with UFOs, (as of Oct 2020) ligature carets are not yet compiled
by ufo2ft, and therefore will not build via FontMake. See
googlefonts/ufo2ft/issues/329


</pre>

* 🔥 **FAIL** Failed to lookup ligatures. This font file seems to be malformed. For more info, read: https://github.com/googlefonts/fontbakery/issues/1596 [code: malformed]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---

Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is
stored in the achVendID field of the OS/2 table.

Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:

https://docs.microsoft.com/en-us/typography/vendors/

This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.

Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.


</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---

Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will
only differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.

However, a quotedbl should have 2 contours, unless the font belongs to a
display family.

This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.


</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: Eth	Contours detected: 3	Expected: 2
Glyph name: Dcroat	Contours detected: 3	Expected: 2
Glyph name: dcroat	Contours detected: 3	Expected: 2
Glyph name: hbar	Contours detected: 2	Expected: 1
Glyph name: oe	Contours detected: 4	Expected: 3
Glyph name: Racute	Contours detected: 2	Expected: 3
Glyph name: uni0156	Contours detected: 2	Expected: 3
Glyph name: Rcaron	Contours detected: 2	Expected: 3
Glyph name: Tbar	Contours detected: 2	Expected: 1
Glyph name: Uogonek	Contours detected: 2	Expected: 1
Glyph name: uni0180	Contours detected: 3	Expected: 2
Glyph name: uni0199	Contours detected: 2	Expected: 1
Glyph name: ohorn	Contours detected: 3	Expected: 2
Glyph name: uni01C2	Contours detected: 3	Expected: 1
Glyph name: uni01EA	Contours detected: 3	Expected: 2
Glyph name: uni01EB	Contours detected: 3	Expected: 2
Glyph name: uni0210	Contours detected: 3	Expected: 4
Glyph name: uni0212	Contours detected: 2	Expected: 3
Glyph name: uni0228	Contours detected: 2	Expected: 1
Glyph name: uni0229	Contours detected: 3	Expected: 2
Glyph name: uni042F	Contours detected: 1	Expected: 2
Glyph name: uni044F	Contours detected: 1	Expected: 2
Glyph name: uni1E08	Contours detected: 3	Expected: 2
Glyph name: uni1E09	Contours detected: 3	Expected: 2
Glyph name: uni1E1C	Contours detected: 3	Expected: 2
Glyph name: uni1E1D	Contours detected: 4	Expected: 3
Glyph name: uni1E5A	Contours detected: 2	Expected: 3
Glyph name: uni1E5E	Contours detected: 2	Expected: 3
Glyph name: uni1EDB	Contours detected: 4	Expected: 3
Glyph name: uni1EDD	Contours detected: 4	Expected: 3
Glyph name: uni1EDF	Contours detected: 4	Expected: 3
Glyph name: uni1EE1	Contours detected: 4	Expected: 3
Glyph name: uni1EE3	Contours detected: 4	Expected: 3
Glyph name: uni2076	Contours detected: 1	Expected: 2
Glyph name: uni2079	Contours detected: 1	Expected: 2
Glyph name: uni2086	Contours detected: 1	Expected: 2
Glyph name: uni2089	Contours detected: 1	Expected: 2
Glyph name: uni20B1	Contours detected: 3	Expected: 1, 2 or 4
Glyph name: uni2159	Contours detected: 3	Expected: 4
Glyph name: uni215A	Contours detected: 3	Expected: 4
Glyph name: Dcroat	Contours detected: 3	Expected: 2
Glyph name: Eth	Contours detected: 3	Expected: 2
Glyph name: Racute	Contours detected: 2	Expected: 3
Glyph name: Rcaron	Contours detected: 2	Expected: 3
Glyph name: Tbar	Contours detected: 2	Expected: 1
Glyph name: Uogonek	Contours detected: 2	Expected: 1
Glyph name: dcroat	Contours detected: 3	Expected: 2
Glyph name: fi	Contours detected: 2	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2
Glyph name: hbar	Contours detected: 2	Expected: 1
Glyph name: oe	Contours detected: 4	Expected: 3
Glyph name: ohorn	Contours detected: 3	Expected: 2
Glyph name: uni0156	Contours detected: 2	Expected: 3
Glyph name: uni0180	Contours detected: 3	Expected: 2
Glyph name: uni0199	Contours detected: 2	Expected: 1
Glyph name: uni01C2	Contours detected: 3	Expected: 1
Glyph name: uni0228	Contours detected: 2	Expected: 1
Glyph name: uni0229	Contours detected: 3	Expected: 2
Glyph name: uni042F	Contours detected: 1	Expected: 2
Glyph name: uni044F	Contours detected: 1	Expected: 2
Glyph name: uni1E08	Contours detected: 3	Expected: 2
Glyph name: uni1E09	Contours detected: 3	Expected: 2
Glyph name: uni1E1C	Contours detected: 3	Expected: 2
Glyph name: uni1E1D	Contours detected: 4	Expected: 3
Glyph name: uni1E5A	Contours detected: 2	Expected: 3
Glyph name: uni1E5E	Contours detected: 2	Expected: 3
Glyph name: uni1EDB	Contours detected: 4	Expected: 3
Glyph name: uni1EDD	Contours detected: 4	Expected: 3
Glyph name: uni1EDF	Contours detected: 4	Expected: 3
Glyph name: uni1EE1	Contours detected: 4	Expected: 3
Glyph name: uni1EE3	Contours detected: 4	Expected: 3
Glyph name: uni20B1	Contours detected: 3	Expected: 1, 2 or 4 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Does GPOS table have kerning information? This check skips monospaced fonts as defined by post.isFixedPitch value</summary>

* [com.google.fonts/check/gpos_kerning_info](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/gpos.html#com.google.fonts/check/gpos_kerning_info)

* ⚠ **WARN** GPOS table lacks kerning information. [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---

This test looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.

This test is not run for variable fonts, as they may legitimately have colinear
vectors.


</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* G.swsh: L<<626.0,248.0>--<622.0,190.0>> -> L<<622.0,190.0>--<608.0,-15.0>>
	* Gbreve.swsh: L<<626.0,248.0>--<622.0,190.0>> -> L<<622.0,190.0>--<608.0,-15.0>>
	* Gdotaccent.swsh: L<<626.0,248.0>--<622.0,190.0>> -> L<<622.0,190.0>--<608.0,-15.0>>
	* uni0122.swsh: L<<626.0,248.0>--<622.0,190.0>> -> L<<622.0,190.0>--<608.0,-15.0>>
	* uni0233.sc: L<<156.0,275.0>--<115.0,360.0>> -> L<<115.0,360.0>--<84.0,425.0>>
	* uni0233.sc: L<<157.0,425.0>--<196.0,348.0>> -> L<<196.0,348.0>--<225.0,290.0>>
	* uni0233.sc: L<<227.0,290.0>--<260.0,339.0>> -> L<<260.0,339.0>--<317.0,425.0>>
	* uni0233.sc: L<<363.0,425.0>--<300.0,333.0>> -> L<<300.0,333.0>--<261.0,275.0>>
	* uni042A: L<<190.0,100.0>--<222.0,566.0>> -> L<<222.0,566.0>--<227.0,635.0>>
	* uni05D2: L<<136.0,537.0>--<147.0,534.0>> -> L<<147.0,534.0>--<258.0,507.0>> and 57 more. [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---

This test heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed
up by manual inspection.


</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* shaddaAlefabovear: L<<-45.0,640.0>--<-45.0,640.0>>/L<<-45.0,640.0>--<-53.0,639.0>> = 7.125016348901757
	* shaddaDammaar: L<<-45.0,640.0>--<-45.0,640.0>>/L<<-45.0,640.0>--<-53.0,639.0>> = 7.125016348901757
	* shaddaDammatanar: L<<-45.0,640.0>--<-45.0,640.0>>/L<<-45.0,640.0>--<-53.0,639.0>> = 7.125016348901757
	* shaddaFathaar: L<<-45.0,639.0>--<-45.0,639.0>>/L<<-45.0,639.0>--<-53.0,638.0>> = 7.125016348901757
	* shaddaFathatanar: L<<-45.0,639.0>--<-45.0,639.0>>/L<<-45.0,639.0>--<-53.0,638.0>> = 7.125016348901757
	* shaddaKasraar: L<<-5.0,789.0>--<-5.0,789.0>>/L<<-5.0,789.0>--<-13.0,788.0>> = 7.125016348901757
	* shaddaKasratanar: L<<35.0,919.0>--<35.0,919.0>>/L<<35.0,919.0>--<27.0,918.0>> = 7.125016348901757
	* uni0446.loclBGR: B<<406.0,7.5>-<418.0,31.0>-<434.0,51.0>>/B<<434.0,51.0>-<383.0,7.0>-<336.0,-15.0>> = 10.554370268643943
	* uni0446: B<<406.0,7.5>-<418.0,31.0>-<434.0,51.0>>/B<<434.0,51.0>-<383.0,7.0>-<336.0,-15.0>> = 10.554370268643943
	* uni0449.loclBGR: B<<638.0,7.5>-<650.0,31.0>-<666.0,51.0>>/B<<666.0,51.0>-<615.0,7.0>-<568.0,-15.0>> = 10.554370268643943 and 9 more. [code: found-jaggy-segments]

</details>
<br>
</details>
<details>
<summary><b>[7] BonaNova-Regular.ttf</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Are there caret positions declared for every ligature?</summary>

* [com.google.fonts/check/ligature_carets](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/ligature_carets)
<pre>--- Rationale ---

All ligatures in a font must have corresponding caret (text cursor) positions
defined in the GDEF table, otherwhise, users may experience issues with caret
rendering.

If using GlyphsApp, ligature carets can be set directly on canvas by accessing
the `Glyph -&gt; Set Anchors` menu option or by pressing the `Cmd+U` keyboard
shortcut.

If designing with UFOs, (as of Oct 2020) ligature carets are not yet compiled
by ufo2ft, and therefore will not build via FontMake. See
googlefonts/ufo2ft/issues/329


</pre>

* 🔥 **FAIL** Failed to lookup ligatures. This font file seems to be malformed. For more info, read: https://github.com/googlefonts/fontbakery/issues/1596 [code: malformed]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---

Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).


</pre>

* 🔥 **FAIL** Failed to lookup ligatures. This font file seems to be malformed. For more info, read: https://github.com/googlefonts/fontbakery/issues/1596 [code: malformed]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---

Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is
stored in the achVendID field of the OS/2 table.

Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:

https://docs.microsoft.com/en-us/typography/vendors/

This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.

Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.


</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---

Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will
only differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.

However, a quotedbl should have 2 contours, unless the font belongs to a
display family.

This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.


</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: Eth	Contours detected: 3	Expected: 2
Glyph name: Dcroat	Contours detected: 3	Expected: 2
Glyph name: dcroat	Contours detected: 3	Expected: 2
Glyph name: hbar	Contours detected: 2	Expected: 1
Glyph name: oe	Contours detected: 4	Expected: 3
Glyph name: Racute	Contours detected: 2	Expected: 3
Glyph name: uni0156	Contours detected: 2	Expected: 3
Glyph name: Rcaron	Contours detected: 2	Expected: 3
Glyph name: Uogonek	Contours detected: 2	Expected: 1
Glyph name: uni0180	Contours detected: 3	Expected: 2
Glyph name: ohorn	Contours detected: 3	Expected: 2
Glyph name: uni01EA	Contours detected: 3	Expected: 2
Glyph name: uni01EB	Contours detected: 3	Expected: 2
Glyph name: uni0210	Contours detected: 3	Expected: 4
Glyph name: uni0212	Contours detected: 2	Expected: 3
Glyph name: uni0228	Contours detected: 2	Expected: 1
Glyph name: uni0229	Contours detected: 3	Expected: 2
Glyph name: uni042F	Contours detected: 1	Expected: 2
Glyph name: uni044F	Contours detected: 1	Expected: 2
Glyph name: uni045B	Contours detected: 2	Expected: 1
Glyph name: uni1E08	Contours detected: 3	Expected: 2
Glyph name: uni1E09	Contours detected: 3	Expected: 2
Glyph name: uni1E1C	Contours detected: 3	Expected: 2
Glyph name: uni1E1D	Contours detected: 4	Expected: 3
Glyph name: uni1E5A	Contours detected: 2	Expected: 3
Glyph name: uni1E5E	Contours detected: 2	Expected: 3
Glyph name: uni1EDB	Contours detected: 4	Expected: 3
Glyph name: uni1EDD	Contours detected: 4	Expected: 3
Glyph name: uni1EDF	Contours detected: 4	Expected: 3
Glyph name: uni1EE1	Contours detected: 4	Expected: 3
Glyph name: uni1EE3	Contours detected: 4	Expected: 3
Glyph name: uni2076	Contours detected: 1	Expected: 2
Glyph name: uni2079	Contours detected: 1	Expected: 2
Glyph name: uni2086	Contours detected: 1	Expected: 2
Glyph name: uni2089	Contours detected: 1	Expected: 2
Glyph name: uni20B1	Contours detected: 3	Expected: 1, 2 or 4
Glyph name: uni2159	Contours detected: 3	Expected: 4
Glyph name: uni215A	Contours detected: 3	Expected: 4
Glyph name: Dcroat	Contours detected: 3	Expected: 2
Glyph name: Eth	Contours detected: 3	Expected: 2
Glyph name: Racute	Contours detected: 2	Expected: 3
Glyph name: Rcaron	Contours detected: 2	Expected: 3
Glyph name: Uogonek	Contours detected: 2	Expected: 1
Glyph name: dcroat	Contours detected: 3	Expected: 2
Glyph name: fi	Contours detected: 1	Expected: 3
Glyph name: fl	Contours detected: 1	Expected: 2
Glyph name: hbar	Contours detected: 2	Expected: 1
Glyph name: oe	Contours detected: 4	Expected: 3
Glyph name: ohorn	Contours detected: 3	Expected: 2
Glyph name: uni0156	Contours detected: 2	Expected: 3
Glyph name: uni0180	Contours detected: 3	Expected: 2
Glyph name: uni0228	Contours detected: 2	Expected: 1
Glyph name: uni0229	Contours detected: 3	Expected: 2
Glyph name: uni042F	Contours detected: 1	Expected: 2
Glyph name: uni044F	Contours detected: 1	Expected: 2
Glyph name: uni045B	Contours detected: 2	Expected: 1
Glyph name: uni1E08	Contours detected: 3	Expected: 2
Glyph name: uni1E09	Contours detected: 3	Expected: 2
Glyph name: uni1E1C	Contours detected: 3	Expected: 2
Glyph name: uni1E1D	Contours detected: 4	Expected: 3
Glyph name: uni1E5A	Contours detected: 2	Expected: 3
Glyph name: uni1E5E	Contours detected: 2	Expected: 3
Glyph name: uni1EDB	Contours detected: 4	Expected: 3
Glyph name: uni1EDD	Contours detected: 4	Expected: 3
Glyph name: uni1EDF	Contours detected: 4	Expected: 3
Glyph name: uni1EE1	Contours detected: 4	Expected: 3
Glyph name: uni1EE3	Contours detected: 4	Expected: 3
Glyph name: uni20B1	Contours detected: 3	Expected: 1, 2 or 4 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---

This test looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.

This test is not run for variable fonts, as they may legitimately have colinear
vectors.


</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* A_H: L<<236.0,253.0>--<236.0,253.0>> -> L<<236.0,253.0>--<236.0,253.0>>
	* uni00B5: L<<70.0,-240.0>--<73.0,109.0>> -> L<<73.0,109.0>--<74.0,440.0>>
	* uni02A9: L<<499.0,335.0>--<499.0,331.0>> -> L<<499.0,331.0>--<499.0,101.0>>
	* uni03BC: L<<70.0,-240.0>--<73.0,109.0>> -> L<<73.0,109.0>--<74.0,440.0>>
	* uniFEBA: L<<1073.0,90.0>--<1115.0,92.0>> -> L<<1115.0,92.0>--<1195.0,92.0>>
	* uniFEBC: L<<704.0,90.0>--<740.0,92.0>> -> L<<740.0,92.0>--<820.0,92.0>>
	* uniFEBE: L<<1073.0,90.0>--<1115.0,92.0>> -> L<<1115.0,92.0>--<1195.0,92.0>> and uniFEC0: L<<704.0,90.0>--<740.0,92.0>> -> L<<740.0,92.0>--<820.0,92.0>> [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---

This test heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed
up by manual inspection.


</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* A_H: L<<236.0,253.0>--<220.0,225.0>>/L<<220.0,225.0>--<221.0,228.0>> = 11.309932474020162
	* u1F679: B<<213.5,456.5>-<216.0,392.0>-<204.0,307.0>>/B<<204.0,307.0>-<218.0,344.0>-<235.5,370.5>> = 12.689848155025715
	* uni0448.loclBGR: B<<407.5,11.0>-<383.0,37.0>-<379.0,80.0>>/L<<379.0,80.0>--<379.0,77.0>> = 5.3145456699447315
	* uni0449.loclBGR: B<<407.5,11.0>-<383.0,37.0>-<379.0,80.0>>/L<<379.0,80.0>--<379.0,77.0>> = 5.3145456699447315
	* uni05D0: L<<173.0,501.0>--<454.0,227.0>>/L<<454.0,227.0>--<425.0,255.0>> = 0.2824748494706725
	* uni062C: L<<566.0,411.0>--<566.0,411.0>>/B<<566.0,411.0>-<500.0,410.0>-<435.0,388.5>> = 0.8680514497453689
	* uni062D: L<<566.0,411.0>--<566.0,411.0>>/B<<566.0,411.0>-<500.0,410.0>-<435.0,388.5>> = 0.8680514497453689
	* uni062E: L<<566.0,411.0>--<566.0,411.0>>/B<<566.0,411.0>-<500.0,410.0>-<435.0,388.5>> = 0.8680514497453689
	* uniFB2E: L<<173.0,501.0>--<454.0,227.0>>/L<<454.0,227.0>--<425.0,255.0>> = 0.2824748494706725
	* uniFB2F: L<<173.0,501.0>--<454.0,227.0>>/L<<454.0,227.0>--<425.0,255.0>> = 0.2824748494706725 and 5 more. [code: found-jaggy-segments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---

This test detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.

This test is disabled for italic styles, which often contain nearly-upright
lines.


</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
	* arrowdown: L<<212.0,100.0>--<214.0,660.0>>
	* arrowdown: L<<244.0,660.0>--<245.0,99.0>>
	* arrowupdn: L<<214.0,106.0>--<212.0,559.0>>
	* arrowupdn: L<<246.0,559.0>--<245.0,104.0>>
	* estimated: L<<605.0,398.0>--<604.0,551.0>>
	* f_f_u: L<<731.0,100.0>--<732.0,356.0>>
	* f_t_u: L<<738.0,100.0>--<739.0,356.0>>
	* f_u: L<<418.0,100.0>--<419.0,356.0>>
	* four.dnom: L<<238.0,363.0>--<237.0,130.0>>
	* four.lf: L<<414.0,665.0>--<413.0,226.0>> and 50 more. [code: found-semi-vertical]

</details>
<br>
</details>

### Summary

| 💔 ERROR | 🔥 FAIL | ⚠ WARN | 💤 SKIP | ℹ INFO | 🍞 PASS | 🔎 DEBUG |
|:-----:|:----:|:----:|:----:|:----:|:----:|:----:|
| 0 | 5 | 15 | 270 | 22 | 243 | 0 |
| 0% | 1% | 3% | 49% | 4% | 44% | 0% |

**Note:** The following loglevels were omitted in this report:
* **SKIP**
* **INFO**
* **PASS**
* **DEBUG**
