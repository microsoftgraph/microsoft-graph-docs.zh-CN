---
title: 更新 unifiedRoleDefinition
description: 更新 unifiedRoleDefinition 对象的属性。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 38ab5c03693978cf62725b5d680f24a323f602d4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444761"
---
# <a name="update-unifiedroledefinition"></a>更新 unifiedRoleDefinition

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [unifiedRoleDefinition 对象](../resources/unifiedroledefinition.md) 的属性。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | RoleManagement.ReadWrite.Directory |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | RoleManagement.ReadWrite.Directory |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
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
|displayName|String| 角色显示名称的定义。 isBuiltIn 为 true 时为只读。 必需。|
|id|String| 角色定义的唯一标识符。 键，不可为 null，只读。 |
|isBuiltIn|Boolean| 指示角色定义是产品或自定义中包含的默认集的一部分的标志。 只读。 |
|isEnabled|Boolean| 指示是否已启用角色分配的标志。 如果为 false，则角色不能用于分配。 isBuiltIn 为 true 时为只读。 |
|resourceScopes|String collection| 角色定义授予的范围权限列表适用。 当前仅支持"/"。 isBuiltIn 为 true 时为只读。 **请勿使用。此属性将很快弃用。将作用域附加到角色分配。**|
|rolePermissions|[unifiedRolePermission](../resources/unifiedrolepermission.md) 集合| 角色中包含的权限列表。 isBuiltIn 为 true 时为只读。 必需。 |
|templateId|String| IsBuiltIn 为 false 时可设置的自定义模板标识符。 如果不同目录的标识符需要相同，则通常使用此标识符。 isBuiltIn 为 true 时为只读。 |
|inheritsPermissionsFrom| [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 集合| 给定角色定义从其继承的角色定义的只读集合。 只有 Azure AD 内置角色支持此属性。 |
|version|String| 指示角色定义的版本。 isBuiltIn 为 true 时为只读。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。


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

---


### <a name="response"></a>响应

下面展示了示例响应。
> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
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


