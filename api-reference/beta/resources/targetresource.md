---
title: targetResource 资源类型
description: 指示与审核活动关联的目标资源类型的集合。 每个目标资源类型将继承此资源从下面概括的属性。
localization_priority: Normal
ms.openlocfilehash: f86cfe45870292dae93327859c32d38aa2b252fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828677"
---
# <a name="targetresource-resource-type"></a>targetResource 资源类型
指示与审核活动关联的目标资源类型的集合。 每个目标资源类型将继承此资源从下面概括的属性。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|字符串|指示下以下目标资源类型列出的资源的显示名称。|
|id|字符串|指示的资源的唯一 Id (例如： UserId，AppId，RoleId。)。|
|ModifiedProperties|[modifiedProperty](modifiedproperty.md)集合|指示名称、 旧值和更改每个属性的新值。 这仅适用于任何"更新"活动|

### <a name="target-resource-types"></a>目标资源类型

目标资源类型会有所不同，根据基础资源：

|资源名称| 参考|
|-------------|----------|
Device|[targetResourceDevice](targetresourcedevice.md)
目录|[targetResourceDirectory](targetresourcedirectory.md]
Group|[targetResourceGroup](targetresourcegroup.md)
策略|[targetResourcePolicy](targetresourcepolicy.md)
Role|[targetResourceRole](targetresourcerole.md)
服务主体|[targetResourceServicePrincipal](targetresourceserviceprincipal.md)
用户|[targetResourceUser](targetresourceuser.md)
其他|[targetResourceOther](targetresourceother.md)

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
