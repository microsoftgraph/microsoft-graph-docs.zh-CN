---
title: 列出 customQuestions
description: 获取与 bookingBusiness 关联的 bookingCustomQuestion 资源。
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: aeac18a40b718724e3d7e7ab3516096024d204f9
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014248"
---
# <a name="list-customquestions"></a>列出 customQuestions

命名空间：microsoft.graph

获取与[bookingBusiness](../resources/bookingbusiness.md)关联的[bookingCustomQuestion](../resources/bookingcustomquestion.md)资源。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                                    |
| :------------------------------------- | :----------------------------------------------------------------------------- |
| 委派（工作或学校帐户）     | BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All |
| 委派（个人 Microsoft 帐户） | 不支持。                                                                 |
| 应用程序                            | 不支持。                                                                 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}-->

```http
GET /solutions/bookingBusinesses/{bookingBusinessesId}/customQuestions
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持一些 OData 查询参数来帮助自定义响应。 有关一般信息，请参阅 $count 和 $expand [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [bookingCustomQuestion](../resources/bookingcustomquestion.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customQuestions
```

### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomQuestion",
  "isCollection": true
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "@odata.type": "#microsoft.graph.bookingCustomQuestion",
        "id": "3bc6fde0-4ad3-445d-ab17-0fc15dba0774",
        "displayName": "What is your age?",
        "answerInputType": "text",
        "answerOptions": [],
    },
    {
        "@odata.type": "#microsoft.graph.bookingCustomQuestion",
        "id": "dbb865a6-530d-46e1-8e88-5d76789034b2",
        "displayName": "What is your nationality?",
        "answerInputType": "radioButton",
        "answerOptions": [
          "US",
          "UK",
          "Canada",
          "India"
        ],
    }
  ]
}
```
