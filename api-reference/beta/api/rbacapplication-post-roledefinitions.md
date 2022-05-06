---
title: 创建 roleDefinitions
description: 创建新的 unifiedRoleDefinition 对象。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6a53b70d813ba0104bcd93f525866d8c73cf378e
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246830"
---
# <a name="create-roledefinitions"></a>创建 roleDefinitions

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为 RBAC 提供程序创建新的 [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象。

目前支持以下 RBAC 提供程序：
- 云电脑
- 设备管理 (Intune) 
- 目录 (Azure AD) 

## <a name="permissions"></a>Permissions

根据 RBAC 提供程序和权限类型 (委派或应用程序) 需要，请从下表中选择调用此 API 所需的最低特权权限。 若要了解详细信息，包括在选择更多特权权限之前 [要小心](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) ，请参阅 [权限](/graph/permissions-reference)。 

### <a name="for-a-cloud-pc-provider"></a>对于云电脑提供商

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | RoleManagement.ReadWrite.CloudPC、CloudPC.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | RoleManagement.ReadWrite.CloudPC、CloudPC.ReadWrite.All  |

### <a name="for-a-device-management-intune-provider"></a>对于设备管理 (Intune) 提供程序

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  DeviceManagementRBAC.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | DeviceManagementRBAC.ReadWrite.All |

### <a name="for-a-directory-azure-ad-provider"></a>对于目录 (Azure AD) 提供程序

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

若要为设备管理提供程序创建角色定义，请执行以下操作：
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/deviceManagement/roleDefinitions
```

若要为目录提供程序创建角色定义，请执行以下操作：
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/directory/roleDefinitions
```

若要为云电脑提供商创建角色定义，请执行以下操作：
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/cloudPc/roleDefinitions
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象的 JSON 表示形式。

下表显示了创建 roleDefinition 时所需的属性。

| 参数 | 类型 | 说明|
|:---------------|:--------|:----------|
|displayName |string |角色定义的显示名称。|
|isEnabled |Boolean |指示是否为分配启用角色的标志。 如果为 false，则该角色不可用于分配。|
|rolePermissions |[unifiedRolePermission](../resources/unifiedrolepermission.md) 集合 |角色中包含的权限列表。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和新的 [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象。

## <a name="example-1create-a-custom-role-for-a-directory-provider"></a>示例 1：为目录提供程序创建自定义角色

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroledefinition_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
Content-type: application/json

{
  "description": "Update basic properties of application registrations",
  "displayName": "Application Registration Support Administrator",
  "rolePermissions":
    [
        {
            "allowedResourceActions": 
            [
                "microsoft.directory/applications/basic/read"
            ]
        }
    ],
    "isEnabled" : "true"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroledefinition-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroledefinition-from-rbacapplication-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroledefinition-from-rbacapplication-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。
> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "d5eec5e0-6992-4c6b-b430-0f833f1a815a",
    "description": "Update basic properties of application registrations",
    "displayName": "Application Registration Support Administrator",
    "isBuiltIn": false,
    "isEnabled": true,
    "templateId": "d5eec5e0-6992-4c6b-b430-0f833f1a815a",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/standard/read",
                "microsoft.directory/applications/basic/update"
            ],
            "condition": null
        }
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('d5eec5e0-6992-4c6b-b430-0f833f1a815a')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": []
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

### <a name="example-2-create-a-custom-role-for-a-cloud-pc-provider"></a>示例 2：为云电脑提供商创建自定义角色

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroledefinition_from_rbacapplication_cloudpc"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/cloudPc/roleDefinitions
Content-type: application/json

{
  "description": "An example custom role",
  "displayName": "ExampleCustomRole",
  "rolePermissions":
    [
        {
            "allowedResourceActions": 
            [
                "Microsoft.CloudPC/CloudPCs/Read"
            ]
        }
    ],
    "condition" : "null"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroledefinition-from-rbacapplication-cloudpc-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroledefinition-from-rbacapplication-cloudpc-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。
> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPc/roleDefinitions/$entity",
    "id": "b7f5ddc1-b7dc-4d37-abce-b9d6fc15ffff",
    "description": "An example custom role",
    "displayName": "ExampleCustomRole",
    "isBuiltIn": false,
    "isEnabled": true,
    "templateId": "b7f5ddc1-b7dc-4d37-abce-b9d6fc15ffff",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "Microsoft.CloudPC/CloudPCs/Read"
            ],
            "condition": null
        }
    ],
    "resourceScopes":["/"]
}
```
