<span data-ttu-id="359c2-p103">注意：为简洁起见，可能会截断此处展示的响应对象。实际调用会返回[默认属性](../api/group_get.md#default-properties)。</span><span class="sxs-lookup"><span data-stu-id="359c2-p103">Note: The response object shown here may be truncated for brevity. The [default properties](../api/group_get.md#default-properties) will be returned from an actual call.</span></span>

注意：为简洁起见，可能会截断此处展示的响应对象。实际调用会返回[默认属性](../api/group_get.md#default-properties)。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

 {
  "value": [
    {
      "id": "id-value",
      "description": "description-value",
      "displayName": "displayName-value",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "mailEnabled": true,
      "mailNickname": "mailNickname-value",
      "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
      "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
      "onPremisesSyncEnabled": true,
      "proxyAddresses": [
        "proxyAddresses-value"
      ],
      "securityEnabled": true,
      "visibility": "visibility-value"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
