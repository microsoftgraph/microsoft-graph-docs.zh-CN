---
title: 与 Microsoft 团队团队创建组
description: '创建组，其中包括团队涉及两个步骤： '
ms.openlocfilehash: 530b3625a1aa1d020bff841196e3b83a2eb99a4e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091803"
---
# <a name="creating-a-group-with-a-microsoft-teams-team"></a>与 Microsoft 团队团队创建组

创建[组](/graph/api/resources/group?view=graph-rest-beta)，其中包括[团队](/graph/api/resources/team?view=graph-rest-beta)涉及两个步骤： 

- [创建组](/graph/api/group-post-groups?view=graph-rest-beta)具有正确的属性。
- [团队添加](/graph/api/team-put-teams?view=graph-rest-beta)到组。

## <a name="create-a-group"></a>创建组

为了包括团队，您需要设置以下属性值，如下面的示例中所示：

- **groupTypes** = {"Unified"} 
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

下面的示例演示响应。 

>**注意：** 为便于阅读，可能缩短显示的响应对象。 所有属性都将通过实际调用返回。

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
}
```

## <a name="add-a-team-to-the-group"></a>团队添加到组

添加到组，团队，如下所示。

```http
PUT /groups/{id}/team
{ }
```

以下示例显示了相应的响应。 

>**注意：** 为便于阅读，可能缩短显示的响应对象。 所有属性都将通过实际调用返回。

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

创建的团队具有组相同的 ID。
