---
title: 获取 applicationSignInSummary
description: 检索**applicationSigninSummary**对象的属性和关系。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2fe08254384c4ff7123e3876ba2286068d2ddb28
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322878"
---
# <a name="get-applicationsigninsummary"></a>获取 applicationSignInSummary

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索[applicationSigninSummary](../resources/applicationsigninsummary.md)对象的属性和关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Report. All |
|委派（个人 Microsoft 帐户） | 不支持   |
|Application | Report. All | 

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
``` http
reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a>函数参数

| 参数 | 说明 |
|:----------|:----------|
| period | `D7` (最近七天) 或`D30` (最近30天);其他值会生成错误。 |

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization | Bearer {code} |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功, 此方法在响应`200 OK`正文中返回响应代码和[applicationSignInSummary](../resources/applicationsigninsummary.md)对象。

## <a name="example"></a>示例

##### <a name="request"></a>请求
下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
### <a name="response"></a>响应
下面是一个响应示例。 

>**注意:** 在此处显示的响应对象将缩短 mmight 以提高可读性。 所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationSignInSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "appId": "appId-value",
  "appDisplayName": "appDisplayName-value",
  "successfulSignInCount": 99,
  "failedSignInCount": 99,
  "successPercentage": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
