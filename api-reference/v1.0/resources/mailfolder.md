---
title: mailFolder 资源类型
description: 用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。 邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。
localization_priority: Priority
ms.openlocfilehash: 32af125f57e02394c4d01913aaf783df11809242
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888156"
---
# <a name="mailfolder-resource-type"></a>mailFolder 资源类型

用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。 邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。

该资源支持通过提供 [delta](../api/mailfolder-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

**已知文件夹名称**

Outlook 默认情况下会为用户创建某些文件夹。 访问这些文件夹时，而不是使用的相应文件夹**id**值，为方便起见，您可以使用下表中的已知文件夹名称。 例如，您可以获取其已知名称使用以下查询草稿文件夹。

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

已知名称工作无论用户的邮箱的区域设置上述查询将始终返回命名方式无论用户的草稿文件夹。

| 已知文件夹名称 | Description |
|:-----------------------|:------------|
| 存档 | 存档文件夹邮件发送到在支持的 Outlook 客户端使用 One_Click 存档功能时。 **注意：** 这是不相同的存档邮箱功能的 Exchange online。 |
| 混乱 | 混乱文件夹低优先级邮件移动到时使用的混乱功能。 |
| 冲突 | 包含邮箱中的冲突项目的文件夹。 |
| conversationhistory | 其中 Skype 保存 IM 对话 （如果 Skype 配置这样） 中的文件夹。 |
| DeletedItems | 文件夹项目移到时被删除。 |
| 草稿 | 包含未发送的邮件的文件夹。 |
| 收件箱 | 收件箱文件夹中。 |
| junkemail | 垃圾邮件文件夹中。 |
| localfailures | 包含本地客户端上存在，但无法上载到服务器的项目的文件夹。 |
| msgfolderroot | "顶部的信息存储"文件夹中。 此文件夹的父文件夹的普通邮件客户端，如收件箱中显示的文件夹。 |
| 发件箱 | 发件箱文件夹中。 |
| recoverableitemsdeletions | 包含软删除项目的文件夹： 删除从已删除邮件文件夹中，或通过按 shift + delete 在 Outlook 中。 此文件夹不可见在任何 Outlook 电子邮件客户端，但是与其进行交互的最终用户可以通过中 Outlook 或 Outlook web 上的**从服务器恢复已删除邮件**功能。 |
| 已计划 | 包含计划重新显示在适用于 iOS 的 Outlook 中使用的日程安排功能收件箱中的邮件文件夹。 |
| searchfolders | 在用户的邮箱中定义的所有搜索文件夹的父文件夹。 |
| sentitems | 已发送的邮件文件夹中。 |
| serverfailures | 包含服务器上存在，但无法同步到本地客户端的项目的文件夹。 |
| syncissues | 包含由 Outlook 创建的同步日志的文件夹。 |

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-------|:------------|:------------|
|[获取 mailFolder](../api/mailfolder-get.md) | [mailFolder](mailfolder.md) |读取 mailFolder 对象的属性和关系。|
|[创建 MailFolder](../api/mailfolder-post-childfolders.md) |[MailFolder](mailfolder.md)| 通过发布到 childFolder 集合，在当前 mailFolder 下新建 mailFolder。|
|[列出 childFolder](../api/mailfolder-list-childfolders.md) |[MailFolder](mailfolder.md) 集合| 获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。|
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
|id|字符串|MailFolder 的唯一标识符。|
|parentFolderId|String|MailFolder 的父 mailFolder 的唯一标识符。|
|totalItemCount|Int32|邮箱中项的数量|
|unreadItemCount|Int32|mailFolder 中标记为未读的项的数量。|

**有效的访问项计数**

`TotalItemCount`和`UnreadItemCount`文件夹的属性，可以方便地计算的文件夹中的读取项目数。
它们使您可以避免查询会引发大量延迟如下：

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

在 Outlook 中的邮件文件夹可以包含多个类型的项目，例如，可以包含收件箱会议请求项目的不同邮件项目。 `TotalItemCount`和`UnreadItemCount`包括而不考虑其项目类型的邮件文件夹中的项目。

## <a name="relationships"></a>Relationships

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
