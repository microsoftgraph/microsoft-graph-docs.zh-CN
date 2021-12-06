---
title: 存档团队
description: '存档指定的团队。 '
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ed4457a55c96b33faae433dc47e2be43f7951ebe
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032822"
---
# <a name="archive-team"></a>存档团队

命名空间：microsoft.graph

将指定[团队](../resources/team.md)存档。存档团队后，用户将无法再在团队中的任意频道中发送或点赞消息，无法再编辑团队名称、说明和其他设置，且通常也无法再对团队进行大部分更改。将继续允许对团队进行成员身份更改。

存档是异步操作。该异步操作成功完成后，团队即已存档，此 API 作出响应后就可能出现此情况。

要对团队存档，团队和[组](../resources/group.md)都必须有一个所有者。

要从存档状态还原团队，请使用 API [取消存档](team-unarchive.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | TeamSettings.ReadWrite.All，Group.ReadWrite.All **，Directory.ReadWrite.All** |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | TeamSettings.ReadWrite.Group *、TeamSettings.ReadWrite.All、Group.ReadWrite.All**、Directory.ReadWrite.All** |

> **注意**：标有 * 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。 标记为 **的权限已弃用，不应使用。

> **注意**：此 API 支持管理员权限。全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
在请求中，可 _选择性地_ 在 JSON 正文中包括 `shouldSetSpoSiteReadOnlyForMembers` 参数，如下所示。
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
此可选参数定义了是否在与团队关联的 SharePoint Online 网站上将团队成员的权限设置为“只读”。 如果将其设置为 false 或完全省略正文，将导致跳过此步骤。

>[!IMPORTANT]
>应用程序上下文不支持 `shouldSetSpoSiteReadOnlyForMembers` 参数。

## <a name="response"></a>响应

如果成功开始存档，此方法将返回一个 `202 Accepted` 响应代码。 响应还将包含一个 `Location` 标头，后者包含创建用于处理团队存档操作的 [teamsAsyncOperation](../resources/teamsasyncoperation.md) 的位置。 可通过向此位置发出 GET 请求，查看存档操作的状态。

## <a name="example"></a>示例
#### <a name="request"></a>请求
请求示例如下所示。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/archive
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/archive-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/archive-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/archive-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/archive-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/archive-team-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应
响应示例如下所示。

<!-- {
  "blockType": "response",
  "name": "archive_team"
}-->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

