---
title: 更新 bookingservice
description: 更新指定 bookingbusiness 中的 bookingService 对象的属性。
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 4a31643464159f7578619eb318ea186a988d6023
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094493"
---
# <a name="update-bookingservice"></a>更新 bookingservice

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新指定的 [bookingBusiness](../resources/bookingservice.md) 中的 [bookingService](../resources/bookingbusiness.md)对象的属性。

以下是您可以为服务自定义的一些示例：
- 价格
- 约会的典型长度
- Reminders
- 在服务之前或之后完成设置的任何时间缓冲区
- [计划策略](../resources/bookingschedulingpolicy.md) 参数，如预订或取消的最低通知，以及客户是否可以选择特定员工进行约会。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  Bookings.ReadWrite.All、Bookings.Manage.All   |
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
| Authorization  | Bearer {code}。 必需。|

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|defaultDuration|期限|服务的默认长度，以天数、小时数、分钟数和秒数表示。 例如，P11D23H59M59.9999999999S。 |
|defaultLocation|[location](../resources/location.md)|服务的默认物理位置。|
|defaultPrice|双精度|服务的默认货币价格。|
|defaultPriceType|bookingPriceType|服务收费的默认方式。 可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`、`unknownFutureValue`。|
|defaultReminders|[bookingReminder](../resources/bookingreminder.md) 集合|此服务约会的默认提醒集。 此属性的值仅在按其 ID 读取此 **bookingService** 时可用。|
|说明|String|服务的文本说明。|
|displayName|String|服务名称。|
|id|String| 只读。|
|isHiddenFromCustomers|布尔|True 表示客户无法预订此服务。|
|isLocationOnline|布尔|如果为 True，则表明该服务的约会将联机进行。 默认值为 false。|
|notes|String|有关此服务的其他信息。|
|postBuffer|期限|此服务的约会结束后以及下一个客户约会可以预订之前进行缓冲的时间。|
|preBuffer|期限|在此服务的约会可以启动之前缓冲的时间。|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|用于确定如何创建和管理这种类型的服务的约会的策略集。|
|smsNotificationsEnabled|布尔|如果为 True，则表明可以针对服务约会将短信通知发送给客户。 默认值为 false。|
|staffMemberIds|String 集合|表示 [提供此服务](../resources/bookingstaffmember.md) 的员工。 |
|customQuestions|[bookingQuestionAssignment](../resources/bookingquestionassignment.md) 集合|这包括与特定服务关联的一组自定义问题。 可选。|
|maximumAttendeesCount|Int32|服务中允许的最大客户数。  |

## <a name="response"></a>响应
如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。
## <a name="example"></a>示例
### <a name="request"></a>请求
以下示例更新指定服务的持续时间。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-bookingservice-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-bookingservice-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应
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
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


