---
-api-id: P:Windows.UI.Xaml.FrameworkElement.MaxWidth
-api-type: winrt property
---

<!-- Property syntax
public double MaxWidth { get;  set; }
-->

# Windows.UI.Xaml.FrameworkElement.MaxWidth

## -description
Gets or sets the maximum width constraint of a [FrameworkElement](frameworkelement.md).

## -xaml-syntax
```xaml
<frameworkElement MaxWidth="double"/>
 
```


## -property-value
The maximum width of the object, in pixels. The default is [PositiveInfinity](https://msdn.microsoft.com/library/system.double.positiveinfinity.aspx). This value can be any value equal to or greater than 0. [PositiveInfinity](https://msdn.microsoft.com/library/system.double.positiveinfinity.aspx) is also valid.

## -remarks
[MaxWidth](frameworkelement_maxwidth.md) is one of three writable properties on [FrameworkElement](frameworkelement.md) that specify width information. The other two are [MinWidth](frameworkelement_minwidth.md) and [Width](frameworkelement_width.md). If there is a conflict between these values, the order of application for actual width determination is that first [MinWidth](frameworkelement_minwidth.md) must be honored, then [MaxWidth](frameworkelement_maxwidth.md), and finally, if it is within bounds, [Width](frameworkelement_width.md). All of these properties are recommendations to the layout behavior of the element's parent in the object tree. The width of the object after layout runs is available as the [ActualWidth](frameworkelement_actualwidth.md) property value.

The final [ActualWidth](frameworkelement_actualwidth.md) of an element might exceed [MaxWidth](frameworkelement_maxwidth.md). For example, if [UseLayoutRounding](uielement_uselayoutrounding.md) is set to **true** and your app is running on a display with a Resolution Scale greater than 100%, then the [ActualWidth](frameworkelement_actualwidth.md) may be rounded up to help ensure your UI doesn't look blurry when scaled.

## -examples
This XAML example shows a technique of specifying a [MaxWidth](frameworkelement_maxwidth.md) for a [ViewBox](../windows.ui.xaml.controls/viewbox.md). [ViewBox](../windows.ui.xaml.controls/viewbox.md) is a decorator that can apply layout information to a single child and divide layout areas for the next parent element (in this case a [StackPanel](../windows.ui.xaml.controls/stackpanel.md)).



[!code-xml[ViewBoxXAML](../windows.ui.xaml/code/ViewBoxSnippet/csharp/MainPage.xaml#SnippetViewBoxXAML)]

## -see-also
[Width](frameworkelement_width.md), [MinWidth](frameworkelement_minwidth.md), [Define layouts with XAML](http://msdn.microsoft.com/library/8d4e4162-1c9c-48f4-8a94-34976fb17079)