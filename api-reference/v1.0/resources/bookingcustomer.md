---
title: bookingCustomer 资源类型
description: 表示 bookingBusiness 的客户。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: fa9bf3e9ebe49857972635dc87c604d066b6da12
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526648"
---
# <a name="bookingcustomer-resource-type"></a>bookingCustomer 资源类型

命名空间：microsoft.graph

表示 [bookingBusiness 的客户](bookingbusiness.md)。

继承自 [bookingCustomerBase](bookingcustomerbase.md)。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出客户](../api/bookingbusiness-list-customers.md) | [bookingCustomer](bookingcustomer.md) 集合 | 获取 **bookingCustomer 对象** 的列表。 |
|[创建 bookingCustomer](../api/bookingbusiness-post-customers.md) | [bookingCustomer](bookingcustomer.md) | 创建新的 **bookingCustomer** 对象。 |
|[获取 bookingCustomer](../api/bookingcustomer-get.md) | [bookingCustomer](bookingcustomer.md) |读取 **bookingCustomer** 对象的属性和关系。|
|[更新](../api/bookingcustomer-update.md) | [bookingCustomer](bookingcustomer.md) |更新 **bookingCustomer** 对象。 |
|[删除](../api/bookingcustomer-delete.md) | 无 |删除 **bookingCustomer** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|String|客户的名称。|
|emailAddress|String|客户的 SMTP 地址。|
|id|String| 客户的 ID。 只读。|
|地址|[physicalAddress](../resources/physicaladdress.md) 集合|与客户关联的地址。 physicalAddress 的属性类型在 v1.0 中不受支持。  在内部，我们将地址映射到类型 `others` 。|
|phones|[phone](../resources/phone.md) collection|电话客户关联的电话号码，包括家庭号码、商务号码和移动电话号码。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCustomer",
  "baseType": "microsoft.graph.bookingCustomerBase"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "addresses": [
    {
      "@odata.type": "microsoft.graph.physicalAddress"
    }
  ],
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


