---
title: 列出 associatedTeamInfo
description: 获取与用户关联的Microsoft Teams中的团队列表。
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 16842866ca4c2b03268e80eb838bbf953844c605
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685262"
---
# <a name="list-associatedteaminfo"></a>列出 associatedTeamInfo
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取[与用户](../resources/user.md)关联的Microsoft Teams中的[团队](../resources/associatedteaminfo.md)列表。
目前， [用户](../resources/user.md) 可以通过两种不同的方式与 [团队](../resources/team.md) 关联：
* [用户](../resources/user.md)可以是[团队](../resources/team.md)的直接成员。
* [用户](../resources/user.md)可以是托管在[团队](../resources/team.md)中的共享[频道](../resources/channel.md)的成员。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户） | Team.ReadBasic.All，TeamSettings.Read.All，TeamSettings.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Team.ReadBasic.All，TeamSettings.Read.All，TeamSettings.ReadWrite.All|

> **注意：** 目前，使用用户委派的权限时，此操作仅适用于“`me`”用户。 使用应用程序权限时，此操作通过指定特定用户 ID 而适用于所有用户 ID。（使用应用程序权限时，不支持“`me`”别名）。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{user-id}/teamwork/associatedTeams
```

## <a name="optional-query-parameters"></a>可选的查询参数
此运营商当前不支持通过 [OData 查询参数](/graph/query-parameters) 来自定义响应。

## <a name="request-headers"></a>请求头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [关联TeamInfo](../resources/associatedteaminfo.md) 对象的集合。

> **注意**：此 API 还返回用户是其直接成员的共享通道的主机团队。

## <a name="examples"></a>示例

### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "request",
  "name": "list_associatedteaminfo"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/teamwork/associatedTeams
```


### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.associatedTeamInfo",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.associatedTeamInfo",
      "id": "b695c5a5-c5a5-b695-a5c5-95b6a5c595b6",
      "tenantId": "172b0cce-e65d-7hd4-9a49-91d9f2e8493a",
      "displayName": "Contoso Team"
    },
    {
      "@odata.type": "#microsoft.graph.associatedTeamInfo",
      "id": "b695c5a5-8934-b695-a5c5-95b6a5c595b6",
      "tenantId": "172b0cce-8961-7hd4-9a49-91d9f2e8493a",
      "displayName": "Fabrikam Team"
    }
  ]
}
```


## <a name="see-also"></a>另请参阅

- [列出 joinedTeams](../api/user-list-joinedteams.md)
- [列出组织中的所有团队](../api/teams-list.md)
- [获取团队](../api/team-get.md)

