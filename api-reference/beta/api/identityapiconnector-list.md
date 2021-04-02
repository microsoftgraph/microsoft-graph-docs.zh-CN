---
title: 列出 identityApiConnectors
description: 获取 identityApiConnector 对象及其属性的列表
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6aa2d3a4a5c45dc7b9e0b168eac7402404fcb982
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507845"
---
# <a name="list-identityapiconnectors"></a>列出 identityApiConnectors

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [identityApiConnector 对象](../resources/identityapiconnector.md) 的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | APIConnectors.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。  |
| 应用程序                            | APIConnectors.ReadWrite.All |

工作或学校帐户需要属于以下角色之一：

* 全局管理员
* 外部标识用户流管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identity/apiConnectors/
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [identityApiConnector](../resources/identityapiconnector.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_identityApiConnectors"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/apiConnectors
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-identityapiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-identityapiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-identityapiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-identityapiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector",
  "isCollection": true
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors",
    "value": [
        {
            "id": "<guid>",
            "displayName": "Test API",
            "targetUrl": "https://someapi.com/api/endpoint",
            "authenticationConfiguration": {
              "@odata.type": "#microsoft.graph.basicAuthentication",
              "username": "<USERNAME>",
              "password": "******"
            }
        },
        {
            "id": "<guid>",
            "displayName": "My API connector",
            "targetUrl": "https://someotherapi.com/api/endpoint",
            "authenticationConfiguration": {
                "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
                "certificateList": [
                    {
                        "thumbprint": "0EB255CC895477798BA418B378255204304897AD",
                        "notAfter": 1666350522,
                        "notBefore": 1508670522,
                        "isActive": true
                    },
                    {
                        "thumbprint": "1AB255CC895477798BA418B378255204304897BC",
                        "notAfter": 1766350522,
                        "notBefore": 1608670522,
                        "isActive": false
                    }
                ]
            }
        }
  ]
}
```
