---
title: 获取频道中的选项卡
description: '检索指定选项卡的属性和关系。 '
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d169ae0e5a19b0c778be44bccf1652446d29bc4f
ms.sourcegitcommit: 4c8444b732b8d6d0de8a95f6666c42095f146266
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/08/2022
ms.locfileid: "62443084"
---
# <a name="get-tab"></a>获取选项卡

命名空间：microsoft.graph



检索团队中频道[中](../resources/teamstab.md)指定[选项卡的属性和](../resources/channel.md)[关系](../resources/team.md)。 

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | TeamsTab.Read.All、TeamsTab.ReadWriteForTeam、TeamsTab.ReadWrite.All、Group.Read.All、**Group.ReadWrite.All**、Directory.Read.All、**Directory.ReadWrite.All** |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | TeamsTab.Read.Group、*TeamsTab.ReadWrite.Group*、TeamsTab.Read.All、TeamsTab.ReadWriteForTeam.All、TeamsTab.ReadWrite.All、**Group.Read.All、Group.ReadWrite.All**、Directory.Read.All、**Directory.ReadWrite.All** |

> **注意**：标记为 ** 的权限仅支持向后兼容。 建议您将解决方案更新为使用不同的权限，并避免今后使用这些权限。 标有 * 的权限使用 [特定于资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)。

> **注意**：此 API 支持管理员权限。全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。

## <a name="http-request"></a>HTTP 请求
```http
GET /teams/{team-id}/channels/{channel-id}/tabs/{tab-id}
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 $select 和 $expand [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [tab](../resources/teamstab.md) 对象。
## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}?$expand=teamsApp
```
### <a name="response"></a>响应
下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "tabId",
  "displayName": "My Contoso Tab - updated",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "teamsApp": {
      "id": "0d820ecd-def2-4297-adad-78056cde7c78",
      "externalId": null,
      "displayName": "Contoso",
      "distributionMethod": "store"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a channel tab",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

