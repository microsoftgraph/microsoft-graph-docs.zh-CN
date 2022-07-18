---
title: 列出组织
description: 检索组织对象列表。
ms.localizationpriority: medium
author: KuiGithui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 93e6e21363c4071c65f590d3e8c948a3d6a18a0b
ms.sourcegitcommit: a11c874a7806fb5825752c8348e12079d23323e4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2022
ms.locfileid: "65293984"
---
# <a name="list-organization"></a>列出组织

命名空间：microsoft.graph



检索组织对象列表。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.Read、Directory.Read.All、Directory.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Directory.Read.All、Directory.ReadWrite.All |

> 注意：授予 User.Read 权限的应用程序仅能读取组织的 *id*、*displayName* 和 *verifiedDomains* 属性。  所有其他属性将返回 `null` 值。 若要读取所有属性，请使用 Directory.Read.All。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/organization.md) 对象集合。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-organization-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-organization-2-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
下面是一个响应示例。 
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#organization",
    "value": [
        {
            "id": "84841066-274d-4ec0-a5c1-276be684bdd3",
            "deletedDateTime": null,
            "businessPhones": [
                "425-555-0100"
            ],
            "city": null,
            "country": null,
            "countryLetterCode": "NL",
            "createdDateTime": "2021-08-02T10:30:06Z",
            "displayName": "Contoso",
            "isMultipleDataLocationsForServicesEnabled": null,
            "marketingNotificationEmails": [],
            "onPremisesLastSyncDateTime": null,
            "onPremisesSyncEnabled": null,
            "postalCode": null,
            "preferredLanguage": "en",
            "securityComplianceNotificationMails": [],
            "securityComplianceNotificationPhones": [],
            "state": null,
            "street": null,
            "technicalNotificationMails": [
                "admin@contoso.com"
            ],
            "tenantType": "AAD",
            "directorySizeQuota": {
                "used": 698,
                "total": 50000
            },
            "assignedPlans": [
                {
                    "assignedDateTime": "2022-04-03T02:46:42Z",
                    "capabilityStatus": "Deleted",
                    "service": "Adallom",
                    "servicePlanId": "932ad362-64a8-4783-9106-97849a1a30b9"
                },
                {
                    "assignedDateTime": "2022-04-03T02:46:42Z",
                    "capabilityStatus": "Deleted",
                    "service": "MultiFactorService",
                    "servicePlanId": "8a256a2b-b617-496d-b51b-e76466e88db0"
                },
                {
                    "assignedDateTime": "2021-08-02T10:36:57Z",
                    "capabilityStatus": "Enabled",
                    "service": "exchange",
                    "servicePlanId": "113feb6c-3fe4-4440-bddc-54d774bf0318"
                },
                {
                    "assignedDateTime": "2021-08-02T10:36:02Z",
                    "capabilityStatus": "Deleted",
                    "service": "SCO",
                    "servicePlanId": "882e1d05-acd1-4ccb-8708-6ee03664b117"
                }
            ],
            "privacyProfile": {
                "contactEmail": "",
                "statementUrl": ""
            },
            "provisionedPlans": [
                {
                    "capabilityStatus": "Deleted",
                    "provisioningStatus": "Success",
                    "service": "Adallom"
                },
                {
                    "capabilityStatus": "Enabled",
                    "provisioningStatus": "Success",
                    "service": "exchange"
                }
            ],
            "verifiedDomains": [
                {
                    "capabilities": "Email, OfficeCommunicationsOnline",
                    "isDefault": true,
                    "isInitial": true,
                    "name": "Contoso.onmicrosoft.com",
                    "type": "Managed"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
