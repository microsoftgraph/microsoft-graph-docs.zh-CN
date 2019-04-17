---
title: 存档团队
description: '将指定的团队存档。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a009dc7214627575b00b2537875e5561b0515d32
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889917"
---
# <a name="archive-team"></a>存档团队

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将指定的[团队](../resources/team.md)存档。 存档团队后, 用户将无法再发送或赞邮件在团队中的任何频道上, 编辑团队的名称、说明或其他设置, 或者通常对团队做出大多数更改。
仍允许对团队进行成员资格更改。

存档是一种异步操作。 一旦异步操作成功完成, 则会存档团队, 这可能会在此 API 响应之后发生。

为了存档团队, 团队和[组](../resources/group.md)必须具有所有者。

若要从存档状态还原团队, 请使用 API[接档](team-unarchive.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Group.ReadWrite.All    |

> **注意**：此 API 支持管理员权限。 全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。

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
在请求中, 可以_选择_将`shouldSetSpoSiteReadOnlyForMembers`参数包含在 JSON 正文中, 如下所示。
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
此可选参数定义是否在与团队关联的 Sharepoint Online 网站上将工作组成员的权限设置为只读。 将其设置为 false 或完全省略正文将导致跳过此步骤。

## <a name="response"></a>响应

如果成功启动存档, 此方法将`202 Accepted`返回响应代码。 该响应还将包含一个`Location`标头, 其中包含为处理团队存档而创建的[teamsAsyncOperation](../resources/teamsasyncoperation.md)的位置。 通过向此位置发出 GET 请求, 检查存档操作的状态。

## <a name="example"></a>示例
#### <a name="request"></a>请求
以下是请求的示例。
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a>响应
下面是响应的一个示例。
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-archive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
