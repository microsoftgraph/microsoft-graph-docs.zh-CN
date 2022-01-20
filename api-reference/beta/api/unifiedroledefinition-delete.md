---
title: 删除 unifiedRoleDefinition
description: 删除 unifiedRoleDefinition 对象。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 09e45b8db050a79a6e80e3a70d275493c78aa28c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089257"
---
# <a name="delete-unifiedroledefinition"></a>删除 unifiedRoleDefinition

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除 RBAC 提供程序的 [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) 对象。

目前支持以下 RBAC 提供程序：
- 云电脑
- Intune (设备) 
- 目录 (Azure AD)  

## <a name="permissions"></a>权限

根据 RBAC 提供程序以及 (或应用程序) 类型，从下表中选择调用此 API 所需的最小特权权限。 若要了解 [更多信息，包括在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 选择更多特权权限之前保持谨慎，请参阅 [权限](/graph/permissions-reference)。 

### <a name="for-a-cloud-pc-provider"></a>对于云电脑提供商

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | CloudPC.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | CloudPC.ReadWrite.All  |

### <a name="for-a-device-management-intune-provider"></a>对于 Intune (提供程序的设备) 管理

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  DeviceManagementRBAC.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | DeviceManagementRBAC.ReadWrite.All |

### <a name="for-a-directory-azure-ad-provider"></a>对于目录 (Azure AD) 提供程序

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All   |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

若要删除设备管理提供程序的角色定义，请运行：
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/deviceManagement/roleDefinitions/{id}
```

删除目录提供程序的角色定义：
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

若要删除云电脑提供商的角色定义，请运行：
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/cloudPc/roleDefinitions/{id}

```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example-1-delete-a-unifiedroledefinition-resource-for-a-directory-provider"></a>示例 1：删除目录提供程序的 **unifiedRoleDefinition** 资源

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-unifiedroledefinition-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-unifiedroledefinition-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="example-2-delete-a-unifiedroledefinition-resource-for-a-cloud-pc-provider"></a>示例 2：删除云电脑提供商的 **unifiedRoleDefinition** 资源
### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition_cloudpc"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/cloudPc/roleDefinitions/b7f5ddc1-b7dc-4d37-abce-b9d6fc15ffff
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroledefinition-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-unifiedroledefinition-cloudpc-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-unifiedroledefinition-cloudpc-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
