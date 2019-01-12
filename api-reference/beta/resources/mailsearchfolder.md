---
title: mailSearchFolder 资源类型
description: MailSearchFolder 是虚拟文件夹中包含与指定的搜索条件匹配的所有电子邮件项目的用户的邮箱。 mailSearchFolder 继承 mailFolder。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1ba9ce248071e3d806383b4cd7e7550c1e3aa145
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920910"
---
# <a name="mailsearchfolder-resource-type"></a>mailSearchFolder 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

MailSearchFolder 是虚拟文件夹中包含与指定的搜索条件匹配的所有电子邮件项目的用户的邮箱。 mailSearchFolder 继承[mailFolder](mailfolder.md)。

## <a name="methods"></a>方法

| 方法 | 返回类型  | 说明 |
|:---------------|:--------|:----------|
| [创建搜索文件夹](../api/mailsearchfolder-post.md) | [mailSearchFolder](mailsearchfolder.md) | 此用户的邮箱中创建搜索文件夹。 |
| [列表搜索文件夹](../api/mailfolder-list-childfolders.md) | [mailFolder](mailfolder.md) 集合 | 列出该用户的邮箱，包括搜索文件夹中的所有文件夹。 |
| [获取搜索文件夹](../api/mailfolder-get.md) | [mailSearchFolder](mailsearchfolder.md) | 获取指定的搜索文件夹。 |
| [更新搜索文件夹](../api/mailsearchfolder-update.md) | [mailSearchFolder](mailsearchfolder.md) | 更新指定的搜索文件夹。 |
| [删除搜索文件夹](../api/mailfolder-delete.md) | 无 | 删除指定的搜索文件夹。 |
| [列表中搜索文件夹的所有邮件](../api/mailfolder-list-messages.md) | [邮件](message.md)集合 | 列表中指定的搜索文件夹的所有邮件。 |

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| isSupported | 布尔 | 指示搜索文件夹是否可编辑使用 REST Api。 |
| includeNestedFolders | 布尔 | 指示应如何遍历的邮箱文件夹层次结构。 `true`意味着应为深入搜索完成时`false`意味着浅表搜索应改为完成。 |
| sourceFolderIDs | String 集合 | 应 mined 邮箱文件夹。 |
| filterQuery | 字符串 | 要筛选的邮件的 OData 查询。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
