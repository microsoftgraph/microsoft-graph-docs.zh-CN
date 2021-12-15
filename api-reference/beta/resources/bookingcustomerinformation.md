---
title: bookingCustomerInformation 资源类型
description: 注册约会的客户属性。 约会包含客户信息列表，每个单元指示属于该约会的客户的属性。
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: d72f54794cc637e7cb90a2f11b59cc2cb026d7ed
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525610"
---
# <a name="bookingcustomerinformation-resource-type"></a>bookingCustomerInformation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

注册约会的客户属性。 约会包含客户信息列表，每个单元指示属于该约会的客户的属性。

继承自 [bookingCustomerInformationBase](bookingcustomerinformationbase.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|customerId|String|此约会的 [bookingCustomer](../resources/bookingcustomer.md) 的 ID。 如果在创建约会时未指定任何 ID，则创建一个新的 **bookingCustomer** 对象。 设置后，你应考虑 customerId 不可变。 |
|customQuestionAnswers|[bookingQuestionAnswer](../resources/bookingquestionanswer.md) 集合|它由客户在约会中给出的自定义问题和答案列表组成。 |
|emailAddress|String| 预订约会 **的 bookingCustomer** 的 SMTP 地址。 |
|位置|[位置](../resources/location.md)| 表示预订约会的 **bookingCustomer** 的位置信息。 |
|name|字符串|客户的名称。 |
|notes|String|与此约会关联的客户的备注。 只有在通过 ID 读取 **此 bookingAppointment 时，才能** 获取该值。 只有在最初创建新客户的约会时，才能设置此属性。 此后，该值从 **customerId** 表示的客户计算。 |
|phone|String|客户的电话号码。 |
|timeZone|字符串|客户的时区。 有关可能值的列表，请参阅 [dateTimeTimeZone](../resources/datetimetimezone.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bookingCustomerInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingCustomerInformation",
  "customerId": "String",
  "name": "String",
  "emailAddress": "String",
  "phone": "String",
  "notes": "String",
  "location": {
    "@odata.type": "microsoft.graph.location"
  },
  "timeZone": "String",
  "customQuestionAnswers": [
    {
      "@odata.type": "microsoft.graph.bookingQuestionAnswer"
    }
  ]
}
```

