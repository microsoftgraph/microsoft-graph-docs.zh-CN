---
title: Unarchive 团队
description: 还原存档的团队。 这将还原发送消息和编辑团队，遵守租户和工作组设置用户的功能。 工作组已存档使用存档 API。
ms.openlocfilehash: 4a90be4c5b2488bf72123cabe1da3aacf856e9d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009133"
---
# <a name="unarchive-team"></a>Unarchive 团队



还原存档的[团队](../resources/team.md)。 这将还原发送消息和编辑团队，遵守租户和工作组设置用户的功能。 工作组已存档使用[存档](team-archive.md)API。

Unarchiving 是异步操作。 一旦异步操作已成功完成，此 API 响应后可能出现的团队未存档。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Group.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Group.ReadWrite.All    |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果 unarchiving 已成功启动，此方法返回`202 Accepted`响应代码。 响应还将包含`Location`标头，其中包含的[teamsAsyncOperation](../resources/teamsasyncoperation.md)创建处理 unarchiving 团队的位置。 通过对此位置进行 GET 请求检查 unarchiving 操作的状态。

## <a name="example"></a>示例
#### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a>响应
下面是响应的示例。
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
