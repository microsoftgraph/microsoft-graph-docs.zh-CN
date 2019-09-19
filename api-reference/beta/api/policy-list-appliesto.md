---
title: 列出分配了特定策略的应用程序和服务主体
description: 获取分配了指定策略的应用程序和服务主体对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 2158c1183bcbf036c7b4b429675d70b0a0b175de
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036135"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a>列出分配了特定策略的应用程序和服务主体

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取分配了指定策略的[应用程序](../resources/application.md)和[服务主体](../resources/serviceprincipal.md)对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.Read.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Directory.Read.All |

## <a name="http-request"></a>HTTP 请求
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在`200 OK`响应正文中返回响应代码和[application](../resources/application.md)和[servicePrincipal](../resources/serviceprincipal.md)对象。 如果失败，将返回 `4xx` 错误并显示具体详细信息。

## <a name="example"></a>示例
下面的示例检索分配了特定策略的应用程序和服务主体。

##### <a name="request"></a>请求
下面是一个请求示例。

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value":[
        {
            "@odata.type"="#microsoft.graph.application",
            "appId":"appId-value",
            "displayName":"displayName-value",
            "errorUrl":"errorUrl-value",
            "groupMembershipClaims":"groupMembershipClaims-value",
            "homepage":"homepage-value",
            "id":"id-value",
            "keyCredentials":[key-credentials],
            "logoutUrl":"logoutUrl-value",
            "replyUrls":["replyUrls-value"]
        }
    ]
}
```
