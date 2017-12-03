# Proposal Summary Form

## Administrative Information
**Proposers name:** Sahar Afshar and José Solé

**Vendor affiliation:** N/A

**Proposal name:** Glyph Extension axis

**Date of submission:** xx December 2017

**New or revised proposal:** New

**Previous revision date:** N/A

## General Technical Information
**Overview:** [A brief description of the proposal—a detailed description is provided below.]

**Related axes:** [If this axis is intended to be used specifically in combination with certain other already-registered or proposed axes, identify the axes or proosals.]

**Similar axes:** [If this is similar to another already-registered or proposed axis — similar font behavior or function — provide the registered axis tag or proposal name.]

**Axis type:** Parametric with optical option

## Proposed Axis Details

**Tag:** gext

**Name:** Glyph Extension

**Description:** Used to vary a glyph's extension by a positive or negative value depending on parameters assigned by the layout engine (when setting lines of text) or by optical adjustment by the user (for single words or shorter lengths of text).

This axis works on a single instance of a glyph, where it will apply a change on it's extension (outline and spacing) on top of any other changes that have been previously applied via other axis.

**Valid numeric range:** Any negative, zero or positive value.

**Scale interpretation:** Starting with 0 as the glyph in it's ‘normal’ state, any increase or decrease should represent the delta of that change in per-mille-of-em of the advanced width.

**Recommended or required ‘Regular’ value:** 0

**Suggested programmatic interactions:** When used to adjust the space of a line of justified text, applications should, taking into consideration the script's rules, adjust individual glyphs extension to satisfy the desired line length.

**UI recommendations:** [Provide any recommendations regarding how this axis should be handled in application user interfaces. See the Guidance file for details on what information is and isn't
expected.]

**Script or language considerations:** This axis should be applicable to any script.

For connecting scripts such as Arabic, Syriac or Nko this could require the development and implementation of a different way of justifying text, potentially dispensing of the ‘Kashida’ or ‘Tatweel’ character. This depends on what is established as the best way for designing the glyph extension and how this affects connections.

For non-connecting scripts something similar could be needed, depending on how the axis is expected to work and the effect it should have on the text layout.

**Additional information:** Although initially thought of as a
justification axis for connecting scripts such as Arabic, Syriac or Nko, the same can be applied to any non-connecting script as way of applying small or large changes to glyphs to affect the length of a line of text.

Think of minute adjustments to contours of certain glyphs on a Gutenberg bible to help adjust the length of lines of text while maintaining the overall density of text colour on the dense columns.

## Justification

**Vendor commitments:** [none at this time]

**Conventionality benefits:** This axis and the proper layout engine implementation would provide a more flexible and familiar way of adjusting the length of a line of text by adjusting single glyphs. This is especially relevant for connecting scripts where the lack of flexibility of previous typesetting methods prevented the use of a more natural or even correct way of adjusting the space a line a of text.

For the above reasons plus the additional functionality this would provide to non-connecting scripts, we think this would be a welcome addition to the OpenType specification by both users and the industry, and it would have a noticeable positive impact on the quality of the typesetting when compared to the current status quo.

**Interoperability benefits:** Having a properly defined axis for single-glyph adjustment and the additional definition of more advanced justification methods would allow users to know what to expect when setting type on different environments and applications. This would also help standardise how fonts that contain such an axis would need to be developed and implemented, ensuring consistency and interoperability.
