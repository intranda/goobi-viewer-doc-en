# 1.16 Theme

If your Goobi viewer has been installed with its own theme, the corresponding name is contained in the following configuration element:

{% tabs %}
{% tab title="config_viewer.xml" %}
```markup
<viewer>
    <theme mainTheme="reference" discriminatorField=""/>
</viewer>
```
{% endtab %}
{% endtabs %}

The `mainTheme` attribute contains the name of the theme. This must correspond to the folder name in which the theme files are located.&#x20;

The optional attribute `discriminatorField` contains the name of the index field which is used to identify the works for which deviating CSS should be used.

{% hint style="info" %}
Basically, the Goobi viewer is delivered with only one theme. If the theme definition is changed to an invalid value, empty pages are displayed.
{% endhint %}
