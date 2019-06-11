# 6.8 Access restriction configuration

The Goobi viewer supports the possibility of making certain aspects of a work inaccessible or only accessible to certain circles. 

The prerequisite is that so-called access conditions are included in the source document of the work as a metadata. The corresponding values must be mapped in the Solr Index in the field `ACCESSCONDITION`:

{% code-tabs %}
{% code-tabs-item title="solr\_indexerconfig.xml" %}
```markup
<ACCESSCONDITION>
    <list>
        <item>
            <xpath>mets:xmlData/mods:mods/mods:accessCondition[@type='restriction on access']</xpath>
            <addToDefault>false</addToDefault>
            <addUntokenizedVersion>false</addUntokenizedVersion>
        </item>
    </list>
</ACCESSCONDITION>
```
{% endcode-tabs-item %}
{% endcode-tabs %}

