# 6.6 Web API

{% hint style="warning" %}
The Web API is marked as deprecated in its current form and will be replaced by a REST service.
{% endhint %}

The Web API allows information on records to be obtained as JSON data records via a simple GET URL call. The data records of the hit set consist of statically defined and optional freely configurable fields. 

The following static fields are always included:

| **Field name**  | Content |
| :--- | :--- |
| **id** | Record identifier |
| **title**  | Record title |
| **dateCreated**  | Import date of the record into the Goobi viewer |
| **collection**  | First collection entry for this record |
| **thumbnailUrl**  | URL to the thumbnail image of the work in \(if available\) size 100x120px |
| **mediumimage**  | URL to the thumbnail image of the work in \(if available\) size 600x500px  |
| **url**  | URL to the image view of this record |



