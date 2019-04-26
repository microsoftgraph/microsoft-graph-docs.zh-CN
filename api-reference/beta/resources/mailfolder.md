---
title: mailFolder 资源类型
description: 用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。 邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 294f2a9a6b4775ad30165352dec5520fb0efa804
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342754"
---
# <a name="mailfolder-resource-type"></a>mailFolder 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用户邮箱中的邮箱文件夹，例如收件箱和草稿箱。 邮箱文件夹可以包含邮件、其他 Outlook 项和子邮件文件夹。

该资源支持通过提供 [delta](../api/mailfolder-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

**众所周知的文件夹名称**

Outlook 默认情况下会为用户创建某些文件夹。 为方便起见, 您可以在访问这些文件夹时使用下表中已知的文件夹名称, 而不是使用相应的文件夹**id**值。 例如, 可以使用以下查询获取 "草稿" 文件夹, 并使用其已知名称。

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

无论用户邮箱的区域设置如何, 已知名称都有效, 因此上述查询将始终返回用户的 "草稿" 文件夹, 而不管它是如何命名的。

| 众所周知的文件夹名称 | 说明 |
|:-----------------------|:------------|
| 档案 | 将存档文件夹邮件发送到在支持它的 Outlook 客户端中使用 One_Click 存档功能时。 **注意:** 这与 Exchange online 的存档邮箱功能不同。 |
| 待 | 使用 "杂乱" 功能时, "筛选邮件" 文件夹的低优先级邮件将移至。 |
| 出现 | 邮箱中包含冲突项目的文件夹。 |
| conversationhistory | skype 保存 IM 对话的文件夹 (如果 skype 已配置为执行此操作)。 |
| DeletedItems | 文件夹项目被删除时移动到这些项目。 |
| 模 | 包含未发送邮件的文件夹。 |
| 收件箱 | "收件箱" 文件夹。 |
| junkemail | "垃圾邮件" 文件夹。 |
| localfailures | 包含本地客户端上存在但未能上载到服务器的项目的文件夹。 |
| msgfolderroot | "信息存储顶部" 文件夹。 此文件夹是在普通邮件客户端 (如 "收件箱") 中显示的文件夹的父文件夹。 |
| 件 | "发件箱" 文件夹。 |
| recoverableitemsdeletions | 包含软删除项目的文件夹: 从 "已删除邮件" 文件夹中删除, 或在 Outlook 中按 shift + delete。 此文件夹在任何 Outlook 电子邮件客户端中都不可见, 但最终用户可以通过 outlook 或 web 上的 outlook 中的 "**从服务器恢复已删除邮件**" 功能与它进行交互。 |
| 已计划 | 包含已计划在收件箱中使用 Outlook for iOS 中的 "日程安排" 功能重新显示的邮件的文件夹。 |
| searchfolders | 用户邮箱中定义的所有搜索文件夹的父文件夹。 |
| 已发送邮件 | "已发送邮件" 文件夹。 |
| serverfailures | 包含服务器上存在但未能同步到本地客户端的项目的文件夹。 |
| syncissues | 包含由 Outlook 创建的同步日志的文件夹。 |

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:-------|:------------|:------------|
|[获取 mailFolder](../api/mailfolder-get.md) | [mailFolder](mailfolder.md) |读取 mailFolder 对象的属性和关系。|
|[创建 MailFolder](../api/mailfolder-post-childfolders.md) |[mailFolder](mailfolder.md)| 通过发布到 childFolder 集合，在当前 mailFolder 下新建 mailFolder。|
|[列出 childFolder](../api/mailfolder-list-childfolders.md) |[mailFolder](mailfolder.md) 集合| 获取指定文件夹下的文件夹集合。你可以使用 `.../me/MailFolders` 快捷方式获取顶级文件夹集合并导航到其他文件夹。|
|[创建邮件](../api/mailfolder-post-messages.md) |[邮件](message.md)| 通过发布到邮件集合，在当前 mailFolder 中新建邮件。|
|[列出邮件](../api/mailfolder-list-messages.md) |[邮件](message.md)集合| 获取已登录用户邮箱中的所有邮件或邮箱的指定文件夹中的邮件。|
|[更新](../api/mailfolder-update.md) | [mailFolder](mailfolder.md)|更新指定的 mailFolder 对象。 |
|[删除](../api/mailfolder-delete.md) | 无 |删除指定的 mailFolder 对象。 |
|[复制](../api/mailfolder-copy.md)|[mailFolder](mailfolder.md)|将 mailfolder 及其内容复制到其他 mailfolder。|
|[delta](../api/mailfolder-delta.md)|[mailFolder](mailfolder.md) 集合|获取用户邮箱中已添加、删除或移除的邮件文件夹集。|
|[移动](../api/mailfolder-move.md)|[mailFolder](mailfolder.md)|将 mailFolder 及其内容移动到其他 mailFolder。|
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
|wellKnownName|String|文件夹的已知文件夹名称。 上面列出了可能的值。 此属性仅为 Outlook 创建的默认文件夹设置。 对于其他文件夹, 此属性为**null**。|

**有效的访问项计数**

通过`TotalItemCount`文件夹`UnreadItemCount`的和属性, 可以方便地计算文件夹中的已读项目数。
使你避免进行可产生重大延迟的查询，如下所示：

```http
https://outlook.office.com/api/beta/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

Outlook 中的邮件文件夹可以包含多种类型的项目, 例如, 收件箱可以包含与邮件项目不同的会议请求项目。 `TotalItemCount`并`UnreadItemCount`在邮件文件夹中包含项目, 而不考虑其项目类型。

## <a name="relationships"></a>关系

| 关系 | 类型 | 说明 |
|:-------------|:-----|:------------|
|childFolders|[MailFolder](mailfolder.md) 集合|mailFolder 中的子文件夹集合。|
|messageRules | [messageRule](messagerule.md) 集合 | 适用于用户“收件箱”文件夹的规则集合。 |
|messages|[Message](message.md) collection|mailFolder 中的邮件集合。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为 mailFolder 定义的多值扩展属性的集合。只读。可为 NULL。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为 mailFolder 定义的单值扩展属性的集合。只读。可为 NULL。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
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
  "unreadItemCount": 1024,
  "wellKnownName": "string",
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
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
