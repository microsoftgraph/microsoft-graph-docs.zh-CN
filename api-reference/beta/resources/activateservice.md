---
title: activateService 资源类型
description: 表示要激活的服务。
author: dkershaw10
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a1ab2112406d0049df002327be784c46b7e879e6
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109082"
---
# <a name="activateservice-resource-type"></a>activateService 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示要激活的服务。

## <a name="properties"></a>属性

| 属性         | 类型         | 说明                           |
| ----------------- | ------------ | ------------------------------------- |
| service| String | 要激活的服务的名称。 |
| servicePlanId | GUID | 要激活的服务计划的计划标识符。 |
| skuId | GUID | 服务计划的 SKU 标识符。 |

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
    "service": "string",
    "skuId": "guid",
    "servicePlanId": "guid"
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
