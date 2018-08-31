# <a name="mailfolder-resource-type"></a>mailFolder 资源类型

用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。 邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。

该资源支持通过提供 [delta](../api/mailfolder_delta.md) 函数使用[增量查询](../../../concepts/delta_query_overview.md)跟踪增量添加、删除和更新。

**已知文件夹名**

Outlook 默认情况下会为用户创建某些文件夹。 访问这些文件夹时，为方便起见，你可以使用下表中的已知文件夹名而不必使用的相应文件夹 **ID** 值。 例如，你可以通过以下查询使用其已知名称来获取草稿箱文件夹。

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

已知名称不分用户邮箱的区域设置一律奏效，所以上述查询将不顾文件夹的命名方式而始终返回用户的草稿箱文件夹。

| 已知文件夹名 | 说明 |
|:-----------------------|:------------|
| 存档 | 在支持的 Outlook 客户端使用“One_Click 存档”功能时，就可发送存档文件夹邮件。 **注意：** 这个与 Exchange online 的“存档邮箱”功能不一样。 |
| 混乱邮件 | 在使用“混乱邮件”功能时，就可移动混乱文件夹低优先级邮件了。 |
| 冲突 | 邮箱中包含冲突项目的文件夹。 |
| conversationhistory | Skype 保存 IM 对话（如果 Skype 配置这样做）的文件夹。 |
| deleteditems | 删除文件夹项目时，就可移动文件夹项目了。 |
| 草稿 | 包含未发送邮件的文件夹。 |
| 收件箱 | 收件箱文件夹。 |
| junkemail | 垃圾邮件文件夹。 |
| localfailures | 包含存在于本地客户端上，但无法上传到服务器的项目的文件夹。 |
| msgfolderroot | “Information Store 顶端”文件夹。 这个文件夹是普通邮件客户端中显示的如收件箱之类文件夹的父文件夹。 |
| 发件箱 | 发件箱文件夹。 |
| recoverableitemsdeletions | 包含软删除项目的文件夹：从“已删除邮件”文件夹中删除的，或在 Outlook 中通过按 shift+delete 删除的。 这个文件夹在任何 Outlook 电子邮件客户端中都不可见，但是最终用户可以通过 Outlook 中或 Outlook 网页版上的**从服务器恢复已删除邮件**功能与其进行交互。 |
| 已计划 | 包含使用 Outlook for iOS 中的日程安排功能计划重新显示在收件箱中的邮件的文件夹。 |
| searchfolders | 在用户的邮箱中定义的所有搜索文件夹的父文件夹。 |
| sentitems | 已发送邮件文件夹。 |
| serverfailures | 包含存在于服务器上，但无法同步到本地客户端的项目的文件夹。 |
| syncissues | 包含由 Outlook 创建的同步日志的文件夹。 |

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-------|:------------|:------------|
|[获取 mailFolder](../api/mailfolder_get.md) | [mailFolder](mailfolder.md) |读取 mailFolder 对象的属性和关系。|
|[创建 MailFolder](../api/mailfolder_post_childfolders.md) |[MailFolder](mailfolder.md)| 通过发布到 childFolder 集合，在当前 mailFolder 下新建 mailFolder。|
|[列出 childFolder](../api/mailfolder_list_childfolders.md) |[MailFolder](mailfolder.md) 集合| 获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。|
|[创建邮件](../api/mailfolder_post_messages.md) |[邮件](message.md)| 通过发布到邮件集合，在当前 mailFolder 中新建邮件。|
|[列出邮件](../api/mailfolder_list_messages.md) |[邮件](message.md) 集合| 获取已登录用户邮箱中的所有邮件或邮箱的指定文件夹中的邮件。|
|[更新](../api/mailfolder_update.md) | [mailFolder](mailfolder.md)|更新指定的 mailFolder 对象。 |
|[删除](../api/mailfolder_delete.md) | 无 |删除指定的 mailFolder 对象。 |
|[复制](../api/mailfolder_copy.md)|[MailFolder](mailfolder.md)|将 mailfolder 及其内容复制到其他 mailfolder。|
|[delta](../api/mailfolder_delta.md)|[mailFolder](mailfolder.md) 集合|获取用户邮箱中已添加、删除或移除的邮件文件夹集。|
|[移动](../api/mailfolder_move.md)|[MailFolder](mailfolder.md)|将 mailFolder 及其内容移动到其他 mailFolder。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[mailFolder](mailFolder.md)  |在新建或现有的 mailFolder 中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的 mailFolder](../api/singlevaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | 通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 mailFolder。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [mailFolder](mailFolder.md) | 在新建或现有的 mailFolder 中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的 mailFolder](../api/multivaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | 使用 `$expand` 获取包含一个多值扩展属性的 mailFolder。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
|childFolderCount|Int32|当前 mailFolder 中的直接子 mailFolder 数量。|
|displayName|字符串|mailFolder 的显示名称。|
|ID|字符串|mailFolder 的唯一标识符。|
|parentFolderId|字符串|MailFolder 的父 mailFolder 的唯一标识符。|
|totalItemCount|Int32|邮箱中项的数量|
|unreadItemCount|Int32|mailFolder 中标记为未读的项的数量。|

**有效的访问项计数**

文件夹的 `TotalItemCount` 和 `UnreadItemCount` 属性允许您方便地计算文件夹中读取项目的数量。
它们让你避免像下面这样会引起严重延迟的查询：

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

Outlook 中的邮件文件夹可以包含多个类型的项，例如，收件箱可以包含不同于邮件项的会议请求项。 `TotalItemCount` 和 `UnreadItemCount` 会计入文件夹中的项目，而无论项目的类型如何。

## <a name="relationships"></a>关系

| 关系 | 类型 | 说明 |
|:-------------|:-----|:------------|
|childFolders|[MailFolder](mailfolder.md) 集合|mailFolder 中的子文件夹集合。|
|messageRules | [messageRule](messagerule.md) 集合 | 适用于用户“收件箱”文件夹的规则集合。 |
|消息|[邮件](message.md) 集合|mailFolder 中的邮件集合。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为 mailFolder 定义的多值扩展属性的集合。只读。可为 NULL。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合| 为 mailFolder 定义的单值扩展属性的集合。只读。可为 NULL。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mailFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "changeTracking": false,
        "navigability": "single",
        "searchable": false
      }
    },
    {
      "property": "messageRules",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single"
      }
    }
  ]
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a>另请参阅

- [使用增量查询跟踪 Microsoft Graph 数据更改](../../../concepts/delta_query_overview.md)
- [获取文件夹中邮件的增量更改](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
