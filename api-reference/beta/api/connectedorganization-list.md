---
title: 列出 connectedOrganizations
description: 检索 connectedOrganization 对象的列表。
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0d74b4624833ca8c6a9feecf824f6e4346ca952c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437441"
---
# <a name="list-connectedorganizations"></a>列出 connectedOrganizations

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [connectedOrganization 对象](../resources/connectedorganization.md) 的列表。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
| 委派（工作或学校帐户）     | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 例如，若要仅检索具有特定组织连接显示名称，请添加 `$filter=displayName eq 'Name'` 。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [connectedOrganization](../resources/connectedorganization.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectedorganizations"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectedorganizations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectedorganizations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectedorganizations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectedorganizations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.connectedOrganization)"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "cd3709c6-be6a-4725-bd07-50f90ccca93f",
      "displayName": "Wingtip Toys",
      "description": "Wingtip Toys",
      "createdBy": "admin@contoso.com",
      "createdDateTime": "2020-05-13T15:18:04.81Z",
      "modifiedBy": "admin@contoso.com",
      "modifiedDateTime": "2020-05-13T15:18:04.81Z",
      "identitySources": [
        {
          "@odata.type": "#microsoft.graph.azureActiveDirectoryTenant",
          "tenantId": "bf85dc9d-cb43-44a4-80c4-469e8c58249e",
          "displayName": "Wingtip Toys Co"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List connectedOrganizations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


