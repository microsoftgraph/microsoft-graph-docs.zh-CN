---
title: 列出 tenantTags
description: 获取 tenantTag 对象及其属性的列表。
author: isaiahwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 60b35cdef256c4485e89d609b1c02d30e4e7c6ca
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020703"
---
# <a name="list-tenanttags"></a>列出 tenantTags
命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [tenantTag 对象](../resources/managedtenants-tenanttag.md) 及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|ManagedTenants.Read.All、ManagedTenants.WriteRead.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantTags
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。

## <a name="request-headers"></a>请求头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [tenantTag](../resources/managedtenants-tenanttag.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tenanttag"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tenanttag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tenanttag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tenanttag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tenanttag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-tenanttag-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenantTag)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/tenantTags",
    "value": [
        {
            "id": "913391c0-5466-42b4-900d-0a7501399cb0",
            "displayName": "Onboarding",
            "description": "Tenants that we are currently onboarding",
            "properties": null,
            "tenantIds": [
                "38227791-a88b-4fcc-81c5-58cf77668320",
                "34298981-4fc8-4974-9486-c8909ed1521b",
                "4d262a25-c70a-430b-9e8e-46c31dec116b"
            ],
            "isDeleted": null,
            "createdDateTime": "2021-06-16T20:36:31.086644Z",
            "createdByUserId": "9bf6a5ad-aecb-4194-a16b-38e02702a602",
            "lastActionDateTime": "2021-06-28T20:46:09.0071888Z",
            "lastActionByUserId": "08ea0285-30cb-46cc-abc8-3d8422e21ecb",
            "tenants": [
                {
                    "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
                },
                {
                    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b"
                },
                {
                    "tenantId": "4d262a25-c70a-430b-9e8e-46c31dec116b"
                }
            ]
        },
        {
            "id": "bfd883e8-10f3-40ee-994c-111fa1c5d1db",
            "displayName": "ExtendedSupport",
            "description": "Tenants that have purchased extended support.",
            "properties": null,
            "tenantIds": [
                "38227791-a88b-4fcc-81c5-58cf77668320",
                "4d262a25-c70a-430b-9e8e-46c31dec116b"
            ],
            "isDeleted": null,
            "createdDateTime": "2021-06-16T20:43:31.8917383Z",
            "createdByUserId": "43a2424c-0fa3-446d-bee9-4ab500bb1603",
            "lastActionDateTime": "2021-06-17T03:23:31.3531635Z",
            "lastActionByUserId": "248f617e-a6a7-4d31-922d-726c24074bb6",
            "tenants": [
                {
                    "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
                },
                {
                    "tenantId": "4d262a25-c70a-430b-9e8e-46c31dec116b"
                }
            ]
        }
    ]
}
```
