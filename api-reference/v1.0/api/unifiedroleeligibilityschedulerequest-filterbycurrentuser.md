---
title: unifiedRoleEligibilityScheduleRequest： filterByCurrentUser
description: 在 PIM 中，检索针对特定主体的角色可取性请求。 主体可以是 unifiedRoleEligibilityScheduleRequest 对象的创建者或审批者，也可以是角色资格的目标。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6c7a14ee910de9e6631c290b2455a9c5f8fe5691
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437680"
---
# <a name="unifiedroleeligibilityschedulerequest-filterbycurrentuser"></a>unifiedRoleEligibilityScheduleRequest： filterByCurrentUser
命名空间：microsoft.graph

在 PIM 中，检索针对特定主体的角色可取性请求。 主体可以是 **unifiedRoleEligibilityScheduleRequest** 对象的创建者或审批者，也可以是角色资格的目标。

> [!NOTE]
> 此 API 不会通过组成员身份返回符合条件的角色分配。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RoleEligibilitySchedule.Read.Directory、RoleManagement.Read.Directory、RoleManagement.Read.All、RoleEligibilitySchedule.ReadWrite.Directory、RoleManagement.ReadWrite.Directory |
|委派（个人 Microsoft 帐户）|不支持|
|Application|RoleManagement.Read.Directory、RoleManagement.Read.All、RoleManagement.ReadWrite.Directory |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a>函数参数
在请求 URL 中，提供以下查询参数（含值）。
下表显示了可用于此函数的参数。

|参数|类型|说明|
|:---|:---|:---|
|on|roleEligibilityScheduleRequestFilterByCurrentUserOptions|可能的值是`principal`， ， `approver``createdBy`， 。 `unknownFutureValue` 仅 `principal` 支持并且 `approver` 当前受支持。|

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 `$select``$filter`OData 查询参数，`$expand`以帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此函数在响应正文中返回 `200 OK` 响应代码和 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityschedulerequestthis.filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleEligibilityScheduleRequests/filterByCurrentUser(on='principal')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unifiedroleeligibilityschedulerequestthisfilterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unifiedroleeligibilityschedulerequestthisfilterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unifiedroleeligibilityschedulerequestthisfilterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unifiedroleeligibilityschedulerequestthisfilterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/unifiedroleeligibilityschedulerequestthisfilterbycurrentuser-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/unifiedroleeligibilityschedulerequestthisfilterbycurrentuser-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilityScheduleRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(unifiedRoleEligibilityScheduleRequest)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.unifiedRoleEligibilityScheduleRequest",
            "id": "50877283-9d40-433c-bab8-7986dc10458a",
            "status": "Provisioned",
            "createdDateTime": "2022-04-12T09:05:41.807Z",
            "completedDateTime": "2022-04-12T09:05:41.853Z",
            "approvalId": null,
            "customData": null,
            "action": "adminAssign",
            "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
            "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
            "directoryScopeId": "/",
            "appScopeId": null,
            "isValidationOnly": false,
            "targetScheduleId": "50877283-9d40-433c-bab8-7986dc10458a",
            "justification": "Assign Attribute Assignment Admin eligibility to restricted user",
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "displayName": null,
                    "id": "3fbd929d-8c56-4462-851e-0eb9a7b3a2a5"
                }
            },
            "scheduleInfo": {
                "startDateTime": "2022-04-12T09:05:41.8532931Z",
                "recurrence": null,
                "expiration": {
                    "type": "afterDateTime",
                    "endDateTime": "2024-04-10T00:00:00Z",
                    "duration": null
                }
            },
            "ticketInfo": {
                "ticketNumber": null,
                "ticketSystem": null
            }
        },
        {
            "@odata.type": "#microsoft.graph.unifiedRoleEligibilityScheduleRequest",
            "id": "f341269e-c926-41fa-a905-cef3b01b2a67",
            "status": "Revoked",
            "createdDateTime": "2022-04-12T09:12:18.187Z",
            "completedDateTime": null,
            "approvalId": null,
            "customData": null,
            "action": "adminRemove",
            "principalId": "071cc716-8147-4397-a5ba-b2105951cc0b",
            "roleDefinitionId": "8424c6f0-a189-499e-bbd0-26c1753c96d4",
            "directoryScopeId": "/",
            "appScopeId": null,
            "isValidationOnly": false,
            "targetScheduleId": null,
            "justification": null,
            "scheduleInfo": null,
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "displayName": null,
                    "id": "3fbd929d-8c56-4462-851e-0eb9a7b3a2a5"
                }
            },
            "ticketInfo": {
                "ticketNumber": null,
                "ticketSystem": null
            }
        }
    ]
}
```

