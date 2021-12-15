---
title: bookingCustomerBase 资源类型
description: Bookings 客户的抽象基本类型。
author: davisjms
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 3eca954718608223977018b82f005001be269ba9
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525026"
---
# <a name="bookingcustomerbase-resource-type"></a>bookingCustomerBase 资源类型

命名空间：microsoft.graph

Bookings 客户的抽象基本类型。

[bookingCustomer 的基本类型](bookingcustomer.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|客户的 ID。 继承自 [实体](../resources/entity.md)。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingCustomerBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingCustomerBase",
  "id": "String (identifier)"
}
```

