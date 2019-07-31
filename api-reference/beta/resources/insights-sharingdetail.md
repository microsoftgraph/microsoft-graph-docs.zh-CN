---
title: sharingDetail 资源类型
description: '包含共享项目的属性的复杂类型。 '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c62fc11c668a5175e0dafa9bdf4c937fecbef798
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005714"
---
# <a name="sharingdetail-resource-type"></a>sharingDetail 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含[共享](insights-shared.md)项目的属性的复杂类型。 

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
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a>属性

| 属性              | 类型          | 说明  |
| -------------         |-----------    | -------------|
| sharedDateTime        | DateTimeOffset| 上次共享文件的日期和时间。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。 只读。  |
| sharingSubject        | String          | 共享文档的主题。 |
| sharingType             | String        | 确定文档的共享方式, 可以是 "链接"、"附件"、"组"、"网站"。     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | 共享文档的用户。  |
| sharingReference        | [resourceReference](insights-resourcereference.md)      |  |
