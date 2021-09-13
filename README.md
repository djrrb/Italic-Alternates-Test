# Italic-Alternates-Test

This test font documents a problem in Adobe apps where an alternate cannot be substituted by a feature variation (rvrn), and have that substitution undone with a stylistic set.

In this demo, the lowercase 'a' is substituted by an italic variant at .5 on the `ital` axis.

The Stylistic Sets are as follows:

* Stylistic Set 01: Substitute default `a` with italic `a`
* Stylistic Set 02: Substitute italic `a` with default `a` (should override default )
* Stylistic Set 03: Substitute default `a` with a second alternate that is  (a with no counterform)

However, when I italicize the font and then try to apply the `ss02` alternate to an individual glyph, nothing happens. It does work when the feature variation is not applied, and when I use the `ss03` alternate.

![apply-alternate-via-tooltip-sometimes-does-not-work.mov](screengrabs/apply-alternate-via-tooltip-sometimes-does-not-work.mov)

I am not able to apply stylistic sets to a selection. I would expect to see the stylistic sets listed here.

![apply-stylistic-set-via-tooltip-does-not-work.png](apply-stylistic-set-via-tooltip-does-not-work)

![apply-stylistic-set-via-character-palette-does-not-work.mov](screengrabs/apply-stylistic-set-via-character-palette-does-not-work.mov)

I would expect these Stylistic Sets to work, overriding the feature variation when applicable. This is what happens when I use the font in other apps or browsers.

![screengrabs/font-goggles.png](Font Goggles)

![screengrabs/chrome.png](Chrome)