---
title: 添加成员
description: 通过 members 导航属性将成员添加到 Microsoft 365 组或安全组中。
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d243dc2aed3604aa6777eb29a4606e42134c0462
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2022
ms.locfileid: "64848697"
---
# <a name="add-members"></a>添加成员

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过 **members** 导航属性将成员添加到安全组或 Microsoft 365 组中。

下表显示了可添加到安全组或Microsoft 365组的成员类型。


| 对象类型          | 安全组的成员     | Microsoft 365组的成员 |
|----------------------|-------------------------------|-------------------------------|
| 用户                | ![可以是组成员][Yes]   | ![可以是组成员][Yes]   |
| 安全组      | ![可以是组成员][Yes]   | ![不能是组成员][No] |
| Microsoft 365 组 | ![不能是组成员][No] | ![不能是组成员][No] |
| 设备              | ![可以是组成员][Yes]   | ![不能是组成员][No] |
| 服务主体   | ![可以是组成员][Yes]   | ![不能是组成员][No] |


## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                             |
| :------------------------------------- | :---------------------------------------------------------------------- |
| 委派（工作或学校帐户）     | GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。                                                          |
| 应用程序                            | GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All |

> [!IMPORTANT]
> 若要将成员添加到可分配角色的组，还必须向调用用户或应用分配 _RoleManagement.ReadWrite.Directory_ 权限。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。 它不会在响应正文中返回任何内容。 当对象已是组的成员时，此方法将返回 `400 Bad Request` 响应代码。 当添加的对象不存在时，此方法返回 `404 Not Found` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{group-id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```

# <a name="javascript"></a>[JavaScript](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/add-group-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](../includes/snippets/java/add-group-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)

[!INCLUDE [sample-code](../includes/snippets/go/add-group-member-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)

[!INCLUDE [sample-code](../includes/snippets/powershell/add-group-member-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

在请求正文中，提供要添加的 `id` [directoryObject](../resources/directoryobject.md)、 [用户](../resources/user.md)或 [组](../resources/group.md) 对象的 JSON 表示形式。

### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>另请参阅

- [添加成员至团队](team-post-members.md)
- [更新成员在团队中的角色](team-update-members.md)
- [从团队删除成员](team-delete-members.md)



[Yes]: /graph/images/yesandnosymbols/greencheck.svg
[No]: /graph/images/yesandnosymbols/no.svg

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
