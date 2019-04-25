---
title: 创建包含 Microsoft Teams 团队的组
description: '若要创建包含团队的组，请按以下两步操作： '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 06b25a6da159030407c904622ffebde09c704d98
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549018"
---
# <a name="creating-a-group-with-a-microsoft-teams-team"></a>创建包含 Microsoft Teams 团队的组

若要创建包含[团队](/graph/api/resources/team?view=graph-rest-beta)的[组](/graph/api/resources/group?view=graph-rest-beta)，请按以下两步操作： 

- 使用正确属性[创建组](/graph/api/group-post-groups?view=graph-rest-beta)。
- [将团队添加](/graph/api/team-put-teams?view=graph-rest-beta)到组。

## <a name="create-a-group"></a>创建组

若要添加团队，必须设置以下属性值，如下面的示例所示：

- **groupTypes** = { "Unified" } 
- **mailEnabled** = true
- **securityEnabled** = false

```http
POST /groups
{
    "displayName":"Flight 157",
    "mailNickname":"flight157",
    "description":"Everything about flight 157",
    "visibility":"Private",
    "groupTypes":["Unified"],
    "mailEnabled":true,
    "securityEnabled":false,
    "members@odata.bind":[
        "https://graph.microsoft.com/v1.0/users/bec05f3d-a818-4b58-8c2e-2b4e74b0246d",
        "https://graph.microsoft.com/v1.0/users/ae67a4f4-2308-4522-9021-9f402ff0fba8",
        "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783",
        "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133"
    ],
    "owners@odata.bind":[
        "https://graph.microsoft.com/v1.0/users/6a1272b5-f6fc-45c4-95fe-fe7c5a676133",
        "https://graph.microsoft.com/v1.0/users/eab978dd-35d0-4885-8c46-891b7d618783"
    ]
}
```

下面的示例展示了响应。 

>**注意：** 为了提高可读性，所示的响应对象可能已缩短。 所有属性都是从实际调用返回。

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
}
```

## <a name="add-a-team-to-the-group"></a>将团队添加到组

将团队添加到组，如下所示。

```http
PUT /groups/{id}/team
{ }
```

下面的示例展示了响应。 

>**注意：** 为了提高可读性，所示的响应对象可能已缩短。 所有属性都是从实际调用返回。

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context" : "https://graph.microsoft.com/v1.0/$metadata#teams/$entity",
    "id" : "b7f968af-ca51-42f6-a77e-82c7147bc8f2",
    "webUrl" : "https://example.com",
    "isArchived" : null,
    "memberSettings" : { },
    "guestSettings" : { },
    "messagingSettings" : { },
    "funSettings" : {}
}
```

已创建团队的 ID 与组相同。
