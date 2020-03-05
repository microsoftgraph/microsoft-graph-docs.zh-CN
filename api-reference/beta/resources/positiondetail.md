---
title: positionDetail 资源类型
description: positionDetail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6c77c116f013000ec4d419ec20c1e45c07187a22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521591"
---
# <a name="positiondetail-resource-type"></a>positionDetail 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关与用户[配置文件](profile.md)中的实体相关的位置的信息。

## <a name="properties"></a>属性

| 属性       | 类型                             | 说明                                            |
|:---------------|:---------------------------------|:-------------------------------------------------------|
|公司         |[companyDetail](companydetail.md) | 有关公司或雇主的详细信息。                  |
|说明     |String                            | 相关职位的描述。               |
|endMonthYear    |日期                              | 位置结束时。                               |
|jobTitle        |String                            | 在该位置保留的标题。                  |
|role            |String                            | 位置 entailed 的角色。                        |
|startMonthYear  |日期                              | 开始月份和位置的年。              |
|摘要         |String                            |职位的简短摘要。                          |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.positionDetail",
  "baseType": null
}-->

```json
{
  "company": {"@odata.type": "microsoft.graph.companyDetail"},
  "description": "String",
  "endMonthYear": "String (timestamp)",
  "jobTitle": "String",
  "role": "String",
  "startMonthYear": "String (timestamp)",
  "summary": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "positionDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->