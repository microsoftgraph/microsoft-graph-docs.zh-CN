---
title: mailSearchFolder 资源类型
description: MailSearchFolder 是用户邮箱中的虚拟文件夹，其中包含与指定的搜索条件匹配的所有电子邮件项目。 mailSearchFolder 继承自 mailFolder。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: eb2ff38cc2089c143e98f8297177341685879635
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447491"
---
# <a name="mailsearchfolder-resource-type"></a>mailSearchFolder 资源类型

命名空间： microsoft. graph

**MailSearchFolder**是用户邮箱中的虚拟文件夹，其中包含与指定的搜索条件匹配的所有电子邮件项目。 **mailSearchFolder**继承自[mailFolder](mailfolder.md)。 可以在用户的 Exchange Online 邮箱中的任何文件夹中创建搜索文件夹。 但是，在 Outlook 中显示的搜索文件夹、Outlook for web 或 Outlook Live 中，必须在**WellKnownFolderName**文件夹中创建该文件夹。 

## <a name="search-folder-lifecycle"></a>搜索文件夹生命周期

由于以下原因之一，Exchange Online 可以删除你的应用程序创建的搜索文件夹：

1.  搜索文件夹在45天后过期（不使用）。 
2.  可以为每个源文件夹创建的搜索文件夹的数量存在限制。 当此限制被突破时，将删除较旧的搜索文件夹，以便为新的搜索文件夹。 

删除搜索文件夹时，您的应用程序应创建一个新的 "搜索文件夹" 资源并使用相同的。


## <a name="methods"></a>方法

| 方法 | 返回类型  | 说明 |
|:---------------|:--------|:----------|
| [创建搜索文件夹](../api/mailsearchfolder-post.md) | [mailSearchFolder](mailsearchfolder.md) | 在此用户的邮箱中创建 "搜索文件夹"。 |
| [列出搜索文件夹](../api/mailfolder-list-childfolders.md) | [mailFolder](mailfolder.md) 集合 | 列出此用户的邮箱中的所有文件夹，包括 "搜索文件夹"。 |
| [获取搜索文件夹](../api/mailfolder-get.md) | [mailSearchFolder](mailsearchfolder.md) | 获取指定的搜索文件夹。 |
| [更新搜索文件夹](../api/mailsearchfolder-update.md) | [mailSearchFolder](mailsearchfolder.md) | 更新指定的搜索文件夹。 |
| [删除搜索文件夹](../api/mailfolder-delete.md) | 无 | 删除指定的搜索文件夹。 |
| [列出搜索文件夹中的所有邮件](../api/mailfolder-list-messages.md) | [message](message.md) 集合 | 列出指定的搜索文件夹中的所有邮件。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| isSupported | 布尔 | 指示是否可使用 REST Api 编辑搜索文件夹。 |
| includeNestedFolders | 布尔 | 指示应如何在搜索中遍历邮箱文件夹层次结构。 `true`表示应执行深入搜索以在**sourceFolderIds**中显式指定的每个文件夹的层次结构中包含子文件夹。 `false`表示仅对**sourceFolderIds**中显式指定的每个文件夹进行浅表搜索。 |
| sourceFolderIds | String 集合 | 应挖掘的邮箱文件夹。 |
| filterQuery | String | 用于筛选邮件的 OData 查询。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailSearchFolder"
}-->

```json
{
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": ["string"],
  "filterQuery": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2018-01-23 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
