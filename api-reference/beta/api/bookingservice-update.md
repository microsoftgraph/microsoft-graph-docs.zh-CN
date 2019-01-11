---
title: 更新 bookingservice
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 6eee5949d5d8cee23821d726563b4687febd77a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838918"
---
# <a name="update-bookingservice"></a>更新 bookingservice

 > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。
 
更新中指定[bookingbusiness](../resources/bookingbusiness.md) [bookingService](../resources/bookingservice.md)对象的属性。

以下是您可以将自定义服务的一些示例：
- Price
- 约会的典型长度
- Reminders
- 任何时候，只要缓冲区之前设置或完成维修之后
- [计划策略](../resources/bookingschedulingpolicy.md)参数，如最低通知书籍或取消，以及是否客户可以选择的约会的特定人员成员。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  Bookings.ReadWrite.All Bookings.Manage.All   |
|委派（个人 Microsoft 帐户） | 不支持。   |
|应用程序 | 不支持。  |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a>可选的请求标头
| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|defaultDuration|Duration|默认服务中的天、 小时、 分钟和秒数字表示的长度。 例如，P11D23H59M59.999999999999S。 |
|defaultLocation|[location](../resources/location.md)|服务的默认物理位置。|
|defaultPrice|Double|该服务默认货币价格。|
|defaultPriceType|string|负责服务的默认方式。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。|
|defaultReminders|[bookingReminder](../resources/bookingreminder.md)集合|默认设置的该服务的约会的提醒。 此属性的值时，可仅读取此**bookingService**由其 id。|
|说明|字符串|服务的文本说明。|
|displayName|字符串|服务名称。|
|emailAddress|String|电子邮件地址|
|id|String| 只读。|
|isHiddenFromCustomers|布尔|True 表示该服务不是预定的客户。|
|notes|String|有关此服务的其他信息。|
|后|Duration|此服务的时间为缓冲区之后为约会结束，且在下一步之前客户约会可以为预约。|
|缓冲区|Duration|缓冲区之前可以启动此服务的约会的时间。|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|确定如何创建和管理服务此类型的约会的策略集。|
|staffMemberIds|String 集合|表示这些[员工](../resources/bookingstaffmember.md)提供此服务。 |

## <a name="response"></a>响应
如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面的示例将更新指定的服务的持续时间。
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
##### <a name="response"></a>响应
下面展示了示例响应。 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
