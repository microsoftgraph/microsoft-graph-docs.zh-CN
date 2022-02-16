---
title: activateService 资源类型
description: 表示要激活的服务。
author: dkershaw10
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d007512113ab46b25714942f93002936c97fe083
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854548"
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
    "service": "String",
    "skuId": "GUID",
    "servicePlanId": "GUID"
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
