---
title: bookingNamedEntity 资源类型
description: 这是 Microsoft Bookings 实体的基本类型，可提供显示名称，例如 bookingBusiness、bookingPerson、bookingService。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 9d0700f6ac86d16ad00684d429a0f88fdb7a16a7
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525286"
---
# <a name="bookingnamedentity-resource-type"></a>bookingNamedEntity 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
这是 Microsoft Bookings 实体的基本类型，可提供显示名称，例如 bookingBusiness、bookingPerson、bookingService[](bookingperson.md)和[bookingCustomQuestion。](bookingcustomquestion.md) [](bookingbusiness.md) [](bookingservice.md)

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|String|派生实体的名称，该实体与客户交互。|
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


