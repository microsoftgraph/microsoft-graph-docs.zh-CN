<a id="configuring-the-invitation-message" class="xliff"></a>
# 配置邀请邮件

使用 invitedUserMessageInfo 对象可以配置[邀请](invitation.md)邮件。


<a id="properties" class="xliff"></a>
## 属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|ccRecipients|[收件人](recipient.md)|应接收邀请邮件的其他收件人。当前仅支持 1 个其他收件人。|
|customizedMessageBody|字符串|在不希望发送默认邮件的情况下，要发送的自定义邮件正文。|
|messageLanguage|字符串|要发送的默认邮件的语言。如果指定了 customizedMessageBody，则忽略此属性，并使用 customizedMessageBody 发送该邮件。语言格式应为 ISO 639 格式。默认为 zh-CN。|


<a id="json-representation" class="xliff"></a>
## JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {"blockType": "resource", "@odata.type": "microsoft.graph.invitedUserMessageInfo"} -->
```json
{
  "ccRecipients": [ {"@odata.type": "microsoft.graph.recipient"} ],
  "customizedMessageBody": "string",
  "messageLanguage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
