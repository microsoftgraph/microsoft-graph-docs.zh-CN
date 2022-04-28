---
title: Delete sharedWithChannelTeamInfo
description: 从共享频道中删除团队。
author: devjha-ms
doc_type: apiPageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 899bc9a9b60f1d7bb8bba8fec89e2bd311be7bae
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060568"
---
# <a name="delete-sharedwithchannelteaminfo"></a>Delete sharedWithChannelTeamInfo
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过删除相应的 [sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md) 资源，取消与[团队](../resources/team.md)共享[频道](../resources/channel.md)。 此操作仅允许 **membershipType** 值为 `shared` 的频道。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户） | ChannelMember.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | ChannelMember.ReadWrite.All |


> **注意**：此 API 支持管理员权限。全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/channels/{channel-id}/sharedWithTeams/{shared-with-channel-team-info-id}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "request",
  "name": "delete_sharedwithchannelteaminfo"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/sharedWithTeams/ece6f0a1-5g39-498b-be79-edf6c8fc4d82
```


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>另请参阅

- [从频道中删除成员](channel-delete-members.md)
- [从团队删除成员](team-delete-members.md)
