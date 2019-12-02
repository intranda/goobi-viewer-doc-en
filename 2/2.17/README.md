# 2.17 Search

The search in the Goobi viewer allows a combined search both in the metadata and in the full texts. Depending on the selection, a search can also be restricted to the metadata or the full texts of the digital collections. Links of search terms, a search with right or left truncation or a phrase search are also possible.

![Simple search](../../.gitbook/assets/2.17.png)

Depending on the precision of the search query and the number of indexed records, hundreds or thousands of search hits may be displayed on a search hit list spread over several pages. The number of search hits displayed per page can be configured using the following element \(the default value is 10\):

{% code title="config\_viewer.xml" %}
```markup
<search>
    <hitsPerPage>10</hitsPerPage>
    <fulltextFragmentLength>120</fulltextFragmentLength>
</search>
```
{% endcode %}

The element `fulltextFragmentLength` defines the approximate length of the full text sections for the search hit display. The default value is 200. 

The following configuration block is available to define the search ranges of the simple search:

{% code title="config\_viewer.xml" %}
```markup
<search>
    <filters>
        <filter>filter_ALL</filter>
        <filter>filter_DEFAULT</filter>
        <filter>filter_FULLTEXT</filter>
        <!-- <filter>filter_NORMDATATERMS</filter> -->
        <!-- <filter>filter_UGCTERMS</filter> -->
        <!-- <filter>filter_OVERVIEWPAGE</filter> -->
    </filters>
</search>
```
{% endcode %}

Each filter entry creates a new radio button below the simple search.

