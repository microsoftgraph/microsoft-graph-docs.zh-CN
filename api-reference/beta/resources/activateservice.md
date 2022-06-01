---
title: activateService 资源类型
description: 表示要激活的服务。
author: dkershaw10
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5f6c54c79010e08f0e44d2202141decb69c2036c
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820271"
---
# <a name="activateservice-resource-type-deprecated"></a>activateService 资源类型 (已弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示要激活的服务。

## <a name="properties"></a>属性

| 属性         | 类型         | 说明                           |
| ----------------- | ------------ | ------------------------------------- |
| service| String | 要激活的服务的名称。 |
| servicePlanId | Guid | 要激活的服务计划的计划标识符。 |
| skuId | Guid | 服务计划的 SKU 标识符。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activateService"
}-->

```json
{
    "service": "String",
    "skuId": "Guid",
    "servicePlanId": "Guid"
}

```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "activateService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
