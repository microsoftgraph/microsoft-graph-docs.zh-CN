---
title: rbacApplication：roleSchedules
description: 检索 roleAssignmentSchedules 和 roleEligibilitySchedules。
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3e098692d1c34b0b1eee077554e7620ace9a31f8
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453987"
---
# <a name="rbacapplication-roleschedules"></a>rbacApplication：roleSchedules
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 roleAssignmentSchedules 和 roleEligibilitySchedules。

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
GET /roleManagement/directory/roleSchedules
```

## <a name="function-parameters"></a>函数参数
下表显示了可用于此方法的查询参数。

|参数|类型|说明|
|:---|:---|:---|
|directoryScopeId|String|表示工作分配范围的目录对象的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 目录范围是存储在目录中的多个应用程序可以理解的共享范围。 用于 `/` 租户范围范围。 使用 **appScopeId** 将作用域限制为仅应用程序。 |
|appScopeId|String|当分配范围特定于应用时，特定于应用的范围的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 应用程序作用域是仅由此应用程序定义和理解的范围。 用于 `/` 租户范围的应用范围。 使用 **directoryScopeId** 将作用域限制为特定目录对象，例如管理单元。 |
|principalId|String| 要向其中授予工作分配的主体的标识符。 可以是组或用户。 |
|roleDefinitionId|String|工作分配的 unifiedRoleDefinition 的标识符。 只读。|


## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rbacapplication_roleschedules"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleSchedules(directoryScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',appScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',principalId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',roleDefinitionId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rbacapplication-roleschedules-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rbacapplication-roleschedules-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rbacapplication-roleschedules-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rbacapplication-roleschedules-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleScheduleBase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.Identity.Governance.Common.Data.ExternalModels.V1.unifiedRoleScheduleBase",
      "id": "String (identifier)",
      "principalId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "roleDefinitionId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "directoryScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "appScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "createdUsing": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "createdDateTime": "2020-09-09T21:32:27.91Z",
      "modifiedDateTime": "2020-09-09T21:32:27.91Z",
      "status": "Provisioned"
    }
  ]
}
```
