---
title: 更新 unifiedRoleDefinition
description: 更新 unifiedRoleDefinition 对象的属性。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: bd7ceb47c3a1d95264405a3d72ef140742c63933
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61008488"
---
# <a name="update-unifiedroledefinition"></a>更新 unifiedRoleDefinition

命名空间：microsoft.graph

更新 [unifiedRoleDefinition 对象](../resources/unifiedroledefinition.md) 的属性。 无法更新内置角色。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | RoleManagement.ReadWrite.Directory |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | RoleManagement.ReadWrite.Directory |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a>请求标头
    
| 名称       | 说明|
|:-----------|:-----------|
| Authorization | 持有者 {token} |
| Content-Type | application/json. Required. |
    
## <a name="request-body"></a>请求正文
    
在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为获得最佳性能，请勿包含尚未更改的现有值。
    
下表显示更新 [unifiedRoleDefinition](../resources/unifiedroledefinition.md)时所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|String| 角色定义的说明。 **isBuiltIn** 为 时为只读 `true` 。 |
|displayName|String| 角色显示名称的角色定义。 **isBuiltIn** 为 时为只读 `true` 。 必需。|
|isEnabled|Boolean| 指示角色是否已启用分配的标志。 如果 `false` 为 ，则角色不可用于分配。 **isBuiltIn** 为 true 时为只读。 |
|resourceScopes|String collection| 角色定义适用的作用域和权限列表。 当前仅 `/` 受支持。 **isBuiltIn** 为 true 时为只读。 **请勿使用。此属性将很快弃用。将作用域附加到角色分配。**|
|rolePermissions|[unifiedRolePermission](../resources/unifiedrolepermission.md) 集合| 角色中包含的权限列表。 **isBuiltIn** 为 时为只读 `true` 。 必需。 |
|templateId|String| 可在 **isBuiltIn** 为 时设置的自定义模板标识符 `false` 。 如果一个标识符在不同目录之间需要相同，则通常使用此标识符。 **isBuiltIn** 为 时为只读 `true` 。 |
|version|String| 指示角色定义的版本。 **isBuiltIn** 为 时为只读 `true` 。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/roleManagement/directory/roleDefinitions/0d55728d-3e24-4309-9b1b-5ac09921475a
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-unifiedroledefinition-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 OK
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

