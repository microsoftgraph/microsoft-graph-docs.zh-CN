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
# <a name="creating-a-group-with-a-microsoft-teams-team"></a><span data-ttu-id="be287-103">与 Microsoft 团队团队创建组</span><span class="sxs-lookup"><span data-stu-id="be287-103">Creating a group with a Microsoft Teams team</span></span>

<span data-ttu-id="be287-104">创建[组](/graph/api/resources/group?view=graph-rest-beta)，其中包括[团队](/graph/api/resources/team?view=graph-rest-beta)涉及两个步骤：</span><span class="sxs-lookup"><span data-stu-id="be287-104">Creating a [group](/graph/api/resources/group?view=graph-rest-beta) that includes a [team](/graph/api/resources/team?view=graph-rest-beta) involves two steps:</span></span> 

- <span data-ttu-id="be287-105">[创建组](/graph/api/group-post-groups?view=graph-rest-beta)具有正确的属性。</span><span class="sxs-lookup"><span data-stu-id="be287-105">[Create a group](/graph/api/group-post-groups?view=graph-rest-beta) with the right properties.</span></span>
- <span data-ttu-id="be287-106">[团队添加](/graph/api/team-put-teams?view=graph-rest-beta)到组。</span><span class="sxs-lookup"><span data-stu-id="be287-106">[Add a team](/graph/api/team-put-teams?view=graph-rest-beta) to the group.</span></span>

## <a name="create-a-group"></a><span data-ttu-id="be287-107">创建组</span><span class="sxs-lookup"><span data-stu-id="be287-107">Create a group</span></span>

<span data-ttu-id="be287-108">为了包括团队，您需要设置以下属性值，如下面的示例中所示：</span><span class="sxs-lookup"><span data-stu-id="be287-108">In order to include a team, you need to set the following property values, as shown in the following example:</span></span>

- <span data-ttu-id="be287-109">**groupTypes** = {"Unified"}</span><span class="sxs-lookup"><span data-stu-id="be287-109">**groupTypes** = { "Unified" }</span></span> 
- <span data-ttu-id="be287-110">**mailEnabled** = true</span><span class="sxs-lookup"><span data-stu-id="be287-110">**mailEnabled** = true</span></span>
- <span data-ttu-id="be287-111">**securityEnabled** = false</span><span class="sxs-lookup"><span data-stu-id="be287-111">**securityEnabled** = false</span></span>

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

<span data-ttu-id="be287-112">下面的示例演示响应。</span><span class="sxs-lookup"><span data-stu-id="be287-112">The following example shows response.</span></span> 

><span data-ttu-id="be287-113">**注意：** 为便于阅读，可能缩短显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="be287-113">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="be287-114">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="be287-114">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx
{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id":"b7f968af-ca51-42f6-a77e-82c7147bc8f2"
}
```

## <a name="add-a-team-to-the-group"></a><span data-ttu-id="be287-115">团队添加到组</span><span class="sxs-lookup"><span data-stu-id="be287-115">Add a team to the group</span></span>

<span data-ttu-id="be287-116">添加到组，团队，如下所示。</span><span class="sxs-lookup"><span data-stu-id="be287-116">Add a team to the group, as shown.</span></span>

```http
PUT /groups/{id}/team
{ }
```

<span data-ttu-id="be287-117">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="be287-117">The following example shows the response.</span></span> 

><span data-ttu-id="be287-118">**注意：** 为便于阅读，可能缩短显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="be287-118">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="be287-119">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="be287-119">All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="be287-120">创建的团队具有组相同的 ID。</span><span class="sxs-lookup"><span data-stu-id="be287-120">The created team has the same ID as the group.</span></span>
