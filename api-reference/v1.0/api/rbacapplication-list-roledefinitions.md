---
title: 列出 roleDefinitions
description: 获取 unifiedRoleDefinition 对象的列表。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: ab357d7006050a41b5169f1e9a09212bcdf70178
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366154"
---
# <a name="list-roledefinitions"></a>列出 roleDefinitions

命名空间：microsoft.graph

获取提供程序的 [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象列表。

目前支持以下 RBAC 提供程序：
- 目录 (Azure AD) 
- Azure AD (权利管理) 

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

### <a name="for-the-directory-azure-ad-provider"></a>对于目录 (Azure AD) 提供程序

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All |


### <a name="for-the-entitlement-management-provider"></a>对于权利管理提供程序

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

列出目录提供程序的角色定义：

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions
```

列出权利管理提供程序的角色定义：
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/entitlementManagement/roleDefinitions
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 (和运算符) OData 查询参数和 `displayName``isBuiltIn` `id`属性。`in` `eq` `$filter` 它还支持 `$expand` 关系。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象的集合。

## <a name="example"></a>示例

### <a name="example-1-retrieve-role-definitions-for-the-directory-provider"></a>示例 1：检索目录提供程序的角色定义

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleDefinitions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roledefinitions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-roledefinitions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-roledefinitions-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleDefinitions",
    "value": [
        {
            "id": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "description": "Can reset passwords for non-administrators and Helpdesk Administrators.",
            "displayName": "Helpdesk Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/users/invalidateAllRefreshTokens",
                        "microsoft.directory/users/bitLockerRecoveryKeys/read",
                        "microsoft.directory/users/password/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        },
        {
            "id": "f023fd81-a637-4b56-95fd-791ac0226033",
            "description": "Can read service health information and manage support tickets.",
            "displayName": "Service Support Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "f023fd81-a637-4b56-95fd-791ac0226033",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        },
        {
            "id": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "description": "Can perform common billing related tasks like updating payment information.",
            "displayName": "Billing Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/organization/basic/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.commerce.billing/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        }
    ]
}
```

### <a name="example-2-retrieve-role-definitions-for-the-entitlement-management-provider"></a>示例 2：检索权利管理提供程序的角色定义

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions_entitlementmanagement_provider"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/roleManagement/entitlementManagement/roleDefinitions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-entitlementmanagement-provider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-entitlementmanagement-provider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-entitlementmanagement-provider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roledefinitions-entitlementmanagement-provider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-roledefinitions-entitlementmanagement-provider-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-roledefinitions-entitlementmanagement-provider-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/entitlementManagement/roleDefinitions",
    "value": [
        {
            "id": "ae79f266-94d4-4dab-b730-feca7e132178",
            "displayName": "Catalog owner",
            "description": "Catalog owner",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "ae79f266-94d4-4dab-b730-feca7e132178",
            "version": "1.0",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.entitlementManagement/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ]
        },
        {
            "id": "44272f93-9762-48e8-af59-1b5351b1d6b3",
            "displayName": "Catalog reader",
            "description": "Catalog reader",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "44272f93-9762-48e8-af59-1b5351b1d6b3",
            "version": "1.0",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.entitlementManagement/allEntities/Read"
                    ],
                    "condition": null
                }
            ]
        },
        {
            "id": "7f480852-ebdc-47d4-87de-0d8498384a83",
            "displayName": "AccessPackages manager",
            "description": "AccessPackages manager",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "7f480852-ebdc-47d4-87de-0d8498384a83",
            "version": "1.0",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.entitlementManagement/AccessPackageCatalog/AccessPackage/allTasks",
                        "microsoft.entitlementManagement/AccessPackageCatalog/allEntities/Read"
                    ],
                    "condition": null
                }
            ]
        },
        {
            "id": "ba92d953-d8e0-4e39-a797-0cbedb0a89e8",
            "displayName": "Catalog creator",
            "description": "Catalog creator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "ba92d953-d8e0-4e39-a797-0cbedb0a89e8",
            "version": "1.0",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.entitlementManagement/AccessPackageCatalog/Create"
                    ],
                    "condition": null
                }
            ]
        },
        {
            "id": "e2182095-804a-4656-ae11-64734e9b7ae5",
            "displayName": "AccessPackage assignment manager",
            "description": "AccessPackage assignment manager",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "e2182095-804a-4656-ae11-64734e9b7ae5",
            "version": "1.0",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.entitlementManagement/AccessPackageCatalog/AccessPackage/GrantRequests/allTasks",
                        "microsoft.entitlementManagement/AccessPackageCatalog/AccessPackage/Grants/allTasks",
                        "microsoft.entitlementManagement/AccessPackageCatalog/allEntities/Read"
                    ],
                    "condition": null
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
  "description": "List roleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

