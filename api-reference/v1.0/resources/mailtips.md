# <a name="mailtips-resource-type"></a>邮件提醒资源类型

有关收件人的提示消息，用户撰写消息时向用户显示。 例如，将外出邮件作为邮件收件人的自动答复。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| AutomaticReplies | [AutomaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | 邮件提示自动答复（如果它已由收件人设置）。 |
| CustomMailTip | 字符串 | 可以在收件人的邮箱上设置的自定义邮件提示。 |
| DeliveryRestricted| 布尔值 | 收件人的邮箱是否受限制，例如仅接受来自预定义的发件人列表的邮件，拒绝来自预定义的发件人列表的邮件，或仅接受来自经过验证的发件人的邮件。 |
| emailAddress | [emailAddress](../resources/emailaddress.md) | 收件人的邮件地址以获取邮件提醒。 |
| error | [mailTipsError](../resources/mailtipserror.md) | 在 [GetMailTips](../api/user_getmailtips.md) 操作期间发生的错误。 |
| ExternalMemberCount | Int32 | 外部成员的数量（如果收件人为通讯组列表）。 |
| isModerated |布尔值  | 是否向收件人发送邮件需要批准。 例如，如果收件人是大型通讯组列表，并且主持人已设置为批准发送到该通讯组列表的邮件，或者如果向收件人发送邮件需要收件人的经理批准。 |
| MailboxFull | 布尔值 | 收件人邮箱的完整状态。 |
| MaxMessageSize | Int32 | 为收件人的组织或邮箱配置的最大邮件大小。 |
| RecipientScope | recipientScopeType | 收件人的作用域。 可取值为：`none`、`internal`、`external`、`externalPartner`、`externalNonParther`。 例如，管理员可以将另一个组织设置为其“合作伙伴”。 如果管理员希望特定范围的用户可以访问某些邮件提醒，该范围很有用。 发件人可以告诉他们，他们的邮件可能会发送至组织以外的收件人，从而帮助他们做出关于措辞、语调和内容的正确决定。|
| RecipientSuggestions | [收件人](../resources/recipient.md) 集合 | 基于此前上下文所建议的收件人，它们出现在相同的邮件中。 |
| TotalMemberCount | Int32 | 收件人是通讯组列表的成员数量。 |

### <a name="recipientscopetype-values"></a>recipientScopeType 值

| 值
|:-------------------------
| none
| internal
| external
| externalPartner
| externalNonPartner


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
