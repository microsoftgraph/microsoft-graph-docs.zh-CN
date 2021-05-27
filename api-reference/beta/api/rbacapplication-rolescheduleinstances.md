---
title: rbacApplication：roleScheduleInstances
description: 检索 roleAssignmentScheduleInstances 和 roleEligibilityScheduleInstances。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 497b29892bb510aec9763cab21ce8f06518a2eee
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679671"
---
# <a name="rbacapplication-rolescheduleinstances"></a>rbacApplication：roleScheduleInstances
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 roleAssignmentScheduleInstances 和 roleEligibilityScheduleInstances。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|PrivilegedAccess.ReadWrite.AzureAD|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|PrivilegedAccess.Read.AzureAD|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleScheduleInstances
```

## <a name="query-parameters"></a>查询参数
在请求 URL 中，提供以下查询参数（含值）。
下表显示了可用于此方法的查询参数。

|参数|类型|说明|
|:---|:---|:---|
|directoryScopeId|String|表示工作分配范围的目录对象的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 应用程序作用域是仅由此应用程序定义和理解的范围。 |
|appScopeId|String|特定于应用的范围的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 对租户范围范围使用"/"。 应用程序作用域是仅由此应用程序定义和理解的范围。 |
|principalId|String|计划所属的主体的 Objectid。 |
|roleDefinitionId|String|工作分配的 unifiedRoleDefinition 的 ID。 只读。|

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) 集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rbacapplication_rolescheduleinstances"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleScheduleInstances(directoryScopeId='parameterValue',appScopeId='parameterValue',principalId='parameterValue',roleDefinitionId='parameterValue')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rbacapplication-rolescheduleinstances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rbacapplication-rolescheduleinstances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rbacapplication-rolescheduleinstances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rbacapplication-rolescheduleinstances-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleScheduleInstanceBase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.Identity.Governance.Common.Data.ExternalModels.V1.unifiedRoleScheduleInstanceBase",
      "id": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "principalId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "roleDefinitionId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "directoryScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "appScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea"
    }
  ]
}
```
