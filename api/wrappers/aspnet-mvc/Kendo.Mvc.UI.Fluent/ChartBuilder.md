---
title:ChartBuilder
slug:aspnetmvc-kendo.mvc.ui.fluent.chartbuilder
publish:true
---

# Kendo.Mvc.UI.Fluent.ChartBuilder

Defines the fluent interface for configuring the !:Chart{T} component.

## Methods

### Events(System.Action\<Kendo.Mvc.UI.Fluent.ChartEventBuilder\>)
Configures the client-side events.

#### Example
    <%= Html.Kendo().Chart()
        .Name("Chart")
        .Events(events => events
        .OnLoad("onLoad")
        )
        %>

#### Parameters

##### configurator System.Action\<[Kendo.Mvc.UI.Fluent.ChartEventBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartEventBuilder)\>
The client events configuration action.

### Theme(System.String)
Sets the theme of the chart.

#### Example
    <%= Html.Kendo().Chart()
        .Name("Chart")
        .Theme("Telerik")
        %>

#### Parameters

##### theme `System.String`
The Chart theme.

### ChartArea(System.Action\<Kendo.Mvc.UI.Fluent.ChartAreaBuilder\>)
Sets the Chart area.

#### Example
    <%= Html.Kendo().Chart()
        .Name("Chart")
        .ChartArea(chartArea => chartArea.margin(20))
        %>

#### Parameters

##### configurator System.Action\<[Kendo.Mvc.UI.Fluent.ChartAreaBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartAreaBuilder)\>
The Chart area.

### PlotArea(System.Action\<Kendo.Mvc.UI.Fluent.PlotAreaBuilder\>)
Sets the Plot area.

#### Example
    <%= Html.Kendo().Chart()
        .Name("Chart")
        .PlotArea(plotArea => plotArea.margin(20))
        %>

#### Parameters

##### configurator System.Action\<[Kendo.Mvc.UI.Fluent.PlotAreaBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/PlotAreaBuilder)\>
The Plot area.

### Title(System.String)
Sets the title of the chart.

#### Example
    <%= Html.Kendo().Chart()
        .Name("Chart")
        .Title("Yearly sales")
        %>

#### Parameters

##### title `System.String`
The Chart title.

### Title(System.Action\<Kendo.Mvc.UI.Fluent.ChartTitleBuilder\>)
Defines the title of the chart.

#### Example
    <%= Html.Kendo().Chart()
        .Name("Chart")
        .Title(title => title.Text("Yearly sales"))
        %>

#### Parameters

##### configurator System.Action\<[Kendo.Mvc.UI.Fluent.ChartTitleBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartTitleBuilder)\>
The configuration action.

### Legend(System.Boolean)
Sets the legend visibility.

#### Example
    <%= Html.Kendo().Chart()
        .Name("Chart")
        .Legend(false)
        %>

#### Parameters

##### visible `System.Boolean`
A value indicating whether to show the legend.

### Legend(System.Action\<Kendo.Mvc.UI.Fluent.ChartLegendBuilder\>)
Configures the legend.

#### Example
    <%= Html.Kendo().Chart()
        .Name("Chart")
        .Legend(legend => legend.Visible(true).Position(ChartLegendPosition.Bottom))
        %>

#### Parameters

##### configurator System.Action\<[Kendo.Mvc.UI.Fluent.ChartLegendBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartLegendBuilder)\>
The configuration action.

### Series(System.Action\<Kendo.Mvc.UI.Fluent.ChartSeriesFactory\<T\>\>)
Defines the chart series.

#### Example
    <%= Html.Kendo().Chart(Model)
        .Name("Chart")
        .Series(series =>
        {
        series.Bar(s => s.SalesAmount);
        })
        %>

#### Parameters

##### configurator System.Action\<[Kendo.Mvc.UI.Fluent.ChartSeriesFactory](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartSeriesFactory)\<T\>\>
The add action.

### SeriesDefaults(System.Action\<Kendo.Mvc.UI.Fluent.ChartSeriesDefaultsBuilder\<T\>\>)
Defines the options for all chart series of the specified type.

#### Example
    <%= Html.Kendo().Chart(Model)
        .Name("Chart")
        .SeriesDefaults(series => series.Bar().Stack(true))
        %>

#### Parameters

##### configurator System.Action\<[Kendo.Mvc.UI.Fluent.ChartSeriesDefaultsBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartSeriesDefaultsBuilder)\<T\>\>
The configurator.

### AxisDefaults(System.Action\<Kendo.Mvc.UI.Fluent.ChartAxisDefaultsBuilder\<T\>\>)
Defines the options for all chart axes of the specified type.

#### Example
    <%= Html.Kendo().Chart(Model)
        .Name("Chart")
        .AxisDefaults(axisDefaults => axisDefaults.MinorTickSize(5))
        %>

