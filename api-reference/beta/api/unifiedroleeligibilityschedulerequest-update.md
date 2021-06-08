---
title: 更新 unifiedRoleEligibilityScheduleRequest
description: 更新 unifiedRoleEligibilityScheduleRequest 对象的属性。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1c9fc6fa0ca837c83e90172fa49eca287c98a42f
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786683"
---
# <a name="update-unifiedroleeligibilityschedulerequest"></a>更新 unifiedRoleEligibilityScheduleRequest
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [unifiedRoleEligibilityScheduleRequest 对象](../resources/unifiedroleeligibilityschedulerequest.md) 的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|PrivilegedAccess.ReadWrite.AzureAD|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|不支持|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象的 JSON 表示形式。

下表显示更新 [unifiedRoleEligibilityScheduleRequest 时所需的属性](../resources/unifiedroleeligibilityschedulerequest.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|unifiedRoleEligibilityScheduleRequest 的唯一标识符。 键，不可为 null，只读|
|action|String|表示对项目执行的操作角色分配。 值可以是 <ul><li>`AdminAdd`：管理员将用户/组分配给角色;</li><li>`UserAdd`：用户激活符合条件的分配;</li><li> `AdminUpdate`：管理员更改现有角色分配</li><li>`AdminRemove`：管理员从角色中删除用户/组;<li>`UserRemove`：用户停用活动分配;<li>`UserExtend`：用户请求延长其过期分配;</li><li>`AdminExtend`：管理员扩展即将过期的工作分配。</li><li>`UserRenew`：用户请求续订其已过期的工作分配;</li><li>`AdminRenew`：管理员扩展即将过期的工作分配。</li></ul>|
|principalId|String|要授予分配的主体的 Objectid。|
|roleDefinitionId|String|分配所针对的 unifiedRoleDefinition 的 ID。 只读。|
|directoryScopeId|String|表示工作分配范围的目录对象的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 应用程序作用域是仅由此应用程序定义和理解的范围。|
|appScopeId|String|当分配范围特定于应用时，特定于应用的范围的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 对租户范围范围使用"/"。 应用程序作用域是仅由此应用程序定义和理解的范围。|
|isValidationOnly|Boolean|确定调用是验证还是实际调用的布尔值。 仅在要检查激活是否受 MFA 等其他规则限制，然后再实际提交请求时设置此属性。|
|targetScheduleId|String|附加到工作分配的计划对象的 ID。|
|justification|String|创建请求时由用户和管理员提供的消息，说明为什么需要该请求。|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|请求的计划角色分配对象。|
|ticketInfo|[ticketInfo](../resources/ticketinfo.md)|附加到请求的 ticketInfo 角色分配，其中包含票证编号和票证系统的详细信息。|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleeligibilityschedulerequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}
Content-Type: application/json
Content-length: 467

{
  "@odata.type": "#microsoft.graph.unifiedRoleEligibilityScheduleRequest",
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroleeligibilityschedulerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroleeligibilityschedulerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroleeligibilityschedulerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroleeligibilityschedulerequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
```http
HTTP/1.1 204 OK

```
<!--
{
  "@odata.type": "#microsoft.graph.unifiedRoleEligibilityScheduleRequest",
  "id": "a2e242a0-42a0-a2e2-a042-e2a2a042e2a2",
  "action": "String",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "isValidationOnly": "Boolean",
  "targetScheduleId": "String",
  "justification": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "ticketInfo": {
    "@odata.type": "microsoft.graph.ticketInfo"
  }
}
```
-->
