---
title: 列出 joinedTeams
description: 获取用户不是其直接成员的 Microsoft Teams 团队。
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5e4e4079bf3e7002ed84797f0989fb66c0326484
ms.sourcegitcommit: 4c8444b732b8d6d0de8a95f6666c42095f146266
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/08/2022
ms.locfileid: "62442867"
---
# <a name="list-joinedteams"></a>列出 joinedTeams

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取用户不是其直接成员的 Microsoft Teams [团队](../resources/team.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Team.ReadBasic.All、TeamSettings.Read.All、TeamSettings.ReadWrite.All、User.Read.All、User.ReadWrite.All、Directory.Read.All **、Directory.ReadWrite.All** |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Team.ReadBasic.All、TeamSettings.Read.All、TeamSettings.ReadWrite.All、User.Read.All、User.ReadWrite.All、Directory.Read.All **、Directory.ReadWrite.All** |

> **Note**： 仅支持使用 ** 标记的权限以实现向后兼容。 我们建议你更新解决方案以使用不同的权限，并避免今后使用这些权限。

> **注意：** 目前，使用用户委派的权限时，此操作仅适用于“`me`”用户。 使用应用程序权限时，此操作通过指定特定用户 ID 而适用于所有用户 ID。（使用应用程序权限时，不支持“`me`”别名）。 有关详细信息，请参阅[已知问题](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview)。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
GET /users/{id | user-principal-name}/joinedTeams
```

## <a name="optional-query-parameters"></a>可选的查询参数
此运营商当前不支持通过 [OData 查询参数](/graph/query-parameters) 来自定义响应。

## <a name="request-headers"></a>请求头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| 接受  | application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [团队](../resources/team.md) 对象集合。

> [!Note]
> 目前，此 API 调用仅返回 [团队](../resources/team.md)的 **id**、**displayName** 和 **说明** 属性。 若要获取所有属性，请使用[获取团队](../api/team-get.md)操作。 有关详细信息，请参阅[已知问题](/graph/known-issues#unable-to-return-all-values-for-properties-for-a-user-joined-teams)。

## <a name="example"></a>示例
### <a name="request"></a>请求
以下示例显示了一个请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/joinedTeams
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-joinedteams-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-joinedteams-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-joinedteams-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-joinedteams-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-joinedteams-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-joinedteams-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应
以下示例显示了相应的响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "172b0cce-e65d-44ce-9a49-91d9f2e8493a",
      "displayName": "Contoso Team",
      "description": "This is a Contoso team, used to showcase the range of properties supported by this API"
    }
  ]
}
```

## <a name="see-also"></a>另请参阅
- [列出所有团队](/graph/teams-list-all-teams)
- [获取团队](../api/team-get.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
