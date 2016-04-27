<properties
    pageTitle="Radio control: reference | Microsoft PowerApps"
    description="Information, including properties and examples, about the Radio control"
    services=""
    suite="powerapps"
    documentationCenter="na"
    authors="aftowen"
    manager="erikre"
    editor=""
    tags=""/>

<tags
   ms.service="powerapps"
   ms.devlang="na"
   ms.topic="article"
   ms.tgt_pltfrm="na"
   ms.workload="na"
   ms.date="03/09/2016"
   ms.author="anneta"/>

# Radio control in PowerApps #
[AZURE.INCLUDE [control-summary-radio](../../includes/control-summary-radio.md)]

## Description ##
A **Radio** control, with which users have decades of experience, is best used with only a few options that are mutually exclusive.

## Key properties ##

[**Default**](properties\properties-core.md) – The initial value of a control before it is changed by the user.

[**Items**](properties\properties-core.md) – The source of data that appears in a control such as a gallery, a list, or a chart.

[AZURE.INCLUDE [long-items](../../includes/long-items.md)]

[**Value**](properties\properties-core.md) – The value of an input control.

## All properties ##
[**Align**](properties\properties-text.md) – The location of text in relation to the horizontal center of its control.

[**BorderColor**](properties\properties-color-border.md) – The color of a control's border.

[**BorderStyle**](properties\properties-color-border.md) – Whether a control's border is **Solid**, **Dashed**, **Dotted**, or **None**.

[**BorderThickness**](properties\properties-color-border.md) – The thickness of a control's border.

[**Color**](properties\properties-color-border.md) – The color of text in a control.

[**Disabled**](properties\properties-core.md) – Whether the user can interact with the control.

[**DisabledBorderColor**](properties\properties-color-border.md) – The color of a control's border if the control's **Disabled** property is set to **true**.

[**DisabledColor**](properties\properties-color-border.md) – The color of text in a control if its **Disabled** property is set to **true**.

[**DisabledFill**](properties\properties-color-border.md) – The background color of a control if its **Disabled** property is set to **true**.

[**Fill**](properties\properties-color-border.md) – The background color of a control.

[**Font**](properties\properties-text.md) – The name of the family of fonts in which text appears.

[**FontWeight**](properties\properties-text.md) – The weight of the text in a control: **Bold**, **Semibold**, **Normal**, or **Lighter**.

[**Height**](properties\properties-size-location.md) – The distance between a control's top and bottom edges.

[**HoverColor**](properties\properties-color-border.md) – The color of the text in a control when the user keeps the mouse pointer on it.

[**HoverFill**](properties\properties-color-border.md) – The background color of a control when the user keeps the mouse pointer on it.

[**Italic**](properties\properties-text.md) – Whether the text in a control is italic.

[**LineHeight**](properties\properties-text.md) – The distance between, for example, lines of text or items in a list.

[**OnChange**](properties\properties-core.md) – How the app responds when the user changes the value of a control (for example, by adjusting a slider).

[**OnSelect**](properties\properties-core.md) – How the app responds when the user taps or clicks a control.

[**PaddingBottom**](properties\properties-size-location.md) – The distance between text in a control and the bottom edge of that control.

[**PaddingLeft**](properties\properties-size-location.md) – The distance between text in a control and the left edge of that control.

[**PaddingRight**](properties\properties-size-location.md) – The distance between text in a control and the right edge of that control.

[**PaddingTop**](properties\properties-size-location.md) – The distance between text in a control and the top edge of that control.

[**PressedColor**](properties\properties-color-border.md) – The color of text in a control when the user taps or clicks that control.

[**PressedFill**](properties\properties-color-border.md) – The background color of a control when the user taps or clicks that control.

**RadioBackgroundFill** – The background color of the circles in a radio-button control.

**RadioBorderColor** – The color of the circle for each option in a radio-button control.

**RadioSelectionFill** – The color that appears inside the circle of the selected option in a radio-button control.

**RadioSize** – The diameter of the circles in a radio-button control.

[**Reset**](properties\properties-core.md) – Whether a control reverts to its default value.

[**Size**](properties\properties-text.md) – The font size of the text that appears on a control.

[**Strikethrough**](properties\properties-text.md) – Whether a line appears through the text that appears on a control.

[**Tooltip**](properties\properties-core.md) – Explanatory text that appears when the user hovers over a control.

[**Underline**](properties\properties-text.md) – Whether a line appears under the text that appears on a control.

[**Visible**](properties\properties-core.md) – Whether a control appears or is hidden.

[**Width**](properties\properties-size-location.md) – The distance between a control's left and right edges.

[**X**](properties\properties-size-location.md) – The distance between the left edge of a control and the left edge of the screen.

[**Y**](properties\properties-size-location.md) – The distance between the top edge of a control and the top edge of the screen.

## Related functions ##

[**Distinct**( *DataSource*, *ColumnName* )](function-distinct.md)

## Example ##
1. Add a **Radio** control, name it **Pricing**, and set its **Items** property to this formula:
<br>**["Standard", "Premium"]**

	Don't know how to [add, name, and configure a control](add-configure-controls.md)?

1. Add a **Text box** control, move it below the **Radio** control, and set the **Text** property of the **Text box** control to this formula:
<br>**If("Premium" in Pricing.Selected.Value, "$200 per day", "$150 per day")**

	Want more information about the [**If** function](function-if.md) or [other functions](formula-reference.md)?

1. Press F5, and then choose either option in the **Radio** control.

	The **Text box** control shows the appropriate text for your choice.

1. (optional) In the **Radio** control, choose the other option to confirm that the appropriate text appears.

1. To return to the default workspace, press Esc.