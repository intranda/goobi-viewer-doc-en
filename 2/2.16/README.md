# 2.16 Theme

If your Goobi viewer has been installed with its own theme, the corresponding name is contained in the following configuration element:

{% code-tabs %}
{% code-tabs-item title="config\_viewer.xml" %}
```markup
<viewer>
    <theme subTheme="true"
           mainTheme="reference"
           discriminatorField=""
           autoSwitch="true"
           addFilterQuery="false"
           filterQueryVisible="false" />
</viewer>
```
{% endcode-tabs-item %}
{% endcode-tabs %}

The `mainTheme` attribute contains the name of the theme. This must correspond to the folder name in which the theme files are located. 

Optionally, alternative themes can be added for certain records. The attribute `subtheme` must be set to `true`. 

The `discriminatorField` attribute contains the name of the index field used to identify the records for which different themes are to be used. In the example above, it is the digital collection. Switching to a sub-theme also causes all search queries to be filtered by the value of the `discriminatorField` configured field, as long as you are in this view, in order to focus the navigation visually as well as data-wise on a certain region or institution. If the attribute `filterQueryVisible` is set to `true` \(default value `false`\), the filter query is also written into the URL so that a filtered search query can be easily passed on via the URL. 

The attribute `autoSwitch` \(default value `true`\) can be used to determine whether a record that has the corresponding value of the field configured in `discriminatorField` should be automatically switched to the corresponding subtheme with search filter when it is opened. If this switch is deactivated, a subtheme must be explicitly switched on \(for example via a menu\).

{% hint style="info" %}
Basically, the Goobi viewer is delivered with only one theme. If the theme definition is changed to an invalid value, empty pages are displayed.
{% endhint %}

