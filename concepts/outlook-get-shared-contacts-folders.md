# <a name="get-outlook-contacts-in-a-shared-folder"></a>获取共享文件夹中的 Outlook 联系人

Outlook 允许客户相互共享文件夹，并提供对个人联系人文件夹的“读取”、“创建”、“修改”或“删除”等访问权限。 Outlook 还允许客户委派另一个用户代表客户操作并访问特定的文件夹或客户的整个邮箱；这在 Outlook 中也称为“委派”。

Microsoft Graph 以编程方式支持在其他用户共享的联系人文件夹中获取联系人，以及获取共享文件夹本身。 该支持还适用于委派邮箱中的文件夹。

例如，Garth 与 John 共享了他的自定义联系人文件夹，并授予 John 读取访问权限。 如果 John 已登录你的应用并提供了委派权限 (Contacts.Read.Shared or Contacts.ReadWrite.Shared)，则你的应用将能够访问 Garth 的自定义联系人文件夹和文件夹中的联系人，如下所述。

## <a name="get-a-contact-in-the-shared-folder"></a>获取共享文件夹中联系人

你可以获取 Garth 与 John 共享的自定义联系人文件夹中的特定联系人：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

成功完成后，你将收到“HTTP 200 正常”消息以及 Garth 共享联系人文件夹中由 `{id}` 标识的[联系人](../api-reference/v1.0/resources/contact.md)实例。

## <a name="get-all-contacts-in-the-shared-folder"></a>获取共享文件夹中的所有联系人

获取 Garth 的共享联系人文件夹中的所有联系人：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

成功完成后，你将收到“HTTP 200 正常”消息以及 Garth 共享联系人文件夹中的[联系人](../api-reference/v1.0/resources/contact.md)实例的集合。

## <a name="get-the-shared-folder"></a>获取共享文件夹

获取 Garth 与 John 共享的联系人文件夹。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

成功完成后，你将收到“HTTP 200 正常”消息以及表示 Garth 共享联系人文件夹的 [contactFolder](../api-reference/v1.0/resources/contactfolder.md) 实例。

如果 Garth 已将其整个邮箱委派给 John，那么可应用相同的 GET 功能。

如果 Garth 未与 John 共享联系人文件夹，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。 


## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- [为何要与 Outlook 个人联系人集成](outlook-contacts-concept-overview.md)
- Microsoft Graph v1.0 中的 [联系人 API](../api-reference/v1.0/resources/contact.md)。