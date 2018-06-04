# <a name="create-and-send-outlook-messages"></a>创建和发送 Outlook 邮件

电子邮件通过 Microsoft Graph 中的[邮件](../api-reference/v1.0/resources/message.md)资源表示。 

默认情况下，邮件由 **ID** 属性中的唯一条目 ID 标识。 当邮件最初保存为草稿或已发送时，存储提供程序会为消息分配一个条目 ID。 当将邮件复制或移动到另一个文件夹、存储或 .PST 文件时，该 ID 会发生变化。

## <a name="creating-and-sending-mail"></a>创建和发送邮件

在 Outlook 中，你可以在同一 [sendMail](../api-reference/v1.0/api/user_sendmail.md) 操作中创建和发送电子邮件，或者可以[创建](../api-reference/v1.0/api/user_post_messages.md)草稿，然后[添加内容](../api-reference/v1.0/api/message_update.md)并[发送](../api-reference/v1.0/api/message_send.md)此草稿。

同样，在回复电子邮件时，也可以使用相同的操作（[答复](../api-reference/v1.0/api/message_reply.md)、[全部答复](../api-reference/v1.0/api//message_replyall.md)或[转发](../api-reference/v1.0/api/message_forward.md)）创建和发送响应。 或者，你可以为响应（[答复](../api-reference/v1.0/api/message_createreply.md)、[全部答复](../api-reference/v1.0/api//message_createreplyall.md)或[转发](../api-reference/v1.0/api/message_createforward.md)）创建草稿，[添加内容](../api-reference/v1.0/api/message_update.md)），然后稍后[发送](../api-reference/v1.0/api/message_send.md)此草稿。

要以编程方式区分草稿和已发送邮件，请选中 **isDraft** 属性。 

默认情况下，草稿邮件保存在 `Drafts` 文件夹中，已发送邮件保存在 `Sent Items` 文件夹中。 为方便起见，你可以通过相应的已知文件夹名称来识别 Drafts 文件夹和 SentItems 文件夹。 例如，你可以执行以下操作[获取 Drafts 文件夹中的邮件](../api-reference/v1.0/api/user_list_messages.md)：

```http
GET /me/mailfolders('Drafts')
```

### <a name="body-format-and-malicious-script"></a>正文格式和恶意脚本

<!-- Remove the following 2 sections from the message.md topics 
-->

邮件正文可以是 HTML 或文本，其中 HTML 作为 GET 响应中返回的默认邮件正文类型。

当[获取邮件](../api-reference/v1.0/api/message_get.md)时，你可以指定以下请求标头以文本格式返回 **body** 和 **uniqueBody** 属性：

```
Prefer: outlook.body-content-type="text"
```
你可以指定以下标头（或直接跳过标头），以 HTML 格式获取邮件正文：
```
Prefer: outlook.body-content-type="html"
```

当指定任一标头时，成功的响应将包含相应的 `Preference-Applied` 标头：

- 对于文本格式请求：`Preference-Applied: outlook.body-content-type="text"`
- 对于 HTML 格式请求：`Preference-Applied: outlook.body-content-type="html"`

默认情况下，如果正文是 HTML 格式，那么在 REST 响应中返回正文内容之前，Outlook 将删除嵌入 **body** 属性中的任何具有潜在不安全性的 HTML（例如 JavaScript）。

若要获取整个原始 HTML 内容，请包括以下 HTTP 请求标头：
```
Prefer: outlook.allow-unsafe-html
```

### <a name="differentiating-the-from-and-sender-properties"></a>区分 from 和 sender 属性

撰写邮件时，Outlook 在大多数情况下会将 **from** 和 **sender** 属性设置为同一登录用户。 你可以在以下情况下更新这些属性：

- 如果 Exchange 管理员已将邮箱的 **sendAs** 权限分配给其他一些用户，可以更改 **from** 属性。为此，管理员可以在 Azure 门户中选择邮箱所有者的**邮箱权限**，也可以使用 Exchange 管理中心或 Windows PowerShell Add-ADPermission cmdlet。然后，可以编程方式将 **from** 属性设置为，对相应邮箱拥有 **sendAs** 权限的用户之一。
- 如果邮箱所有者已委派一个或多个用户能够从该邮箱发送邮件，则可以更改 **sender** 属性。 可以在 Outlook 中委派邮箱所有者。 当代理代表邮箱所有者发送邮件时，Outlook 将 **sender** 属性设置为代理的帐户，**from** 属性仍保持为邮箱所有者。 通过编程方式，你可以将 **sender** 属性设置为已拥有邮箱委派权限的用户。

## <a name="using-mailtips-to-check-recipient-status-and-save-time-preview"></a>使用邮件提醒检查收件人状态并节省时间（预览版）

在发送电子邮件之前，可使用[邮件提醒](../api-reference/beta/resources/mailtips.md)做出明智的决定。 邮件提醒可以告诉你诸如收件人的邮箱限于特定发件人，或者需要批准才能向收件人发送电子邮件等信息。

## <a name="integrating-with--social-gesture-preview"></a>与“@”社交手势集成（预览版）

@-mention 是提醒用户邮件中是否有提到他们的通知。 [mention](../api-reference/beta/resources/mention.md)资源使应用能够在电子邮件中设置和获取常见的在线社交手势，即“@”前缀。
可以执行下列操作：

- 在[创建邮件](../api-reference/beta/api/user_post_messages.md#request-2)时创建 @-mention
- [获取用户邮箱中包含用户 @-mention 的所有邮件](../api-reference/beta/api/user_list_messages.md#request-2)
- [获取所有 @-mention 就形成一封邮件](../api-reference/beta/api/message_get.md#request-2) 


## <a name="other-shared-capabilities"></a>其他共享的功能

利用以下在 Microsoft Graph 实体之间共享的常用功能：

- 发生一种或多种类型的更改时（如创建或更新邮件），订阅邮件的[更改通知](../api-reference/v1.0/resources/webhooks.md)。
- [跟踪文件夹中邮件的这些增量更改](delta_query_messages.md)
- 创建[开放扩展](extensibility_overview.md#open-extensions)或[架构扩展](extensibility_overview.md#schema-extensions)，以将自定义数据添加到邮件实例。
- 当 Outlook MAPI 属性尚未通过 Microsoft Graph API 元数据公开时，在邮件实例中创建[扩展属性](../api-reference/v1.0/resources/extended-properties-overview.md)以存储这些属性的自定义数据。

## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- [为什么与 Outlook 邮件集成](outlook-mail-concept-overview.md)
- [使用邮件 API](../api-reference/v1.0/resources/mail_api_overview.md) 及其在 Microsoft Graph v1.0 中的[用例](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases)。