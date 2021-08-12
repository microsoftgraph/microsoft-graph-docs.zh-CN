---
title: mailFolder 资源类型
description: 用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。 邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a65a5a88e2c0951c9b292140ca6a071b788651c8a0dcbebbb22eab5205407b64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169436"
---
# <a name="mailfolder-resource-type"></a>mailFolder 资源类型

命名空间：microsoft.graph

用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。 邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。

该资源支持通过提供 [delta](../api/mailfolder-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

**已知文件夹名称**

Outlook 默认情况下会为用户创建某些文件夹。 为方便起见，可以在访问这些文件夹时使用已知的文件夹名称来替代使用相应的文件夹 **id** 值。 例如，你可以使用其已知名称和以下查询来获取“草稿”文件夹。

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

无论用户邮箱的区域设置如何，已知名称都可以工作，因此无论命名方式如何，上述查询都将始终返回用户的“草稿”文件夹。

| 已知文件夹名称 | 说明 |
|:-----------------------|:------------|
| archive | 在支持它的 Outlook 客户端中使用 One_Click 存档功能时，将发送存档文件夹邮件。 **注意：** 这与 Exchange Online 的存档邮箱功能并不相同。 |
| clutter | 使用待筛选邮件功能时，待筛选文件夹低优先级邮件将被移动到这里。 |
| conflicts | 包含邮箱中冲突项的文件夹。 |
| conversationhistory | Skype 保存 IM 对话的文件夹（如果 Skype 配置为这样做）。 |
| deleteditems | 文件夹项被删除时，将被移动到这里。 |
| drafts | 包含未发送邮件的文件夹。 |
| inbox | 收件箱文件夹。 |
| junkemail | “垃圾邮件”文件夹。 |
| localfailures | 包含本地客户端上存在但无法上载到服务器的项的文件夹。 |
| msgfolderroot | “最上层的信息存储”文件夹。此文件夹是邮件客户端（如收件箱）中显示的文件夹的父文件夹。 |
| outbox | “发件箱”文件夹。 |
| recoverableitemsdeletions | 包含软删除项的文件夹：从“已删除邮件”文件夹中删除，或者在 Outlook 中按 shift+delete 删除。 此文件夹在任何 Outlook 电子邮件客户端中都不可见，但最终用户可以通过 Outlook 中的“**从服务器恢复已删除邮件**”功能或 Web 上的 Outlook 与其进行交互。 |
| scheduled | 包含计划使用 Outlook for iOS 中的“计划”功能重新出现在收件箱中的邮件的文件夹。 |
| searchfolders | 用户邮箱中定义的所有搜索文件夹的父文件夹。 |
| sentitems | 已发送项的文件夹。 |
| serverfailures | 包含服务器上存在但无法同步到本地客户端的项的文件夹。 |
| syncissues | 包含 Outlook 创建的同步日志的文件夹。 |

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-------|:------------|:------------|
|[List mailFolders](../api/user-list-mailfolders.md) | [mailFolder](mailfolder.md) 集合|获取指定用户的邮箱内的所有邮件文件夹，包括所有邮件搜索文件夹。|
|[获取 mailFolder](../api/mailfolder-get.md) | [mailFolder](mailfolder.md) |读取 mailFolder 对象的属性和关系。|
|[Create mailFolder](../api/user-post-mailfolders.md) |[mailFolder](mailfolder.md)| 在用户邮箱的根文件夹中新建邮件文件夹。|
|[列出 childFolder](../api/mailfolder-list-childfolders.md) |[MailFolder](mailfolder.md) 集合| 获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。|
|[创建 childFolder](../api/mailfolder-post-childfolders.md) |[mailFolder](mailfolder.md)| 通过发布到 childFolder 集合，在当前 mailFolder 下新建 mailFolder。|
|[创建邮件](../api/mailfolder-post-messages.md) |[邮件](message.md)| 通过发布到邮件集合，在当前 mailFolder 中新建邮件。|
|[列出邮件](../api/mailfolder-list-messages.md) |[邮件](message.md) 集合| 获取已登录用户邮箱中的所有邮件或邮箱的指定文件夹中的邮件。|
|[更新](../api/mailfolder-update.md) | [mailFolder](mailfolder.md)|更新指定的 mailFolder 对象。 |
|[删除](../api/mailfolder-delete.md) | 无 |删除指定的 mailFolder 对象。 |
|[复制](../api/mailfolder-copy.md)|[MailFolder](mailfolder.md)|将 mailfolder 及其内容复制到其他 mailfolder。|
|[delta](../api/mailfolder-delta.md)|[mailFolder](mailfolder.md) 集合|获取用户邮箱中已添加、删除或移除的邮件文件夹集。|
|[移动](../api/mailfolder-move.md)|[MailFolder](mailfolder.md)|将 mailFolder 及其内容移动到其他 mailFolder。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[mailFolder](mailfolder.md)  |在新建或现有的 mailFolder 中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的 mailFolder](../api/singlevaluelegacyextendedproperty-get.md)  | [mailFolder](mailfolder.md) | 通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的 mailFolder。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [mailFolder](mailfolder.md) | 在新建或现有的 mailFolder 中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的 mailFolder](../api/multivaluelegacyextendedproperty-get.md)  | [mailFolder](mailfolder.md) | 使用 `$expand` 获取包含一个多值扩展属性的 mailFolder。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
|childFolderCount|Int32|当前 mailFolder 中的直接子 mailFolder 数量。|
|displayName|String|mailFolder 的显示名称。|
|id|String|MailFolder 的唯一标识符。|
|IsHidden|布尔值|指示 mailFolder 是否处于隐藏状态。 此属性只能在创建文件夹时设置。 请在[隐藏的邮件文件夹](#hidden-mail-folders)中获取更多信息。|
|parentFolderId|String|MailFolder 的父 mailFolder 的唯一标识符。|
|totalItemCount|Int32|邮箱中项的数量|
|unreadItemCount|Int32|mailFolder 中标记为未读的项的数量。|

**有效的访问项计数**

使用文件夹的 `TotalItemCount` 和 `UnreadItemCount` 的属性可以方便地计算在文件夹中读取的项数。
使你避免进行可产生重大延迟的查询，如下所示：

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

Outlook 中的邮件文件夹可包含多个类型的项，例如，收件箱可以包含不同于邮件项的会议请求项。 `TotalItemCount` 和 `UnreadItemCount`包括邮件文件夹中的项，无论其项类型如何。

### <a name="hidden-mail-folders"></a>隐藏的邮件文件夹
`isHidden` 属性的默认值为 `false`。 仅当 [创建 mailFolder](../api/user-post-mailfolders.md)时可以设置 **isHidden**。 不可使用“修补”操作更新属性。 若要更改 **isHidden** 属性，请删除现有文件夹，然后使用希望的值，新建一个文件夹。

隐藏邮件文件夹支持常规邮件文件夹支持的所有操作。

默认情况下，[邮件文件夹列表](../api/user-list-mailfolders.md)仅返回未隐藏的邮件文件夹。 若要在答复中包括隐藏的邮件文件夹，请使用查询参数 `includeHiddenFolders=true`。 然后使用 **isHidden** 属性来识别邮件文件夹是否处于隐藏状态。 

## <a name="relationships"></a>关系

| 关系 | 类型 | 说明 |
|:-------------|:-----|:------------|
|childFolders|[MailFolder](mailfolder.md) 集合|mailFolder 中的子文件夹集合。|
|messageRules | [messageRule](messagerule.md) 集合 | 适用于用户“收件箱”文件夹的规则集合。 |
|messages|[邮件](message.md) 集合|mailFolder 中的邮件集合。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为 mailFolder 定义的多值扩展属性的集合。只读。可为 NULL。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为 mailFolder 定义的单值扩展属性的集合。只读。可为 NULL。|

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
  "isHidden": false,
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a>另请参阅

- [使用增量查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)
- [获取文件夹中邮件的增量更改](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

