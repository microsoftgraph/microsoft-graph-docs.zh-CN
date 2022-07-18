---
title: group：assignLicense
description: 添加或删除组上的许可证。 分配给组的许可证将分配给组中的所有用户。
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 46b1f78f3341fcd06bb0c2cf592aa8b6c6ceda4b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210722"
---
# <a name="group-assignlicense"></a>group：assignLicense

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

添加或删除组上的许可证。 分配给组的许可证将分配给组中的所有用户。 若要详细了解基于组的许可，请参阅[Azure Active Directory中基于组的许可](/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal)。

若要获取目录中可用的订阅，请执行 [GET subscribedSkus 请求](subscribedsku-list.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）  |
| :------------------------------------- | :------------------------------------------- |
| 委派（工作或学校帐户）     | Group.ReadWrite.All, Directory.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。                               |
| 应用程序                            | Group.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/assignLicense
```

## <a name="request-headers"></a>请求标头

| 标头        | 值                       |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数      | 类型                                                          | 说明                                                                                                                                                                                                                                                                    |
| :------------- | :------------------------------------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| addLicenses    | [assignedLicense](../resources/assignedlicense.md) collection | 用于指定要添加的许可证的 [assignedLicense](../resources/assignedlicense.md) 对象集合。 可以通过在 [assignedLicense](../resources/assignedlicense.md) 对象上设置 disabledPlans 属性来禁用与许可证关联的 **servicePlans**。 |
| removeLicenses | Guid 集合                                               | 标识要删除的许可证的 skuId 的集合。                                                                                                                                                                                                                   |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `202 Accepted` 响应代码和目标 [组](../resources/group.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-add-licenses-to-the-group"></a>示例 1：向组添加许可证

以下示例将许可证添加到组。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "group_assignlicense"
}-->

```http
POST https://graph.microsoft.com/beta/groups/1132b215-826f-42a9-8cfe-1643d19d17fd/assignLicense
Content-type: application/json

{
  "addLicenses": [
    {
      "disabledPlans": [
        "113feb6c-3fe4-4440-bddc-54d774bf0318",
        "14ab5db5-e6c4-4b20-b4bc-13e36fd2227f"
      ],
      "skuId": "b05e124f-c7cc-45a0-a6aa-8cf78c946968"
    },
    {
      "disabledPlans": [
        "a413a9ff-720c-4822-98ef-2f37c2a21f4c"
      ],
      "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df"
    }
  ],
  "removeLicenses": []
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-assignlicense-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/group-assignlicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-assignlicense-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/group-assignlicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-assignlicense-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/group-assignlicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-assignlicense-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/group-assignlicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-assignlicense-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/group-assignlicense-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/group-assignlicense-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/group-assignlicense-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

响应是更新后的组对象。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json
location: https://graph.microsoft.com/v2/e8e96c2a-d787-4eb1-98d7-9e57c965f1de/directoryObjects/1132b215-826f-42a9-8cfe-1643d19d17fd/Microsoft.DirectoryServices.Group

{
  "id": "1132b215-826f-42a9-8cfe-1643d19d17fd",
  "createdDateTime": "2021-03-12T11:15:03Z",
  "groupTypes": [],
  "securityEnabled": true,
}
```

### <a name="example-2-remove-licenses-from-the-group"></a>示例 2：从组中删除许可证

以下示例从组中删除许可证。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "group_removelicense"
}-->

```http
POST https://graph.microsoft.com/beta/groups/1132b215-826f-42a9-8cfe-1643d19d17fd/assignLicense
Content-type: application/json

{
  "addLicenses": [],
  "removeLicenses": [
    "c7df2760-2c81-4ef7-b578-5b5392b571df",
    "b05e124f-c7cc-45a0-a6aa-8cf78c946968"
  ]
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removelicense-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removelicense-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removelicense-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removelicense-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removelicense-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/group-removelicense-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-removelicense-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/group-removelicense-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-removelicense-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/group-removelicense-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/group-removelicense-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/group-removelicense-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

响应是更新后的组对象。

> **注意：** 此处显示的响应对象可能会缩短可读性。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json
location: https://graph.microsoft.com/v2/e8e96c2a-d787-4eb1-98d7-9e57c965f1de/directoryObjects/1132b215-826f-42a9-8cfe-1643d19d17fd/Microsoft.DirectoryServices.Group

{
  "id": "1132b215-826f-42a9-8cfe-1643d19d17fd",
  "createdDateTime": "2021-03-12T11:15:03Z",
  "groupTypes": [],
  "securityEnabled": true,
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: assignLicense",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
