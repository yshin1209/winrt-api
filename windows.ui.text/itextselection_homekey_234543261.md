---
-api-id: M:Windows.UI.Text.ITextSelection.HomeKey(Windows.UI.Text.TextRangeUnit,System.Boolean)
-api-type: winrt method
---

<!-- Method syntax
public int HomeKey(Windows.UI.Text.TextRangeUnit unit, System.Boolean extend)
-->

# Windows.UI.Text.ITextSelection.HomeKey

## -description
Moves the insertion point or the active end of the text selection to the home position, mimicking the functionality of the Home key.

## -parameters
### -param unit
The units by which to move the insertion point or active end. The following values are valid.

### -param extend
Indicates how to change the selection. True extends the selection by moving only the active end. False collapses the selection to an insertion point and then moves the insertion point. The default value is false.

## -returns
The number of units that the insertion point or the active end is moved.

## -remarks
The [HomeKey](itextselection_homekey.md) method is a logical method rather than a directional method and so is dependent on the language that is involved. For example, in Arabic text, [HomeKey](itextselection_homekey.md) moves to the right end of a line, whereas in English text, it moves to the left. Thus [HomeKey](itextselection_homekey.md) is different from the [ITextSelection.MoveRight](itextselection_moveright.md) or [ITextSelection.MoveLeft](itextselection_moveleft.md) methods. [HomeKey](itextselection_homekey.md) also differs from the [ITextRange.StartOf](itextrange_startof.md) method in that it extends from the active end, whereas [StartOf](itextrange_startof.md) extends from the start position.

## -examples

## -see-also
[ITextSelection.EndKey](itextselection_endkey.md)