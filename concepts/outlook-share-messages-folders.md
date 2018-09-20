# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a>获取一个共享或委派文件夹中的 Outlook 邮件

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

Outlook 允许客户相互共享邮件文件夹，并提供对个人文件夹的“读取”、“创建”、“修改”或“删除”等访问权限。 Outlook 还允许客户委派另一个用户代表客户操作并访问特定的邮件文件夹或客户的整个邮箱；这在 Outlook 中也称为“委派”。

Microsoft Graph 以编程方式支持在其他用户共享的邮件文件夹中获取邮件，以及获取共享文件夹本身。 该支持还适用于已委派的文件夹。

举个例子，Garth 已经与 John 共享并授予他 Garth 收件箱的读取访问权限。 如果 John 已登录你的应用并提供了委派权限 (Mail.Read.Shared or Mail.ReadWrite.Shared)，则你的应用将能够访问 Garth 的邮件和 Garth 的收件箱，如下所述。

## <a name="get-a-message-in-the-shared-folder"></a>获取共享文件夹中的邮件

你可以在 Garth 的收件箱中获取特定邮件：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

成功完成后，你将收到“HTTP 200 正常”消息和由来自 Garth 收件箱的 `{id}` 标识的[消息](../api-reference/v1.0/resources/message.md)实例。

## <a name="get-all-messages-in-the-shared-folder"></a>获取共享文件夹中的全部邮件

获取 Garth 收件箱中的所有邮件：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

成功完成后，你将收到“HTTP 200 正常”消息和 Garth 收件箱中的[消息](../api-reference/v1.0/resources/message.md)实例的集合。

## <a name="get-the-shared-folder"></a>获取共享文件夹

获取 Garth 与 John 共享的文件夹（收件箱）。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

成功完成后，你将收到“HTTP 200 正常”消息和表示 Garth 收件箱文件夹的 [mailFolder](../api-reference/v1.0/resources/mailfolder.md) 实例。

如果 Garth 已经委派 John 进一步访问他的收件箱，或者如果 Garth 已将其整个邮箱委派给 John，那么可应用相同的 GET 功能。

如果 Garth 未与 John 共享他的收件箱，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。 


## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- [为什么与 Outlook 邮件集成](outlook-mail-concept-overview.md)
- [使用邮件 API](../api-reference/v1.0/resources/mail_api_overview.md) 及其在 Microsoft Graph v1.0 中的[用例](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases)。