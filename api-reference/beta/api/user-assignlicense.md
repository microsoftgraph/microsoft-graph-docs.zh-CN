---
title: assignLicense
description: 为用户添加或删除许可证以启用或禁用其使用 Microsoft 云产品/服务。 例如，组织可以拥有包含 100 个许可证的 Microsoft 365 企业版 E3 订阅，此请求将其中一个许可证分配给特定用户。 还可以启用和禁用与订阅相关的特定计划。 若要详细了解订阅和许可证，请参阅此 Technet 文章。
ms.localizationpriority: medium
author: jconley76
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 5c84288339cc6f59e11dcf4ea7318d83b5621612
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549510"
---
# <a name="user-assignlicense"></a>用户：assignLicense

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为用户添加或删除许可证以启用或禁用其使用 Microsoft 云产品/服务。 例如，组织可以拥有包含 100 个许可证的 Microsoft 365 企业版 E3 订阅，此请求将其中一个许可证分配给特定用户。 还可以启用和禁用与订阅相关的特定计划。 若要详细了解订阅和许可证，请参阅此 [Technet 文章](/microsoft-365/enterprise/subscriptions-licenses-accounts-and-tenants-for-microsoft-cloud-offerings)。

若要获取目录中可用的订阅，请执行 [GET subscribedSkus 请求](subscribedsku-list.md)。 

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.ReadWrite.All、Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | User.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/assignLicense
```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|addLicenses|[assignedLicense](../resources/assignedlicense.md) collection|用于指定要添加的许可证的 [assignedLicense](../resources/assignedlicense.md) 对象集合。 可以通过在 [assignedLicense](../resources/assignedlicense.md) 对象上设置 disabledPlans 属性来禁用与许可证关联的 **servicePlans**。|
|removeLicenses|Guid 集合|标识要删除的许可证的 skuId 的集合。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新后的 [用户](../resources/user.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-assign-licenses-to-the-signed-in-user"></a>示例 1：将许可证分配给已登录用户

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}-->
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json

{
    "addLicenses": [
        {
            "disabledPlans": [
                "8a256a2b-b617-496d-b51b-e76466e88db0"
            ],
            "skuId": "84a661c4-e949-4bd2-a560-ed7766fcaf2b"
        },
        {
            "disabledPlans": [],
            "skuId": "f30db892-07e9-47e9-837c-80727f46fd3d"
        }
    ],
    "removeLicenses": []
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-assignlicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-assignlicense-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/user-assignlicense-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled": true,
  "assignedLicenses": [
        {
            "disabledPlans": [
                "8a256a2b-b617-496d-b51b-e76466e88db0"
            ],
            "skuId": "84a661c4-e949-4bd2-a560-ed7766fcaf2b"
        },
        {
            "disabledPlans": [],
            "skuId": "f30db892-07e9-47e9-837c-80727f46fd3d"
        }
    ],
  "city": "Nairobi",
  "companyName": "Contoso"
}
```

### <a name="example-2-remove-licenses-from-the-signed-in-user"></a>示例 2：从登录用户中删除许可证

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_assignlicense_removelicenses"
}-->
```http
POST https://graph.microsoft.com/beta/me/assignLicense
Content-type: application/json

{
    "addLicenses": [],
    "removeLicenses": [
        "f30db892-07e9-47e9-837c-80727f46fd3d",
        "84a661c4-e949-4bd2-a560-ed7766fcaf2b"
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-assignlicense-removelicenses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-assignlicense-removelicenses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-assignlicense-removelicenses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-assignlicense-removelicenses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-assignlicense-removelicenses-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/user-assignlicense-removelicenses-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled": true,
  "assignedLicenses": [],
  "city": "Nairobi",
  "companyName": "Contoso"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
