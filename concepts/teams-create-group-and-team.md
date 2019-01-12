---
title: 创建包含 Microsoft Teams 团队的组
description: '若要创建包含团队的组，请按以下两步操作： '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 06b25a6da159030407c904622ffebde09c704d98
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970477"
---
# <a name="creating-a-group-with-a-microsoft-teams-team"></a><span data-ttu-id="0bc4c-103">创建包含 Microsoft Teams 团队的组</span><span class="sxs-lookup"><span data-stu-id="0bc4c-103">Creating a group with a Microsoft Teams team</span></span>

<span data-ttu-id="0bc4c-104">若要创建包含[团队](/graph/api/resources/team?view=graph-rest-beta)的[组](/graph/api/resources/group?view=graph-rest-beta)，请按以下两步操作：</span><span class="sxs-lookup"><span data-stu-id="0bc4c-104">Creating a [group](/graph/api/resources/group?view=graph-rest-beta) that includes a [team](/graph/api/resources/team?view=graph-rest-beta) involves two steps:</span></span> 

- <span data-ttu-id="0bc4c-105">使用正确属性[创建组](/graph/api/group-post-groups?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="0bc4c-105">[Create a group](/graph/api/group-post-groups?view=graph-rest-beta) with the right properties.</span></span>
- <span data-ttu-id="0bc4c-106">[将团队添加](/graph/api/team-put-teams?view=graph-rest-beta)到组。</span><span class="sxs-lookup"><span data-stu-id="0bc4c-106">[Add a team](/graph/api/team-put-teams?view=graph-rest-beta) to the group.</span></span>

## <a name="create-a-group"></a><span data-ttu-id="0bc4c-107">创建组</span><span class="sxs-lookup"><span data-stu-id="0bc4c-107">Create a group</span></span>

<span data-ttu-id="0bc4c-108">若要添加团队，必须设置以下属性值，如下面的示例所示：</span><span class="sxs-lookup"><span data-stu-id="0bc4c-108">In order to include a team, you need to set the following property values, as shown in the following example:</span></span>

- <span data-ttu-id="0bc4c-109">**groupTypes** = { "Unified" }</span><span class="sxs-lookup"><span data-stu-id="0bc4c-109">**groupTypes** = { "Unified" }</span></span> 
- <span data-ttu-id="0bc4c-110">**mailEnabled** = true</span><span class="sxs-lookup"><span data-stu-id="0bc4c-110">**mailEnabled** = true</span></span>
- <span data-ttu-id="0bc4c-111">**securityEnabled** = false</span><span class="sxs-lookup"><span data-stu-id="0bc4c-111">**securityEnabled** = false</span></span>

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

<span data-ttu-id="0bc4c-112">下面的示例展示了响应。</span><span class="sxs-lookup"><span data-stu-id="0bc4c-112">The following example shows response.</span></span> 

><span data-ttu-id="0bc4c-113">**注意：** 为了提高可读性，所示的响应对象可能已缩短。</span><span class="sxs-lookup"><span data-stu-id="0bc4c-113">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="0bc4c-114">所有属性都是从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0bc4c-114">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
}
```

## <a name="add-a-team-to-the-group"></a><span data-ttu-id="0bc4c-115">将团队添加到组</span><span class="sxs-lookup"><span data-stu-id="0bc4c-115">Add a team to the group</span></span>

<span data-ttu-id="0bc4c-116">将团队添加到组，如下所示。</span><span class="sxs-lookup"><span data-stu-id="0bc4c-116">Add a team to the group, as shown.</span></span>

```http
PUT /groups/{id}/team
{ }
```

<span data-ttu-id="0bc4c-117">下面的示例展示了响应。</span><span class="sxs-lookup"><span data-stu-id="0bc4c-117">The following example shows the response.</span></span> 

><span data-ttu-id="0bc4c-118">**注意：** 为了提高可读性，所示的响应对象可能已缩短。</span><span class="sxs-lookup"><span data-stu-id="0bc4c-118">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="0bc4c-119">所有属性都是从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0bc4c-119">All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="0bc4c-120">已创建团队的 ID 与组相同。</span><span class="sxs-lookup"><span data-stu-id="0bc4c-120">The created team has the same ID as the group.</span></span>
