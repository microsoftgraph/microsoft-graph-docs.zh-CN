<span data-ttu-id="49cfe-p118">若要获取新扩展，首先 [获取此线程中的所有帖子](../api/conversationthread_list_posts.md)，线程中最初应该只有一个帖子。然后应用帖子 ID 和扩展名 `Com.Contoso.Benefits` 以[获取扩展](../api/opentypeextension_get.md)。</span><span class="sxs-lookup"><span data-stu-id="49cfe-p118">To get the new extension, first [get all the posts](../api/conversationthread_list_posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension_get.md).</span></span>

若要获取新扩展，首先 [获取此线程中的所有帖子](../api/conversationthread_list_posts.md)，线程中最初应该只有一个帖子。然后应用帖子 ID 和扩展名 `Com.Contoso.Benefits` 以[获取扩展](../api/opentypeextension_get.md)。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
    "threads": [
        {
            "id": "AAQkADJDtMUzsf_PdhAAswJOhGVsnkyDtMUzsf_Pdg=="
        }
    ]
}

```


<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
