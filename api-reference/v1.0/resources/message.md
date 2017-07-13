<span data-ttu-id="74d39-p122">为邮件定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="74d39-p122">The collection of single-value extended properties defined for the message. Read-only. Nullable.</span></span>| 为邮件定义的单值扩展属性的集合。只读。可为 Null。|


## <span data-ttu-id="74d39-330">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74d39-330">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="74d39-331">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74d39-331">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.message"
}-->

```json
{
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "string",
  "conversationId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageId": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "parentFolderId": "string",
  "receivedDateTime": "String (timestamp)",
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```

## <span data-ttu-id="74d39-332">另请参阅</span><span class="sxs-lookup"><span data-stu-id="74d39-332">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="74d39-333">获取邮箱设置</span><span class="sxs-lookup"><span data-stu-id="74d39-333">Get mailbox settings</span></span>](../api/user_get_mailboxsettings.md) 
- [<span data-ttu-id="74d39-334">更新邮箱设置</span><span class="sxs-lookup"><span data-stu-id="74d39-334">Update mailbox settings</span></span>](../api/user_update_mailboxsettings.md)
- [<span data-ttu-id="74d39-335">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="74d39-335">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="74d39-336">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="74d39-336">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)
- [<span data-ttu-id="74d39-337">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="74d39-337">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="74d39-338">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="74d39-338">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="74d39-339">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="74d39-339">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
