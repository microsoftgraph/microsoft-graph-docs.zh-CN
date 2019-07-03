---
title: 列出 secureScores
description: 检索 secureScore 对象的列表。
author: preetikr
localization_priority: Normal
ms.openlocfilehash: a632a0abdf15d91fc37a511ab75b50d8233d5a4c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441623"
---
# <a name="list-securescores"></a>列出 secureScores

检索[secureScore](../resources/securescore.md)对象的列表。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  Securityevents.readwrite.all、Securityevents.readwrite.all、All。   |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | Securityevents.readwrite.all、Securityevents.readwrite.all、All。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores
GET /security/secureScores?$top=1
GET /security/secureScores?$top=1&$skip=7
GET /security/secureScores?$filter={property} eq '{property-value}'
```
## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持以下 [OData 查询参数](/graph/query-parameters)，它们有助于自定义响应：

- `$count`
- `$filter`
- `$skip`
- `$top` 将返回每个安全 API 提供程序的顶部聚合结果。  

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {code}。 必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。 将忽略请求正文。

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和**secureScores**对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescores"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores?$top=1
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescores-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescores-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescores-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScore",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "00000001-0001-0001-0001-000000000001c_2019-03-19",
            "azureTenantId": "00000001-0001-0001-0001-000000000001c",
            "activeUserCount": 0,
            "createdDateTime": "2019-03-19T15:21:00Z",
            "currentScore": 387.0,
            "enabledServices": [
                "HasExchange",
                "HasSharePoint",
                "HasInTune"
            ],
            "licensedUserCount": 100,
            "maxScore": 697.0,
            "averageComparativeScores": [
                {
                    "basis": "AllTenants",
                    "averageScore": 37.0
                },
                {
                    "basis": "TotalSeats",
                    "averageScore": 46.0
                },
                {
                    "basis": "IndustryTypes",
                    "averageScore": 109.0
                }
            ],
            "controlScores": [
                {
                    "controlCategory": "Identity",
                    "controlName": "AdminMFA",
                    "description": "Requiring multi-factor authentication (MFA) for all Azure Active Directory accounts with privileged roles",
                    "score": 35.0
                },
                {
                    "controlCategory": "Data",
                    "controlName": "DLPEnabled",
                    "description": "Data Loss Prevention (DLP) policies can be used to comply with business standards and industry regulations.",
                    "score": 20.0
                }
            ],
            "vendorInformation": {
                "provider": "SecureScore",
                "providerVersion": null,
                "subProvider": null,
                "vendor": "Microsoft"
            }
        }
    ]
}

```


<!--
{
  "type": "#page.annotation",
  "description": "List secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
