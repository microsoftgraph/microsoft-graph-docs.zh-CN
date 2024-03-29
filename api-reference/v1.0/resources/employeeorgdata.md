---
title: employeeOrgData 资源类型
description: 表示与用户关联的组织数据。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: cmmdesai
ms.openlocfilehash: 8a0ee00ed1165eddd69a212419292a7690514238
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123606"
---
# <a name="employeeorgdata-resource-type"></a>employeeOrgData 资源类型

命名空间：microsoft.graph

表示与用户关联的组织数据。 user 实体的 **employeeOrgData** 属性是组织属性的集合。 [](user.md)

## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
| division | String | 用户工作部门的名称。 <br><br>仅在 `$select` 上返回。 支持 `$filter`。 |
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
