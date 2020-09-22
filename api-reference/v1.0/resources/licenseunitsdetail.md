---
title: licenseUnitsDetail 资源类型
description: '**subscribedSku** 实体的 prepaidUnits 属性为 **licenseUnitsDetail** 类型。'
localization_priority: Normal
author: krbain
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: af761aea94f21d3543bcaa8032d4120e3d1ad502
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048328"
---
# <a name="licenseunitsdetail-resource-type"></a>licenseUnitsDetail 资源类型

命名空间：microsoft.graph

**subscribedSku** 实体的 [prepaidUnits](subscribedsku.md) 属性为 **licenseUnitsDetail** 类型。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:-------------|:-----|:----------|
|已启用|Int32| 启用的单位数。 |
|已挂起|Int32| 挂起的单位数。 |
|警告|Int32| 处于警告状态的单位数。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

