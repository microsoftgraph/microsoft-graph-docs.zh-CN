---
title: sharingDetail 资源类型
description: '包含共享项的属性的复杂类型。 '
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 96840e801e7789c287dad26e014797013039a6a5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094287"
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
| sharedDateTime        | DateTimeOffset| 上次共享文件的日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。  |
| sharingSubject        | String          | 与文档共享的主题。 |
| sharingType             | String        | 确定文档的共享方式，可通过"Link"、"Attachment"、"Group"、"Site"来表示。     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | 共享文档的用户。  |
| sharingReference        | [resourceReference](insights-resourcereference.md)      |  |

