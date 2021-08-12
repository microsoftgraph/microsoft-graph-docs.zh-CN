---
title: licenseUnitsDetail 资源类型
description: '**subscribedSku** 实体的 prepaidUnits 属性为 **licenseUnitsDetail** 类型。'
localization_priority: Normal
author: 'michaelcurnutt '
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: af038eab4589fcaf98743b34cdc1ce6f43b09bd7b511d1f3a05862862155fa32
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54135062"
---
# <a name="licenseunitsdetail-resource-type"></a>licenseUnitsDetail 资源类型

命名空间：microsoft.graph

**subscribedSku** 实体的 [prepaidUnits](subscribedsku.md) 属性为 **licenseUnitsDetail** 类型。 有关订阅进度状态详细信息，请参阅如果我 [的订阅过期，如何？](/microsoft-365/commerce/subscriptions/what-if-my-subscription-expires?view=o365-worldwide)

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:-------------|:-----|:----------|
|已启用|Int32| 为服务 SKU 的活动订阅启用的单位数。  |
|已挂起|Int32| 由于服务 SKU 的订阅已取消而暂停的单位数。 无法分配单位，但仍可以在删除之前将其重新激活。 |
|警告|Int32| 警告状态的单位数。 当服务 SKU 订阅已过期时，客户有一个宽限期来续订其订阅，然后取消订阅 (移动到暂停状态) 。   |

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

