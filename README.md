# How can customize the filter and advanced filter appearance of  WPF DataGrid (SfDataGrid) ? 

How can customize the filter and advanced filter appearance of  WPF DataGrid (SfDataGrid) ? 

# About the sample

In SfDataGrid, you customize the appearance of GridFilterControl and AdvancedFilterControl by overriding its ControlTemplate.

```Xaml
<!--Filter Style-->
<Style x:Key="ButtonFocusVisual">
    <Setter Property="Control.Template">
        <Setter.Value>
            <ControlTemplate>
                <Rectangle SnapsToDevicePixels="true"
                            Stroke="{DynamicResource {x:Static SystemColors.ControlTextBrushKey}}"
                            StrokeDashArray="1 2"
                            StrokeThickness="1" />
            </ControlTemplate>
        </Setter.Value>
    </Setter>
</Style>

<!--Advanced Filter Style-->
<Style x:Key="ComboBoxFocusVisual">
    <Setter Property="Control.Template">
        <Setter.Value>
            <ControlTemplate>
                <Rectangle Margin="4,4,19,4"
                            SnapsToDevicePixels="true"
                            Stroke="Black"
                            StrokeDashArray="1 2"
                            StrokeThickness="1" />
            </ControlTemplate>
        </Setter.Value>
    </Setter>
</Style>
```
## Requirements to run the demo
 Visual Studio 2015 and above versions
