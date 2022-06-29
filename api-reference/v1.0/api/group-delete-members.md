---
title: 删除成员
description: 通过成员导航属性从组中删除成员。
ms.localizationpriority: high
author: psaffaie
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3f8ee44072ca62dd00f2e497b2c29310dac6c0c0
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439291"
---
# <a name="remove-member"></a>删除成员

命名空间：microsoft.graph

通过 **成员** 导航属性从组中删除成员。 你不能从具有动态成员身份的组中删除成员。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                             |
| :------------------------------------- | :---------------------------------------------------------------------- |
| 委派（工作或学校帐户）     | GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。                                                          |
| 应用程序                            | GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All |

> [!IMPORTANT]
> 若要从可分配角色的组中删除成员，还必须向调用用户或应用分配 _RoleManagement.ReadWrite.Directory_ 权限。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/members/{id}/$ref
```
> [!CAUTION]
> 如果未将 `/$ref` 追加到请求中，并且调用应用有权管理成员对象类型，则也会从 Azure Active Directory (Azure AD) 中删除成员对象；否则，将返回 `403 Forbidden` 错误。 例如，同时具有 *GroupMember.ReadWrite.All* 和 *User.ReadWrite.All* 权限的应用将删除用户。 可以通过 [还原已删除的项 API](directory-deleteditems-restore.md) 还原特定对象。

## <a name="request-headers"></a>请求头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "delete_member_from_group"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/groups/{group-id}/members/{directory-object-id}/$ref
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-member-from-group-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/delete-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-member-from-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-member-from-group-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

在请求中，指定组的标识符和要删除目录对象的标识符。

#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
