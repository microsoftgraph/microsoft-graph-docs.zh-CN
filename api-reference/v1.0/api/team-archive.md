---
title: 存档团队
description: '存档指定的团队。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6a9a2d7c3994d3b1d3e96c1c7f4d16195bb135ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961405"
---
# <a name="archive-team"></a>存档团队



存档指定的[团队](../resources/team.md)。 团队存档时，用户可以不再发送或团队中的任何频道上的邮件，类似编辑工作组的名称、 说明或其他设置，或通常对团队大多数的更改。
向团队的成员身份更改继续允许。

存档是异步操作。 一旦异步操作已成功完成，此 API 响应后可能出现的存档团队。

才能存档团队，团队和[组](../resources/group.md)必须具有一个所有者。

若要从其存档状态还原团队，使用 API 对[unarchive](team-unarchive.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Group.ReadWrite.All    |

> **注意**： 此 API 支持管理员权限。 全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。

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
在请求中，则可以_选择_包括`shouldSetSpoSiteReadOnlyForMembers`以 json 格式的参数正文，，如下所示。
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
此可选的参数定义是否与团队关联的 Sharepoint Online 网站上设置为只读的工作组成员的权限。 设置为 false 或省略正文完全将导致正在跳过此步骤。

## <a name="response"></a>响应

如果存档成功启动，此方法返回`202 Accepted`响应代码。 响应还将包含`Location`标头，其中包含已创建以处理存档的团队[teamsAsyncOperation](../resources/teamsasyncoperation.md)的位置。 通过对此位置进行 GET 请求检查存档操作的状态。

## <a name="example"></a>示例
#### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a>响应
下面是响应的示例。
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
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