#### Parameters

##### configurator System.Action\<[Kendo.Mvc.UI.Fluent.ChartAxisDefaultsBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartAxisDefaultsBuilder)\<T\>\>
The configurator.

### CategoryAxis(System.Action\<Kendo.Mvc.UI.Fluent.ChartCategoryAxisBuilder\<T\>\>)
Configures the category axis

#### Example
    <%= Html.Kendo().Chart(Model)
        .Name("Chart")
        .CategoryAxis(axis => axis
        .Categories(s => s.DateString)
        )
        %>

#### Parameters

##### configurator System.Action\<[Kendo.Mvc.UI.Fluent.ChartCategoryAxisBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartCategoryAxisBuilder)\<T\>\>
The configurator

### ValueAxis(System.Action\<Kendo.Mvc.UI.Fluent.ChartValueAxisFactory\<T\>\>)
Defines value axis options

#### Example
    <%= Html.Kendo().Chart(Model)
        .Name("Chart")
        .ValueAxis(a => a.Numeric().TickSize(4))
        %>

#### Parameters

##### configurator System.Action\<[Kendo.Mvc.UI.Fluent.ChartValueAxisFactory](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartValueAxisFactory)\<T\>\>
The configurator

### XAxis(System.Action\<Kendo.Mvc.UI.Fluent.ChartValueAxisFactory\<T\>\>)
Defines X-axis options for scatter charts

#### Example
    <%= Html.Kendo().Chart(Model)
        .Name("Chart")
        .XAxis(a => a.Numeric().Max(4))
        %>

#### Parameters

##### configurator System.Action\<[Kendo.Mvc.UI.Fluent.ChartValueAxisFactory](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartValueAxisFactory)\<T\>\>
The configurator

### YAxis(System.Action\<Kendo.Mvc.UI.Fluent.ChartValueAxisFactory\<T\>\>)
Configures Y-axis options for scatter charts.

#### Example
    <%= Html.Kendo().Chart(Model)
        .Name("Chart")
        .YAxis(a => a.Numeric().Max(4))
        %>

#### Parameters

##### configurator System.Action\<[Kendo.Mvc.UI.Fluent.ChartValueAxisFactory](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartValueAxisFactory)\<T\>\>
The configurator

### DataSource(System.Action\<Kendo.Mvc.UI.Fluent.ReadOnlyAjaxDataSourceBuilder\<T\>\>)
Data Source configuration

#### Example
    <%= Html.Kendo().Chart()
        .Name("Chart")
        .DataSource(ds =>
        {
        ds.Ajax().Read(r => r.Action("SalesData", "Chart"));
        })
        %>

#### Parameters

##### configurator System.Action\<[Kendo.Mvc.UI.Fluent.ReadOnlyAjaxDataSourceBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ReadOnlyAjaxDataSourceBuilder)\<T\>\>
Use the configurator to set different data binding options.

### SeriesColors(System.Collections.Generic.IEnumerable\<System.String\>)
Sets the series colors.

#### Example
    <%= Html.Kendo().Chart()
        .Name("Chart")
        .SeriesColors(new string[] { "#f00", "#0f0", "#00f" })
        %>

#### Parameters

##### colors `System.Collections.Generic.IEnumerable<System.String>`
A list of the series colors.

### SeriesColors(System.String[])
Sets the series colors.

#### Example
    <%= Html.Kendo().Chart()
        .Name("Chart")
        .SeriesColors("#f00", "#0f0", "#00f")
        %>

#### Parameters

##### colors `System.String[]`
The series colors.

### Tooltip(System.Action\<Kendo.Mvc.UI.Fluent.ChartTooltipBuilder\>)
Use it to configure the data point tooltip.

#### Example
    <%= Html.Kendo().Chart()
        .Name("Chart")
        .Tooltip(tooltip =>
        {
        tooltip.Visible(true).Format("{0:C}");
        })
        %>

#### Parameters

##### configurator System.Action\<[Kendo.Mvc.UI.Fluent.ChartTooltipBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/ChartTooltipBuilder)\>
Use the configurator to set data tooltip options.

### Tooltip(System.Boolean)
Sets the data point tooltip visibility.

#### Example
    <%= Html.Kendo().Chart()
        .Name("Chart")
        .Tooltip(true)
        %>

#### Parameters

##### visible `System.Boolean`
A value indicating if the data point tooltip should be displayed.
            The tooltip is not visible by default.

### Transitions(System.Boolean)
Enables or disabled animated transitions on initial load and refresh.

#### Example
    <%= Html.Kendo().Chart()
        .Name("Chart")
        .Transitions(false)
        %>

#### Parameters

##### transitions `System.Boolean`
A value indicating if transition animations should be played.