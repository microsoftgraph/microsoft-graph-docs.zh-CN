---
title: accessPackageAssignment：additionalAccess
description: 检索 accessPackageAssignment 对象的列表，这些对象指示可能分离职责冲突或访问不兼容的访问包。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6aac3e2ac4ecb3c539a24bf8fa730641e2fa09e1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203781"
---
# <a name="accesspackageassignment-additionalaccess"></a>accessPackageAssignment：additionalAccess
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD权利管理](../resources/entitlementmanagement-overview.md)中，检索 [accessPackageAssignment](../resources/accesspackageassignment.md) 对象的集合，这些对象指示目标用户具有指定访问包的分配以及另一个可能不兼容的访问包的分配。  这可用于准备为特定访问包配置不兼容的访问包。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageAssignments/additionalAccess(accessPackageId='parameterValue',incompatibleAccessPackageId='parameterValue')
```

## <a name="function-parameters"></a>函数参数
下表显示了必须随此函数一起提供的参数。  两个访问包 ID 必须是不同的。

|参数|类型|说明|
|:---|:---|:---|
| accessPackageId | String |  指示调用方要为其检索分配的访问包的 ID。 必填。 |
| incompatibleAccessPackageId | String | 特定的不兼容访问包，调用方希望仅检索用户还具有此不兼容访问包的分配的分配。 必填。 |

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 `$select``$filter`OData 查询参数，`$expand`以帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [accessPackageAssignment](../resources/accesspackageassignment.md) 对象集合。

当结果集跨多个页面时，Microsoft Graph在响应中返回包含`@odata.nextLink`下一页结果 URL 的属性的页面。 如果该属性存在，请继续在每个响应中使用 URL 发出其他请求 `@odata.nextLink` ，直到返回所有结果。 有关详细信息，请参阅[在应用中分页 Microsoft Graph数据](/graph/paging)。

## <a name="examples"></a>示例

以下示例获取对这两个访问包具有分配的用户的访问包分配。

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignment_additionalaccess"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments/additionalAccess(accessPackageId='2506aef1-3929-4d24-a61e-7c8b83d95e6f',incompatibleAccessPackageId='d5d99728-8c0b-4ede-83d2-cf9b0e8dabfb')?$expand=target
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accesspackageassignment-additionalaccess-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignment-additionalaccess-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignment-additionalaccess-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accesspackageassignment-additionalaccess-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/accesspackageassignment-additionalaccess-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/accesspackageassignment-additionalaccess-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
        {
            "@odata.type": "#microsoft.graph.accessPackageAssignment",
            "id": "a61f7889-ae61-4e97-a4dc-e4fa525f5b33",
            "catalogId": "beedadfe-01d5-4025-910b-84abb9369997",
            "accessPackageId": "2506aef1-3929-4d24-a61e-7c8b83d95e6f",
            "assignmentPolicyId": "07c7c99d-6cf3-4527-bd05-5fc2ac8e96e7",
            "targetId": "cdbdf152-82ce-479c-b5b8-df90f561d5c7",
            "target": {
                "id": "ebaf071e-c647-42c6-b86f-fbe3625b4b63",
                "objectId": "cdbdf152-82ce-479c-b5b8-df90f561d5c7",
                "displayName": "user1"
            }
        },
        {
            "@odata.type": "#microsoft.graph.accessPackageAssignment",
            "id": "a7284263-8233-44de-8095-0ee3ff5a1716",
            "catalogId": "beedadfe-01d5-4025-910b-84abb9369997",
            "accessPackageId": "2506aef1-3929-4d24-a61e-7c8b83d95e6f",
            "assignmentPolicyId": "07c7c99d-6cf3-4527-bd05-5fc2ac8e96e7",
            "targetId": "79a8f0b6-61dc-41db-b49e-470c278e05b6",
            "target": {
                "id": "9865b0f8-868f-42c6-a49b-3067eb4b2da1",
                "objectId": "79a8f0b6-61dc-41db-b49e-470c278e05b6",
                "displayName": "user2"
            }
        }
  ]
}

```

