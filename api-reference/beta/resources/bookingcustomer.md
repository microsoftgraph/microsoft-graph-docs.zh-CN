---
title: bookingCustomer 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 3d5eff9d0add4a0840e864b9f4caf1730be98e5a
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696229"
---
# <a name="bookingcustomer-resource-type"></a>bookingCustomer 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
表示 [bookingBusiness 的客户](bookingbusiness.md)。


## <a name="methods"></a>Methods

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
|displayName|字符串|客户的名称。|
|emailAddress|String|客户的 SMTP 地址。|
|id|String| 客户的 ID。 只读。|
|地址|[physicalAddress](../resources/physicaladdress.md) 集合|与客户关联的地址，包括住宅、企业和其他地址。|
|phones|[phone](../resources/phone.md) collection|电话客户关联的电话号码，包括家庭号码、商务号码和移动电话号码。|

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


