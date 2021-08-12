---
title: sharingDetail 资源类型
description: '包含共享项的属性的复杂类型。 '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 341bef801b8ee8a7cfc8b5176f4984251209db9e4aff05de9d983b8e06cb61fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124463"
---
# <a name="sharingdetail-resource-type"></a>sharingDetail 资源类型

命名空间：microsoft.graph

包含 [sharedInsight 项的属性的复杂](insights-shared.md) 类型。 

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingDetail"
}-->
```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "sharingReference": "resourceReference"
}
```

## <a name="properties"></a>属性

| 属性              | 类型          | 说明  |
| -------------         |-----------    | -------------|
| sharedDateTime        | DateTimeOffset| 上次共享文件的日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。 只读。  |
| sharingSubject        | String          | 与文档共享的主题。 |
| sharingType             | String        | 确定文档的共享方式，可通过"Link"、"Attachment"、"Group"、"Site"来表示。     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | 共享文档的用户。  |
| sharingReference        | [resourceReference](insights-resourcereference.md)      |  |

