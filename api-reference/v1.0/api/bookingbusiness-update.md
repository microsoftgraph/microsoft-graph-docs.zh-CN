---
title: 更新 bookingbusiness
description: 更新 bookingBusiness 对象的属性。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 3e86b5815999dc4c7388f00dd8077bed0fb1b906
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014164"
---
# <a name="update-bookingbusiness"></a>更新 bookingbusiness

命名空间：microsoft.graph

更新 [bookingBusiness 对象](../resources/bookingbusiness.md) 的属性。
## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  Bookings.ReadWrite.All、Bookings.Manage.All   |
|委派（个人 Microsoft 帐户） | 不支持。   |
|应用程序 | 不支持。  |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /solutions/bookingBusinesses/{id}
```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|address|[physicalAddress](../resources/physicaladdress.md)|企业街道地址。 physicalAddress 的属性类型在 v1.0 中不受支持。  在内部，我们将地址映射到类型 `others` 。|
|businessHours|[bookingWorkHours](../resources/bookingworkhours.md) 集合|企业运营的小时数。|
|businessType|String|业务类型。|
|defaultCurrencyIso|String|在 Microsoft Bookings 上运营业务的货币代码。|
|displayName|String|与客户交互的企业的名称。|
|email|String|企业的电子邮件地址。|
|phone|String|企业的电话号码。|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|指定如何为此业务创建预订。|
|webSiteUrl|String|业务网站的 URL。|

## <a name="response"></a>响应
如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。
## <a name="example"></a>示例
### <a name="request"></a>请求
以下示例更新了企业电子邮件地址和日程安排策略，将业务默认预订时间段更改为一小时，并提前预定最多 30 天。

<!-- {
  "blockType": "request"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/fabrikam@contoso.onmicrosoft.com
Content-type: application/json

{
  "email": "admin@fabrikam.com",
  "schedulingPolicy": {
      "timeSlotInterval": "PT60M",
      "minimumLeadTime": "P1D",
      "maximumAdvance": "P30D",
      "sendConfirmationsToOwner": true,
      "allowStaffSelection": true
  }
}
```

### <a name="response"></a>响应
这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingbusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


