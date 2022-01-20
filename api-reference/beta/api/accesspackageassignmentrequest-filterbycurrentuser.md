---
title: accessPackageAssignmentRequest： filterByCurrentUser
description: 检索在已登录用户上筛选的 accesspackageassignmentrequest 对象列表。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 928063cd435aa2d0346a7b2935b69b16b8b59c5a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107208"
---
# <a name="accesspackageassignmentrequest-filterbycurrentuser"></a>accessPackageAssignmentRequest： filterByCurrentUser
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD管理](../resources/entitlementmanagement-overview.md)"中，检索在登录用户上筛选的[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a>函数参数
下表显示了可用于此函数的参数。

|参数|类型|Description|
|:---|:---|:---|
|on|[accessPackageAssignmentRequestFilterByCurrentUserOptions](../resources/accesspackageassignmentrequest-accesspackageassignmentrequestfilterbycurrentuseroptions.md)|可用于对访问包分配请求列表进行筛选的当前用户选项的列表。 可能的值为 `target` `createdBy` `approver` 、、。|

- `target` 用于获取 `accessPackageAssignmentRequest` 已登录用户作为目标的对象。 结果列表包括所有目录和访问包中调用方或调用方请求的所有分配请求（当前和已过期）。

- `createdBy` 用于获取 `accessPackageAssignmentRequest` 已登录用户创建的对象。 结果列表包括所有目录和访问包中调用方自己或代表其他人创建的所有分配请求，例如管理员直接分配。

- `approver` 用于获取已登录用户是任何包含的用户或用户集合中允许的审批 `accessPackageAssignmentRequest` `accessPackageAssignment/accessPackageAssignmentPolicy/requestApprovalSettings/approvalStages` `primaryApprovers` `escalationApprovers` () 。 生成的列表包括所有目录和访问包中挂起且需要调用方做出决策的分配请求。 生成的列表包括状态中跨所有目录和访问包的分配请求，并且需要 `pending` 调用方做出决策。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合。

## <a name="examples"></a>示例

以下示例获取针对已登录用户的访问包分配请求的状态。

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accesspackageassignmentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/filterByCurrentUser(on='target')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accesspackageassignmentrequest-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accesspackageassignmentrequest-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accesspackageassignmentrequest-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accesspackageassignmentrequest-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/accesspackageassignmentrequest-filterbycurrentuser-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/accesspackageassignmentrequest-filterbycurrentuser-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignmentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
            "createdDateTime": "2021-01-19T20:02:23.907Z",
            "completedDate": "2021-01-19T20:02:40.97Z",
            "id": "46c1410d-ef96-44c5-ae9c-a577d014fe0e",
            "requestType": "AdminAdd",
            "requestState": "Delivered",
            "requestStatus": "Fulfilled",
            "isValidationOnly": false,
            "expirationDateTime": null,
            "justification": null,
            "answers": [],
            "schedule": {
                "startDateTime": "2021-01-19T20:01:57.643Z",
                "recurrence": null,
                "expiration": {
                    "endDateTime": null,
                    "duration": null,
                    "type": "noExpiration"
                }
            }
        }
    ]
}
```

