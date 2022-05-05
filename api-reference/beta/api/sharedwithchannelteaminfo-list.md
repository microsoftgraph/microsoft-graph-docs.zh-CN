---
title: 列出 sharedWithChannelTeamInfo
description: 获取已与频道共享的团队列表。
author: devjha-ms
doc_type: apiPageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: e57444da50bd0fbbd844b71e4a4ed6c5c914d3a4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212792"
---
# <a name="list-sharedwithchannelteaminfo"></a>列出 sharedWithChannelTeamInfo
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取已共享指定[频道](../resources/channel.md)的[团队](../resources/sharedwithchannelteaminfo.md)列表。 此操作仅允许 **membershipType** 值为 `shared` 的频道。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|ChannelMember.Read.All、 ChannelMember.ReadWrite.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|ChannelMember.Read.All、 ChannelMember.ReadWrite.All |

> **注意**：此 API 支持管理员权限。全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/channels/{channel-id}/sharedWithTeams
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持`$filter` 和 `$select` [OData 查询参数](/graph/query-parameters)，以帮助自定义响应。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和响应主体中的 [sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_sharedwithchannelteaminfo"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/sharedWithTeams
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-sharedwithchannelteaminfo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-sharedwithchannelteaminfo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-sharedwithchannelteaminfo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-sharedwithchannelteaminfo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-sharedwithchannelteaminfo-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-sharedwithchannelteaminfo-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
下面展示了示例响应。
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.sharedWithChannelTeamInfo",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sharedWithChannelTeamInfo",
      "id": "2173de69-de69-2173-69de-732169de7321",
      "tenantId": "b3246f44-b4gb-4627-96c6-25b18fa2c910",
      "displayName": "Team Contosso",
      "isHostTeam": true
    },
    {
      "@odata.type": "#microsoft.graph.sharedWithChannelTeamInfo",
      "id": "893075dd-2487-4122-86db-022c42e20265",
      "displayName": "Team fabricam",
      "isHostTeam": false,
      "tenantId": "b3246f44-b4gb-5678-96c6-25b18fa2c910"
    }
  ]
}
```

