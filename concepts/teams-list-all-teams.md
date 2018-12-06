---
title: 列表中的 Microsoft 团队的组织的所有团队
description: '列出所有团队 '
ms.openlocfilehash: 2a9dbaa1fc9a02897870865295fd8d0dac9266a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091859"
---
# <a name="list-all-teams-in-microsoft-teams-for-an-organization"></a><span data-ttu-id="25457-103">列表中的 Microsoft 团队的组织的所有团队</span><span class="sxs-lookup"><span data-stu-id="25457-103">List all teams in Microsoft Teams for an organization</span></span>

<span data-ttu-id="25457-104">列出所有[团队](/graph/api/resources/team?view=graph-rest-beta)组织 （租户） 中，可以查找具有团队的所有组，然后获取每个工作组的信息。</span><span class="sxs-lookup"><span data-stu-id="25457-104">To list all [teams](/graph/api/resources/team?view=graph-rest-beta) in an organization (tenant), you find all groups that have teams, and then get information for each team.</span></span>

## <a name="get-a-list-of-groups"></a><span data-ttu-id="25457-105">获取组的列表</span><span class="sxs-lookup"><span data-stu-id="25457-105">Get a list of groups</span></span>

<span data-ttu-id="25457-106">要获取的团队的组织中的所有[组](/graph/api/resources/group?view=graph-rest-beta)列表，请获取[所有组的列表](/graph/api/group-list?view=graph-rest-beta)，然后在代码中查找具有**resourceProvisioningOptions**属性包含"团队"。</span><span class="sxs-lookup"><span data-stu-id="25457-106">To get a list of all [groups](/graph/api/resources/group?view=graph-rest-beta) in the organization that have teams, get a [list of all groups](/graph/api/group-list?view=graph-rest-beta) and then in code find the ones that have a **resourceProvisioningOptions** property that contains "Team".</span></span>
<span data-ttu-id="25457-107">由于组大型对象，使用 $select 仅获取您关注的组的属性。</span><span class="sxs-lookup"><span data-stu-id="25457-107">Since groups are large objects, use $select to only get the properties of the group you care about.</span></span>

```http
GET /groups?$select=id,resourceProvisioningOptions
```

> <span data-ttu-id="25457-108">**注意**： 某些未使用的旧小组没有 resourceProvisioningOptions 设置。</span><span class="sxs-lookup"><span data-stu-id="25457-108">**Note**: Certain unused old teams will not have resourceProvisioningOptions set.</span></span> <span data-ttu-id="25457-109">有关详细信息，请参阅[已知问题](known-issues.md#missing-teams-in-list-all-teams)。</span><span class="sxs-lookup"><span data-stu-id="25457-109">For details, see [known issues](known-issues.md#missing-teams-in-list-all-teams).</span></span>

<span data-ttu-id="25457-110">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="25457-110">The following is an example of the response.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

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

## <a name="get-a-list-of-groups-using-beta-apis"></a><span data-ttu-id="25457-111">获取使用 beta Api 的组的列表</span><span class="sxs-lookup"><span data-stu-id="25457-111">Get a list of groups using beta APIs</span></span>

<span data-ttu-id="25457-112">使用 beta Api，您可以使用 $filter 返回仅包含团队的组。</span><span class="sxs-lookup"><span data-stu-id="25457-112">Using the beta APIs, you can use $filter to return only the groups that have teams.</span></span>

```http
GET /groups?$filter=resourceProvisioningOptions/Any(x:x eq 'Team')
```

> <span data-ttu-id="25457-113">**注意**： 上 /groups $filter 仅可通过 beta 终结点。</span><span class="sxs-lookup"><span data-stu-id="25457-113">**Note**: $filter on /groups is only available through the beta endpoint.</span></span> <span data-ttu-id="25457-114">resourceProvisioningOptions 是在 v1.0 和 beta 中可用。</span><span class="sxs-lookup"><span data-stu-id="25457-114">resourceProvisioningOptions is available in v1.0 and beta.</span></span>

> <span data-ttu-id="25457-115">**注意**： 不会列出某些未使用的旧团队。</span><span class="sxs-lookup"><span data-stu-id="25457-115">**Note**: Certain unused old teams will not be listed.</span></span> <span data-ttu-id="25457-116">有关详细信息，请参阅[已知问题](known-issues.md#missing-teams-in-list-all-teams)。</span><span class="sxs-lookup"><span data-stu-id="25457-116">For details, see [known issues](known-issues.md#missing-teams-in-list-all-teams).</span></span>

<span data-ttu-id="25457-117">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="25457-117">The following is an example of the response.</span></span> 

><span data-ttu-id="25457-118">**注意：** 为便于阅读，可能缩短显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="25457-118">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="25457-119">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="25457-119">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups",
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
            "visibility": "Private",
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
            "visibility": "Private",
        }
    ]
}
```

## <a name="get-team-information-for-a-group"></a><span data-ttu-id="25457-120">获取组的工作组信息</span><span class="sxs-lookup"><span data-stu-id="25457-120">Get team information for a group</span></span>

<span data-ttu-id="25457-121">若要获取特定组中的工作组的工作组信息，请调用[让团队](/graph/api/team-get?view=graph-rest-beta)API，并包括组 id。</span><span class="sxs-lookup"><span data-stu-id="25457-121">To get team information for the team in a particular group, call the [get team](/graph/api/team-get?view=graph-rest-beta) API and include the group ID.</span></span>

```http
GET /teams/{group-id}
```

<span data-ttu-id="25457-122">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="25457-122">The following example shows the response.</span></span>

><span data-ttu-id="25457-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="25457-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

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

## <a name="see-also"></a><span data-ttu-id="25457-125">另请参阅</span><span class="sxs-lookup"><span data-stu-id="25457-125">See also</span></span>

- [<span data-ttu-id="25457-126">列表 joinedTeams</span><span class="sxs-lookup"><span data-stu-id="25457-126">List joinedTeams</span></span>](/graph/api/user-list-joinedteams?view=graph-rest-beta)
- [<span data-ttu-id="25457-127">列出组</span><span class="sxs-lookup"><span data-stu-id="25457-127">List groups</span></span>](/graph/api/group-list?view=graph-rest-beta)
