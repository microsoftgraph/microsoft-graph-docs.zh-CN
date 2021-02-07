---
title: mailSearchFolder 资源类型
description: mailSearchFolder 是用户邮箱中的虚拟文件夹，其中包含符合指定搜索条件的所有电子邮件项目。 mailSearchFolder 继承自 mailFolder。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9e153999cfa647b2f8f13e350b3193b358b536cf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129707"
---
# <a name="mailsearchfolder-resource-type"></a>mailSearchFolder 资源类型

命名空间：microsoft.graph

**mailSearchFolder** 是用户邮箱中的虚拟文件夹，其中包含符合指定搜索条件的所有电子邮件项目。 **mailSearchFolder** 继承自 [mailFolder](mailfolder.md)。 可以在用户的 Exchange Online 邮箱的任何文件夹中创建搜索文件夹。 但是，若要在 Outlook、Outlook 网页或 Outlook Live 中显示搜索文件夹，必须在 **WellKnownFolderName.SearchFolders** 文件夹中创建该文件夹。 

## <a name="search-folder-lifecycle"></a>搜索文件夹生命周期

Exchange Online 可以删除由应用程序创建的搜索文件夹，原因如下：

1.  搜索文件夹在 45 天未使用后过期。 
2.  每个源文件夹可创建的搜索文件夹数量有一些限制。 如果超过此限制，将删除较旧的搜索文件夹，为新的搜索文件夹提供途径。 

删除搜索文件夹后，应用应创建新的搜索文件夹资源，并使用相同的资源。


## <a name="methods"></a>Methods

| 方法 | 返回类型  | 说明 |
|:---------------|:--------|:----------|
| [创建搜索文件夹](../api/mailsearchfolder-post.md) | [mailSearchFolder](mailsearchfolder.md) | 在此用户的邮箱中创建搜索文件夹。 |
| [列出搜索文件夹](../api/mailfolder-list-childfolders.md) | [mailFolder](mailfolder.md) 集合 | 列出此用户邮箱中所有文件夹，包括搜索文件夹。 |
| [获取搜索文件夹](../api/mailfolder-get.md) | [mailSearchFolder](mailsearchfolder.md) | 获取指定的搜索文件夹。 |
| [更新搜索文件夹](../api/mailsearchfolder-update.md) | [mailSearchFolder](mailsearchfolder.md) | 更新指定的搜索文件夹。 |
| [删除搜索文件夹](../api/mailfolder-delete.md) | 无 | 删除指定的搜索文件夹。 |
| [列出搜索文件夹中的所有邮件](../api/mailfolder-list-messages.md) | [邮件](message.md)集合 | 列出指定搜索文件夹中的所有邮件。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| isSupported | 布尔 | 指示搜索文件夹是否可以使用 REST API 进行编辑。 |
| includeNestedFolders | 布尔 | 指示如何在搜索中遍历邮箱文件夹层次结构。 `true` 意味着应执行深入搜索，以在 **sourceFolderIds** 中显式指定的每个文件夹的层次结构中包括子文件夹。 `false` 表示仅对 **sourceFolderIds** 中显式指定的每个文件夹进行浅表搜索。 |
| sourceFolderIds | String collection | 应缩小的邮箱文件夹。 |
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

