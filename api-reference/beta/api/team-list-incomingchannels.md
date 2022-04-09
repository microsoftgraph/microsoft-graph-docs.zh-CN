---
title: 列出 incomingChannels
description: 获取传入频道列表。
author: devjha-ms
doc_type: apiPageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 4e664f4460b46c76cb1aeb6ccded0812feadfa66
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704242"
---
# <a name="list-incomingchannels"></a>列出 incomingChannels
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取传入 [频道](../resources/channel.md)（与[团队](../resources/team.md)共享的频道）列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户） | Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Channel.ReadBasic.All、ChannelSettings.Read.All、ChannelSettings.ReadWrite.All |

> **注意**：此 API 支持管理员权限。全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/incomingChannels
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

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和响应主体中的 [频道](../resources/channel.md) 对象集合。 响应还包括 **@odata.id** 属性，可用于访问频道并在 [频道](../resources/channel.md) 对象上运行其他操作。

> [!Note]
> 目前，调用 **@odata.id** 属性返回的 URL 对跨租户共享频道失败。 如果在调用此 API 之前从 URL 中删除 `/tenants/{tenant-id}` 部件，则可以解决此问题。 有关详细信息，请参阅 [Microsoft Graph 的已知问题](/graph/known-issues#unable-to-access-a-cross-tenant-shared-channel-when-the-request-url-contains-tenantscross-tenant-id)。

## <a name="examples"></a>示例

### <a name="request"></a>请求
下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "list_channel"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/incomingChannels
```


### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.id": "https://graph.microsoft.com/beta/tenants/b3246f44-b4gb-4627-96c6-25b18fa2c910/teams/893075dd-5678-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
      "id": "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
      "createdDateTime": "2020-05-27T19:22:25.692Z",
      "displayName": "Contoso Sales channel",
      "description": "channel created in Contoso to be shared with other teams/tenants.",
      "membershipType": "shared",
      "tenantId": "b3246f44-b4gb-4627-96c6-25b18fa2c910"
    }
  ]
}
```

