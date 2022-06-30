---
title: 列出组织中 Microsoft Teams 的所有团队
description: 使用 Microsoft Graph 中的 Microsoft Teams API，通过查找所有拥有团队的组并获取每个团队的信息，列出组织中的所有团队。
author: nkramer
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 955d55d521d1dda3ace17943261477020f2fb935
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556141"
---
# <a name="list-all-teams-in-microsoft-teams-for-an-organization"></a>列出组织中 Microsoft Teams 的所有团队

若要列出组织（租户）中的所有[团队](/graph/api/resources/team)，请找到包含团队的所有组，然后获取每个团队的信息。

## <a name="get-a-list-of-groups"></a>获取组列表

### <a name="example-1-get-a-list-of-groups-that-contain-a-team"></a>示例 1：获取包含团队的组的列表

若要获取包含团队的组织中所有 [组](/graph/api/resources/group)的列表，请获取所有 [组的列表](/graph/api/group-list)，然后在代码中找到具有包含“Team”的 **resourceProvisioningOptions** 属性的代码。

将 API 与 `$filter`一起使用，以仅返回具有团队的组。

#### <a name="request"></a>请求

```http
GET /groups?$filter=resourceProvisioningOptions/Any(x:x eq 'Team')
```

> [!NOTE]
> 某些未使用的旧团队将不会设置 **resourceProvisioningOptions**。 有关详细信息，请参阅[已知问题](known-issues.md#properties-are-missing-in-the-list-of-teams-that-a-user-has-joined)。

#### <a name="response"></a>响应

下面介绍响应示例。 

>**注意：** 为了提高可读性，可能缩短了显示的响应对象。 
>
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
    "value": [
        {
            "id": "02bd9fd6-8f93-4758-87c3-1fb73740a315",
            "description": "Welcome to the HR Taskforce team.",
            "displayName": "HR Taskforce",
            "groupTypes": [
                "Unified"
            ],
            "mailEnabled": true,
            "mailNickname": "HRTaskforce",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [
                "Team"
            ],
            "securityEnabled": false,
            "visibility": "Private"
        },
        {
            "id": "8090c93e-ba7c-433e-9f39-08c7ba07c0b3",
            "description": "Welcome to the team that we've assembled to launch our product.",
            "displayName": "X1050 Launch Team",
            "groupTypes": [
                "Unified"
            ],
            "mailEnabled": true,
            "mailNickname": "X1050LaunchTeam",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [
                "Team"
            ],
            "securityEnabled": false,
            "visibility": "Private"
        }
    ]
}
```

### <a name="example-2-get-a-list-of-groups-by-selecting-required-properties-only"></a>示例 2：仅通过选择所需属性来获取组列表

由于组是大型对象，因此使用 `$select` 仅获取你关注的组的属性。

#### <a name="request"></a>请求

```http
GET /groups?$select=id,resourceProvisioningOptions
```

> [!NOTE]
> 某些未使用的旧团队将不会设置 **resourceProvisioningOptions**。 有关详细信息，请参阅[已知问题](known-issues.md#properties-are-missing-in-the-list-of-teams-that-a-user-has-joined)。

#### <a name="response"></a>响应

下面介绍响应示例。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups",
    "value": [
        {
            "id": "00e897b1-70ba-4cb9-9126-fd5f95c4bb78",
            "resourceProvisioningOptions": []
        },
        {
            "id": "00f6e045-f884-4359-a617-d459ee626862",
            "resourceProvisioningOptions": [
                "Team"
            ]
        }
    ]
}

```

## <a name="get-team-information-for-a-group"></a>获取组的团队信息

若要获取特定组中团队的团队信息，请调用[获取团队](/graph/api/team-get) API 并包括组 ID。

### <a name="request"></a>请求

```http
GET /teams/{group-id}
```

### <a name="response"></a>响应

以下示例显示了相应的响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "isArchived" : false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true    
  },
  "guestSettings": {
    "allowCreateUpdateChannels": true,
    "allowDeleteChannels": true 
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
    "giphyContentRating": "strict",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```

## <a name="see-also"></a>另请参阅

- [列出 joinedTeams](/graph/api/user-list-joinedteams)
- [列出组](/graph/api/group-list)
- [Microsoft Teams API 概述](teams-concept-overview.md)