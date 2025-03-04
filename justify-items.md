# justify-items

The CSS justify-items property defines the default justify-self for all items of the box, giving them all a default way of justifying each box along the appropriate axis.

## Values

<dl>
<dt>auto</dt>
<dd>The value used is the value of the justify-items property of the parents box, unless the box has no parent, or is absolutely positioned, in these cases, auto represents normal.</dd>
<dt>normal</dt>
<dd>The effect of this keyword is dependent of the layout mode we are in:

-   In block-level layouts, the keyword is a synonym of start.
-   In absolutely-positioned layouts, the keyword behaved like start on replaced absolutely-positioned boxes, and as stretch on all other absolutely-positioned boxes.
-   In table cell layouts, this keyword has no meaning as this property is ignored.
-   In flexbox layouts, this keyword has no meaning as this property is ignored.
-   In grid layouts, this keyword leads to a behavior similar to the one of stretch, except for boxes with an aspect ratio or an intrinsic sizes where it behaves like start.</dd>
<dt>start</dt>
<dd>The item is packed flush to each other toward the start edge of the alignment container in the appropriate axis.</dd>
<dt>end</dt>
<dd>The item is packed flush to each other toward the end edge of the alignment container in the appropriate axis.</dd>
<dt>flex-start</dt>
<dd>For items that are not children of a flex container, this value is treated like start.</dd>
<dt>flex-end</dt>
<dd>For items that are not children of a flex container, this value is treated like end.</dd>
<dt>self-start</dt>
<dd>The item is packed flush to the edge of the alignment container of the start side of the item, in the appropriate axis.</dd>
<dt>self-end</dt>
<dd>The item is packed flush to the edge of the alignment container of the end side of the item, in the appropriate axis.</dd>
<dt>center</dt>
<dd>The items are packed flush to each other toward the center of the of the alignment container.</dd>
<dt>left</dt>
<dd>The items are packed flush to each other toward the left edge of the alignment container. If the property’s axis is not parallel with the inline axis, this value behaves like
start.</dd>
<dt>right</dt>
<dd>The items are packed flush to each other toward the right edge of the alignment container in the appropriate axis. If the property’s axis is not parallel with the inline axis, this value behaves like start.</dd>
<dt>baseline, first baseline, last baseline</dt>
<dd>Specifies participation in first- or last-baseline alignment: aligns the alignment baseline of the box’s first or last baseline set with the corresponding baseline in the shared first or last baseline set of all the boxes in its baseline-sharing group.
The fallback alignment for first baseline is start, the one for last baseline is end.</dd>
<dt>stretch</dt>
<dd>If the combined size of the items is less than the size of the alignment container, any auto-sized items have their size increased equally (not proportionally), while still respecting the constraints imposed by max-height/max-width (or equivalent functionality), so that the combined size exactly fills the alignment container.</dd>
<dt>safe</dt>
<dd>If the size of the item overflows the alignment container, the item is instead aligned as if the alignment mode were start.</dd>
<dt>unsafe</dt>
<dd>Regardless of the relative sizes of the item and alignment container, the given alignment value is honored.</dd>
<dt>legacy</dt>
<dd>Makes the value inherited by the box descendants. Note that if a descendant has a justify-self: auto value, the legacy keyword is not considered by the descend, only the left, right, or center value associated to it.</dd>
</dl>

## Examples

```
justify-items="center"     /* Pack items around the center */
justify-items="start"      /* Pack items from the start */
justify-items="end"        /* Pack items from the end */
justify-items="flex-start" /* Equivalent to 'start'. Note that justify-items is ignored in Flexbox layouts. */
```
