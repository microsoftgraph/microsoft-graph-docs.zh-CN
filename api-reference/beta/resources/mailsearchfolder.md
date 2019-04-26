---
title: mailSearchFolder 资源类型
description: mailSearchFolder 是用户邮箱中的虚拟文件夹, 其中包含与指定的搜索条件匹配的所有电子邮件项目。 mailSearchFolder 继承自 mailFolder。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ba76029b69d91be39c9d63ca755e8a4603aec0b9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562591"
---
# <a name="mailsearchfolder-resource-type"></a>mailSearchFolder 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

mailSearchFolder 是用户邮箱中的虚拟文件夹, 其中包含与指定的搜索条件匹配的所有电子邮件项目。 mailSearchFolder 继承自[mailFolder](mailfolder.md)。

## <a name="methods"></a>方法

| 方法 | 返回类型  | 说明 |
|:---------------|:--------|:----------|
| [创建搜索文件夹](../api/mailsearchfolder-post.md) | [mailSearchFolder](mailsearchfolder.md) | 在此用户的邮箱中创建 "搜索文件夹"。 |
| [列出搜索文件夹](../api/mailfolder-list-childfolders.md) | [mailFolder](mailfolder.md) 集合 | 列出此用户的邮箱中的所有文件夹, 包括 "搜索文件夹"。 |
| [获取搜索文件夹](../api/mailfolder-get.md) | [mailSearchFolder](mailsearchfolder.md) | 获取指定的搜索文件夹。 |
| [更新搜索文件夹](../api/mailsearchfolder-update.md) | [mailSearchFolder](mailsearchfolder.md) | 更新指定的搜索文件夹。 |
| [删除搜索文件夹](../api/mailfolder-delete.md) | 无 | 删除指定的搜索文件夹。 |
| [列出搜索文件夹中的所有邮件](../api/mailfolder-list-messages.md) | [邮件](message.md)集合 | 列出指定的搜索文件夹中的所有邮件。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| isSupported | Boolean | 指示是否可使用 REST api 编辑搜索文件夹。 |
| includeNestedFolders | Boolean | 指示应如何遍历邮箱文件夹层次结构。 `true`表示应执行深入搜索, 而不是`false`指应改为进行浅表搜索。 |
| sourceFolderIDs | String collection | 应挖掘的邮箱文件夹。 |
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
  "sourceFolderIDs": ["string"],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/mailsearchfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
