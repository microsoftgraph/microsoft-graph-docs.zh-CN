---
title: licenseUnitsDetail 资源类型
description: '**subscribedSku** 实体的 prepaidUnits 属性为 **licenseUnitsDetail** 类型。'
ms.localizationpriority: medium
author: jconley76
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6a321eeb77b011730ec99b76112bd441862e72d2
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900399"
---
# <a name="licenseunitsdetail-resource-type"></a>licenseUnitsDetail 资源类型

命名空间：microsoft.graph

**subscribedSku** 实体的 [prepaidUnits](subscribedsku.md) 属性为 **licenseUnitsDetail** 类型。 有关订阅的进度状态的详细信息， [请参阅我的订阅是否过期？](/microsoft-365/commerce/subscriptions/what-if-my-subscription-expires?view=o365-worldwide&preserve-view=true)

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:-------------|:-----|:----------|
|已启用|Int32| 为服务 SKU 的活动订阅启用的单位数。  |
|已挂起|Int32| 因服务 SKU 订阅已取消而暂停的单位数。 无法分配这些单元，但仍可在删除之前重新激活。 |
|警告|Int32| 处于警告状态的单位数。 服务 SKU 的订阅已过期时，客户有一个宽限期来续订其订阅，然后才将其取消 (移动到 **暂停** 状态) 。  |

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

