---
title: 更新 bookingCustomQuestion
description: 更新 bookingCustomQuestion 对象的属性。
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 1e4f16585de42fb094c404283870c348d0579fe9
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526940"
---
# <a name="update-bookingcustomquestion"></a>更新 bookingCustomQuestion

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [bookingCustomQuestion 对象](../resources/bookingcustomquestion.md) 的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                                    |
| :------------------------------------- | :----------------------------------------------------------------------------- |
| 委派（工作或学校帐户）     | BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All |
| 委派（个人 Microsoft 帐户） | 不支持。                                                                 |
| 应用程序                            | 不支持。                                                                 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /bookingBusinesses/{bookingBusinessesId}/customQuestions/{bookingCustomQuestionId}
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| 属性        | 类型              | 说明                                                                                                         |
| :-------------- | :---------------- | :------------------------------------------------------------------------------------------------------------------ |
| answerInputType | answerInputType   | 预期的答案类型。 可能的值包括 `text`、`radioButton`、`unknownFutureValue`。 可选。    |
| answerOptions   | 字符串集合 | 可能的答案值列表。 可选。                                                                   |
| displayName     | String            | 问题。 继承自 [bookingNamedEntity](../resources/bookingnamedentity.md)。 必需。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [bookingCustomQuestion](../resources/bookingcustomquestion.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "update_bookingcustomquestion"
}
-->

```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customQuestions/3bc6fde0-4ad3-445d-ab17-0fc15dba0774
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.bookingCustomQuestion",
  "displayName": "What is your age?",
  "answerInputType": "text",
  "answerOptions": []
}
```

### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomQuestion"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.bookingCustomQuestion",
  "id": "3bc6fde0-4ad3-445d-ab17-0fc15dba0774",
  "displayName": "What is your age?",
  "answerInputType": "text",
  "answerOptions": []
}
```
