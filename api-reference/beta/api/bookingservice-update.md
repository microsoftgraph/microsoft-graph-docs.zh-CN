---
title: 更新 bookingservice
description: 更新指定 bookingbusiness 中的 bookingService 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 607949e8c4b00230815fa8b29eba751494efb8b3
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636007"
---
# <a name="update-bookingservice"></a>更新 bookingservice

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新指定[bookingbusiness](../resources/bookingbusiness.md)中的[bookingService](../resources/bookingservice.md)对象的属性。

下面是可以为服务自定义的一些示例:
- 价格
- 约会的典型长度
- 提醒
- 在服务完成之前或结束前设置的任何时间缓冲
- 将策略参数 (如 "最低通知")[安排](../resources/bookingschedulingpolicy.md)为 "书籍" 或 "取消", 以及客户是否可以选择约会的特定员工成员。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  全部预订。全部, 全部预订。全部   |
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

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|defaultDuration|持续时间|服务的默认长度, 以天数、小时数、分钟数和秒数表示。 例如, P11D23H59M 59.999999999999 S。 |
|defaultLocation|[location](../resources/location.md)|服务的默认物理位置。|
|defaultPrice|双精度|服务的默认货币价格。|
|defaultPriceType|string|服务收费的默认方式。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。|
|defaultReminders|[bookingReminder](../resources/bookingreminder.md)集合|此服务的约会的默认提醒集。 此属性的值仅在按 ID 读取此**bookingService**时可用。|
|说明|String|服务的文本说明。|
|displayName|字符串|服务名称。|
|emailAddress|String|电子邮件地址|
|id|字符串| 只读。|
|isHiddenFromCustomers|Boolean|如果为 True, 则表示此服务不可供客户预订。|
|notes|字符串|有关此服务的其他信息。|
|postBuffer|持续时间|此服务的约会结束后以及下一个客户约会可以被预订前要缓冲的时间。|
|preBuffer|持续时间|在此服务的约会开始之前要缓冲的时间。|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|确定应如何创建和管理此类服务的约会的一组策略。|
|staffMemberIds|String collection|代表提供此服务的[教职员工成员](../resources/bookingstaffmember.md)。 |

## <a name="response"></a>响应
如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面的示例更新指定服务的持续时间。
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
下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[语言](#tab/cs)
[!INCLUDE [sample-code](../includes/update_bookingservice-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_bookingservice-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingservice-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
