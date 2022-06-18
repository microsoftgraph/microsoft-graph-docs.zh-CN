---
title: bookingCustomer 资源类型
description: 表示 bookingBusiness 的客户。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 7e4c31ec68cdda121dcb1f7954faa742746271fc
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160643"
---
# <a name="bookingcustomer-resource-type"></a>bookingCustomer 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
表示 [bookingBusiness](bookingbusiness.md) 的客户。


## <a name="methods"></a>方法

| 方法           | 返回类型    |Description|
|:---------------|:--------|:----------|
|[列出客户](../api/bookingbusiness-list-customers.md) | [bookingCustomer](bookingcustomer.md) 集合 | 获取 **bookingCustomer** 对象的列表。 |
|[创建 bookingCustomer](../api/bookingbusiness-post-customers.md) | [bookingCustomer](bookingcustomer.md) | 创建新的 **bookingCustomer** 对象。 |
|[获取 bookingCustomer](../api/bookingcustomer-get.md) | [bookingCustomer](bookingcustomer.md) |读取 **bookingCustomer** 对象的属性和关系。|
|[更新](../api/bookingcustomer-update.md) | 无  |更新 **bookingCustomer** 对象。 |
|[删除](../api/bookingcustomer-delete.md) | 无 |删除 **bookingCustomer** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|地址|[physicalAddress](../resources/physicaladdress.md) 集合|与客户关联的地址，包括家庭、业务和其他地址。|
|displayName|String|客户的名称。|
|emailAddress|String|客户的 SMTP 地址。|
|id|String| 客户的 ID。 只读。|
|phones|[phone](../resources/phone.md) collection|电话与客户关联的数字，包括家庭、商业和移动号码。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCustomer"
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


