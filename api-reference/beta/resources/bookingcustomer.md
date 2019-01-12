---
title: bookingCustomer 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b213e4026ee33886c0e56db9790efff09fd8c522
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925103"
---
# <a name="bookingcustomer-resource-type"></a>bookingCustomer 资源类型

 > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。
 
代表[bookingBsiness](bookingbusiness.md)客户。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出的客户](../api/bookingbusiness-list-customers.md) | [bookingCustomer](bookingcustomer.md)集合 | 获取**bookingCustomer**对象的列表。 |
|[创建 bookingCustomer](../api/bookingbusiness-post-customers.md) | [bookingCustomer](bookingcustomer.md) | 创建新的**bookingCustomer**对象。 |
|[获取 bookingCustomer](../api/bookingcustomer-get.md) | [bookingCustomer](bookingcustomer.md) |读取的属性和**bookingCustomer**对象的关系。|
|[Update](../api/bookingcustomer-update.md) | [bookingCustomer](bookingcustomer.md) |更新**bookingCustomer**对象。 |
|[删除](../api/bookingcustomer-delete.md) | 无 |删除**bookingCustomer**对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|字符串|客户的名称。|
|emailAddress|String|客户的 SMTP 地址。|
|id|字符串| 客户的 ID。 只读。|

## <a name="relationships"></a>Relationships
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
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
