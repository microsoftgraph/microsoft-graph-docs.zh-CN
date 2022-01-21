---
title: 创建 unifiedRoleAssignmentMultiple
description: 创建新的 unifiedRoleAssignmentMultiple 对象。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d60221dece4d600d795adc81c3e321a23064eaa9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135142"
---
# <a name="create-unifiedroleassignmentmultiple"></a>创建 unifiedRoleAssignmentMultiple

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为 RBAC 提供程序创建新的 [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。 

目前支持以下 RBAC 提供程序：
- 云电脑 
- Intune (设备) 

For other Microsoft 365 applications (like Azure AD) ， use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).

## <a name="permissions"></a>权限

根据 RBAC 提供程序以及 (或应用程序) 类型，从下表中选择调用此 API 所需的最低特权权限。 若要了解 [更多信息，包括在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 选择更多特权权限之前保持谨慎，请参阅 [权限](/graph/permissions-reference)。 

### <a name="for-cloud-pc-provider"></a>对于云电脑提供商

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  CloudPC.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | CloudPC.ReadWrite.All  |

### <a name="for-device-management-intune-provider"></a>对于 Intune (设备) 提供程序

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  DeviceManagementRBAC.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | DeviceManagementRBAC.ReadWrite.All |


## <a name="http-request"></a>HTTP 请求

若要为角色分配创建云电脑提供商：

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/cloudPC/roleAssignments
```

若要创建角色分配 Intune 提供程序，
<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a>请求标头

| 名称 | 说明 |
|:---- |:----------- |
| Authorization | Bearer {token}。必需。 |
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象的 JSON 表示形式。 请求必须具有在 Azure AD 中定义的作用域（如 ）或特定于应用程序的范围（ `directoryScopeIds` 如 `appScopeId` ）。 例如Azure AD租户 (/") 、管理单元或应用程序。 

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和新的 `201 Created` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-create-a-role-assignment-in-intune-over-two-scope-groups-which-are-azure-ad-objects"></a>示例 1：在 Intune 角色分配两个作用域组上创建一个 (，这两Azure AD对象) 

#### <a name="request"></a>请求

下面展示了示例请求。
> **注意****：roleDefinitionId** 的 **roleTemplateId 的使用**。 **roleDefinitionId** 可以是服务范围的模板 ID 或特定于目录 **的 roleDefinitionId**。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"],
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroleassignmentmultiple-from-rbacapplication-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroleassignmentmultiple-from-rbacapplication-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。
> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"]
}
```

### <a name="example-2-create-a-role-assignment-in-intune-at-intune-specific-scope-of-all-devices"></a>示例 2：在 Intune 角色分配"所有设备"的 Intune 中创建一个应用

使用以下信息创建 Intune 角色分配：
- 若要允许在所有 Intune 设备上进行分配，请使用 `AllDevices` **appScopeIds 中的值**。
- 若要允许分配所有 Intune 许可用户，请使用 `AllLicensedUsers` **appScopeIds 中的值**。
- 若要允许分配所有 Intune 设备和许可用户，请使用 `/` **directoryScopeIds 中的值**。

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_intune_specific"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "appScopeIds": ["allDevices"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-intune-specific-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-intune-specific-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-intune-specific-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-intune-specific-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroleassignmentmultiple-intune-specific-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroleassignmentmultiple-intune-specific-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。
> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "appScopeIds": ["allDevices"]
}
```

### <a name="example-3-create-a-role-assignment-for-a-cloud-pc-provider"></a>示例 3：角色分配云电脑提供商

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_from_rbacapplication_cloudpc"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "description": "My role assignment description",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应

下面展示了示例响应。
> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "id": "47c88dcd-cc79-4b0c-ba7d-7af2199649c5",
    "displayName": "My role assignment",
    "description": "My role assignment description",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": [
        "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
        "c1518aa9-4da5-4c84-a902-a31404023890"
    ],
    "directoryScopeIds": [
        "/"
    ],
    "appScopeIds": []
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


