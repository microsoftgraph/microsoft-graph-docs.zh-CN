---
title: 创建 bookingCustomQuestion
description: 创建新的 bookingCustomQuestion 对象。
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: f1b8ee38c527d8972ee38014a51f6f38cb3bd3b6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106892"
---
# <a name="create-bookingcustomquestion"></a>创建 bookingCustomQuestion

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [bookingCustomQuestion](../resources/bookingcustomquestion.md) 对象。

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
POST /bookingBusinesses/{bookingBusinessesId}/customQuestions
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [bookingCustomQuestion](../resources/bookingcustomquestion.md) 对象的 JSON 表示形式。

您可以在创建 **bookingCustomQuestion** 时指定以下属性。

| 属性        | 类型              | Description                                                                                                         |
| :-------------- | :---------------- | :------------------------------------------------------------------------------------------------------------------ |
| answerInputType | answerInputType   | 预期的答案类型。 可能的值包括 `text`、`radioButton`、`unknownFutureValue`。 可选。    |
| answerOptions   | String 集合 | 可能的答案值列表。 可选。                                                                     |
| displayName     | String            | 问题。 继承自 [bookingNamedEntity](../resources/bookingnamedentity.md)。 必需。 |

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [bookingCustomQuestion](../resources/bookingcustomquestion.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_bookingcustomquestion_from_"
}
-->

```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customQuestions/3bc6fde0-4ad3-445d-ab17-0fc15dba0774
Content-Type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.bookingCustomQuestion",
  "displayName": "What is your age?",
  "answerInputType": "text",
  "answerOptions": []
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingcustomquestion-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingcustomquestion-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomQuestion"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.bookingCustomQuestion",
  "id": "3bc6fde0-4ad3-445d-ab17-0fc15dba0774",
  "displayName": "What is your age?",
  "answerInputType": "text",
  "answerOptions": []
}
```
