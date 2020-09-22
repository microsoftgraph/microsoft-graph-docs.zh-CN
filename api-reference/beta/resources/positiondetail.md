---
title: positionDetail 资源类型
description: positionDetail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: fbd013292754dea43dd69b645dcd2ab735559b69
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971480"
---
# <a name="positiondetail-resource-type"></a>positionDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关与用户 [配置文件](profile.md)中的实体相关的位置的信息。

## <a name="properties"></a>属性

| 属性       | 类型                             | 说明                                            |
|:---------------|:---------------------------------|:-------------------------------------------------------|
|公司         |[companyDetail](companydetail.md) | 有关公司或雇主的详细信息。                  |
|description     |String                            | 相关职位的描述。               |
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

