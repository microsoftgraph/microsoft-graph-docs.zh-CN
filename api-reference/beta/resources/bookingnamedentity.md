---
title: bookingNamedEntity 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 5c219d0ab879c1bc1ae172d08322647b2c261497
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507987"
---
# <a name="bookingnamedentity-resource-type"></a>bookingNamedEntity 资源类型

命名空间： microsoft. graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
这是 Microsoft 预订实体的基本类型，可提供显示名称，例如， [bookingBusiness](bookingbusiness.md)、 [bookingPerson](bookingperson.md)、 [bookingService](bookingservice.md)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|String|派生实体的名称，与客户进行交互。|
|id|String| 派生实体的 ID。 只读。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingNamedEntity"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingNamedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
