---
title: 列出 allowedMembers
description: 从 allowedMembers 导航属性获取 conversationMember 资源列表。
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: eae5653a68d72d8ec68ad3eb81d96bc192c3f90a
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060855"
---
# <a name="list-allowedmembers"></a>列出 allowedMembers
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取可以访问共享的[频道](../resources/channel.md)的 [conversationMembers](../resources/conversationmember.md) 列表。

此方法不从[团队](../resources/team.md)返回以下 [conversationMembers](../resources/conversationmember.md)：
- 具有 `Guest` 角色的用户
- 在租户中进行外部身份验证的用户

> [!NOTE]
> 服务器返回的成员 ID 必须作为不透明的字符串处理。 客户端不应尝试对此 ID 进行分析或做出任何假设。
>
> 未来，成员资格结果可以映射到来自不同租户的用户，如响应中所示。客户端不应假定所有成员仅来自当前租户。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户） | ChannelMember.Read.All、 ChannelMember.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | ChannelMember.Read.All、 ChannelMember.ReadWrite.All |


> **注意**：此 API 支持管理员权限。全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/channels/{channel-id}/sharedWithTeams/{shared-with-channel-team-info-id}/allowedMembers
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持使用 `$select` 和 `$count` [OData 查询参数](/graph/query-parameters)自定义响应。

## <a name="request-headers"></a>请求头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationMember](../resources/conversationmember.md) 对象的集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "list_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/893075dd-2487-5634-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/sharedWithTeams/893075dd-2487-5634-925f-022c42e20265/allowedMembers
```


### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.conversationMember",
      "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkMTQ",
      "roles": [
        "owner"
      ],
      "displayName": "Eric Solomon",
      "userId": "eef9cb36-06de-469b-87cd-70f4cbe32d14",
      "email": "ericsol@fabrikam.com",
      "tenantId": "df81db53-c7e2-418a-8803-0e68d4b88607"
    },
    
    {
      "@odata.type": "#microsoft.graph.conversationMember",
      "id": "MmFiOWMFxTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkMTQ",
      "roles": [
        "user"
      ],
      "displayName": "Caleb Foster",
      "userId": "eef9cb36-06de-469b-87cd-70f4cbe32d14",
      "email": "calfos@fabrikam.com",
      "tenantId": "df81db53-c7e2-418a-8803-0e68d4b88607"
    }
  ]
}
```

## <a name="see-also"></a>另请参阅

- [列出团队成员](team-list-members.md)
