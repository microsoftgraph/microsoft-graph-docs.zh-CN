---
title: 获取 teamDefinition
description: 获取与 teamTemplateDefinition 对象关联的团队的属性。
author: Charlieforce
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 6b2b588ea46c3b47b13e36a7449f63fdaed3f674
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690116"
---
# <a name="get-teamdefinition"></a>获取 teamDefinition
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取与 [teamTemplateDefinition](../resources/teamstemplate.md) 对象关联的[团队](../resources/team.md)的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Team.Create|
|委派（个人 Microsoft 帐户）|不支持|
|Application|Team.Create|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teamwork/teamTemplates/{teamTemplateId}/definitions/{teamTemplateDefinitionId}/teamDefinition
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [team](../resources/team.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。

<!-- {
  "blockType": "request",
  "name": "get_teamtemplate/teamDefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/teamTemplates/com.microsoft.teams.template.ManageAProject/definitions/Y29tLm1pY3Jvc29mdC50ZWFtcy50ZW1wbGF0ZS5NYW5hZ2VBUHJvamVjdCMjUHVibGljIyNlbi1VUw==/teamDefinition
```

### <a name="response"></a>响应
下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "com.microsoft.teams.template.ManageAProject.Team",
    "createdDateTime": null,
    "displayName": "Manage a Project",
    "description": "Manage tasks, share documents, conduct project meetings and document risks and decisions with this template for general project management.",
    "internalId": null,
    "classification": null,
    "specialization": "none",
    "visibility": "private",
    "webUrl": null,
    "isArchived": null,
    "tenantId": null,
    "isMembershipLimitedToOwners": null,
    "summary": null,
    "memberSettings": {
        "allowCreateUpdateChannels": true,
        "allowCreatePrivateChannels": true,
        "allowDeleteChannels": true,
        "allowAddRemoveApps": true,
        "allowCreateUpdateRemoveTabs": true,
        "allowCreateUpdateRemoveConnectors": true
    },
    "guestSettings": {
        "allowCreateUpdateChannels": false,
        "allowDeleteChannels": false
    },
    "messagingSettings": {
        "allowUserEditMessages": true,
        "allowUserDeleteMessages": true,
        "allowOwnerDeleteMessages": true,
        "allowTeamMentions": true,
        "allowChannelMentions": true
    },
    "funSettings": {
        "allowGiphy": true,
        "giphyContentRating": "moderate",
        "allowStickersAndMemes": true,
        "allowCustomMemes": true
    },
    "discoverySettings": {
        "showInTeamsSearchAndSuggestions": true
    }
}
```
