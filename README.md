LoadingIndicators.WPF
====================
![Demo](./demo.gif)

LoadingIndicators.WPF is a collection of 8 animated loading indicators for WPF compatible with [MahApps.Metro](https://github.com/MahApps/MahApps.Metro).

## Styles
- Arcs
- Arcs Ring
- Double Bounce
- FlipPlane
- Pulse
- Ring
- Three Dots
- Wave

## Features
- Variable Animation Speed
- Easy activation/deactivation
- Easy change of theme using resources
- Out of the box [MahApps.Metro](https://github.com/MahApps/MahApps.Metro) compatibility

## Usage
- Include Namespace
```xml
<Window ...
        xmlns:li="http://github.com/zeluisping/loadingIndicators/xaml/controls">
```
- Add Loading indicator and select mode
```xml
```<Window.Resources>
       
        <ResourceDictionary>            
            <ResourceDictionary.MergedDictionaries>
                <ResourceDictionary Source="pack://application:,,,/LoadingIndicators.WPF;component/Styles/LoadingArcs.xaml"/>
            <ResourceDictionary Source="pack://application:,,,/LoadingIndicators.WPF;component/Styles.xaml"/>
                
            </ResourceDictionary.MergedDictionaries>
    </ResourceDictionary>
    </Window.Resources>
<li:LoadingIndicator Grid.Column="0" SpeedRatio="2" Visibility="{Binding LoadingIndicator}" IsActive="true" Style="{DynamicResource LoadingIndicatorThreeDotsStyle}" />
```

Note: Waves mode will be selected by default if left empty
