---
title: employeeOrgData 资源类型
description: 表示与用户相关联的组织数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: cmmdesai
ms.openlocfilehash: f8a8ba6add4a68ffa0759346d97cfebbb4199f1c
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635620"
---
# <a name="employeeorgdata-resource-type"></a>employeeOrgData 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与用户相关联的组织数据。 [User](user.md)实体的**employeeOrgData**属性是一个组织属性的集合。

## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
| division | String | 用户工作的部门的名称。 <br><br>仅在 `$select` 上返回。 支持 `$filter`。 |
| costCenter | String | 与用户关联的成本中心。 <br><br>仅在 `$select` 上返回。 支持 `$filter`。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.employeeOrgData"
}-->

```json
{
  "costCenter": "string",
  "division": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-10-24 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "employeeOrgData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
