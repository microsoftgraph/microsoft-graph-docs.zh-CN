---
title: 更新 unifiedRoleDefinition
description: 更新 unifiedRoleDefinition 对象的属性。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3d6e727ad610594b1ba9997c81479fdd9dded2d9
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524621"
---
# <a name="update-unifiedroledefinition"></a>更新 unifiedRoleDefinition

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 RBAC 提供程序 [的 unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象的属性。


目前支持以下 RBAC 提供程序：
- 云电脑
- Intune (设备) 
- 目录 (Azure AD)  


## <a name="permissions"></a>权限

根据 RBAC 提供程序以及 (或应用程序) ，从下表中选择调用此 API 所需的最低特权权限。 若要了解 [更多信息（包括在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 选择更多特权权限之前要谨慎操作），请搜索权限参考 [中的以下权限](/graph/permissions-reference)。 

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

若要更新设备管理提供程序的角色定义，请运行：
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/deviceManagement/roleDefinitions/{id}
```

更新目录提供程序的角色定义：
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

若要更新云电脑提供商的角色定义，请运行：
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/cloudPc/roleDefinitions/{id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|String| 角色定义的说明。 isBuiltIn 为 true 时为只读。 |
|displayName|String| 角色显示名称的角色定义。 isBuiltIn 为 true 时为只读。 必需。|
|id|String| 角色定义的唯一标识符。 键，不可为 null，只读。 |
|isBuiltIn|Boolean| 指示角色定义是否属于产品或自定义中包含的默认集的标志。 只读。 |
|isEnabled|Boolean| 指示角色是否已启用分配的标志。 如果为 false，则角色不能用于分配。 isBuiltIn 为 true 时为只读。 |
|resourceScopes|String collection| 角色定义授予的作用域权限列表适用。 目前仅支持"/"。 isBuiltIn 为 true 时为只读。 **请勿使用。此属性将很快弃用。将作用域附加到角色分配。**|
|rolePermissions|[unifiedRolePermission](../resources/unifiedrolepermission.md) 集合| 角色中包含的权限列表。 isBuiltIn 为 true 时为只读。 必填。 |
|templateId|String| 可以在 isBuiltIn 为 false 时设置的自定义模板标识符。 如果一个标识符在不同目录之间需要相同，则通常使用此标识符。 isBuiltIn 为 true 时为只读。 |
|inheritsPermissionsFrom| [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 集合| 给定角色定义从其继承的角色定义的只读集合。 只有Azure AD角色才支持此属性。 |
|version|String| 指示角色定义的版本。 isBuiltIn 为 true 时为只读。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="example-1-updates-a-unifiedroledefinition-for-a-directory-provider"></a>示例 1：为目录提供程序更新 **unifiedRoleDefinition**

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/0d55728d-3e24-4309-9b1b-5ac09921475a
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
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-unifiedroledefinition-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。
> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
Content-type: application/json

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedroledefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="example-2-updates-a-unifiedroledefinition-for-a-cloudpc-provider"></a>示例 2：为 CloudPC 提供程序更新 **unifiedRoleDefinition**

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition_cloudpc"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/cloudPc/roleDefinitions/b7f5ddc1-b7dc-4d37-abce-b9d6fc15ffff
Content-type: application/json

{
  "description": "Update basic properties and permission of application registrations",
  "displayName": "ExampleCustomRole",
  "rolePermissions":
    [
        {
            "allowedResourceActions": 
            [
                "Microsoft.CloudPC/CloudPCs/Read",
                "Microsoft.CloudPC/CloudPCs/Reprovision"
            ]
        }
    ]
}
```

### <a name="response"></a>响应

下面展示了示例响应。
> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
Content-type: application/json

```
