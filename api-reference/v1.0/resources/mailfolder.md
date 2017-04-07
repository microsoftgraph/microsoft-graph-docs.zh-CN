# <a name="mailfolder-resource-type"></a>mailFolder 资源类型

用户邮箱中的 mailFolder，例如收件箱、草稿箱和已发送邮件。MailFolders 可包含邮件和子 mailFolder。


## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 mailFolder](../api/mailfolder_get.md) | [mailFolder](mailfolder.md) |读取 mailFolder 对象的属性和关系。|
|[创建 MailFolder](../api/mailfolder_post_childfolders.md) |[MailFolder](mailfolder.md)| 通过发布到 childFolder 集合，在当前 mailFolder 下新建 mailFolder。|
|[列出 childFolder](../api/mailfolder_list_childfolders.md) |[MailFolder](mailfolder.md) 集合| 获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。|
|[创建邮件](../api/mailfolder_post_messages.md) |[邮件](message.md)| 通过发布到邮件集合，在当前 mailFolder 中新建邮件。|
|[列出邮件](../api/mailfolder_list_messages.md) |[邮件](message.md) 集合| 获取已登录用户邮箱中的所有邮件或邮箱的指定文件夹中的邮件。|
|[更新](../api/mailfolder_update.md) | [mailFolder](mailfolder.md)|更新指定的 mailFolder 对象。 |
|[删除](../api/mailfolder_delete.md) | 无 |删除指定的 mailFolder 对象。 |
|[复制](../api/mailfolder_copy.md)|[MailFolder](mailfolder.md)|将 mailfolder 及其内容复制到其他 mailfolder。|
|[移动](../api/mailfolder_move.md)|[MailFolder](mailfolder.md)|将 mailFolder 及其内容移动到其他 mailFolder。|
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[mailFolder](mailFolder.md)  |在新建或现有的 mailFolder 中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的 mailFolder](../api/singlevaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | 通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 mailFolder。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [mailFolder](mailFolder.md) | 在新建或现有的 mailFolder 中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的 mailFolder](../api/multivaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | 使用 `$expand` 获取包含一个多值扩展属性的 mailFolder。 |


## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|childFolderCount|Int32|当前 mailFolder 中的直接子 mailFolder 数量。|
|displayName|String|mailFolder 的显示名称。|
|id|String|MailFolder 的唯一标识符。可以使用以下已知名称访问相应的文件夹：收件箱、草稿箱、已发送邮件、已删除邮件。|
|parentFolderId|String|MailFolder 的父 mailFolder 的唯一标识符。|
|totalItemCount|Int32|邮箱中项的数量|
|unreadItemCount|Int32|mailFolder 中标记为未读的项的数量。|

**有效的访问项计数**

使用文件夹的 TotalItemCount 和 UnreadItemCount 的属性可以方便地计算在文件夹中读取的项数。使你避免进行可产生重大延迟的查询，如下所示：
```
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```
Outlook 中的 MailFolder 可包含多个类型的项，例如，收件箱可以包含不同于邮件项的会议请求项。无论项目类型如何，TotalItemCount 和 UnreadItemCount 包括 mailFolder 中的项。


## <a name="relationships"></a>关系
| 关系 | 类型    |说明|
|:---------------|:--------|:----------|
|childFolders|[MailFolder](mailfolder.md) 集合|mailFolder 中的子文件夹集合。|
|邮件|[邮件](message.md) 集合|mailFolder 中的邮件集合。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为 mailFolder 定义的多值扩展属性的集合。只读。可为 NULL。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为 mailFolder 定义的单值扩展属性的集合。只读。可为 NULL。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailFolder"
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
