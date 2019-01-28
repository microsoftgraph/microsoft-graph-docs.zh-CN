---
title: 创建团队
description: 新建团队。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 3e901225f5a8f94abb61a6b4052b0db2d47865c3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519610"
---
# <a name="create-team"></a><span data-ttu-id="e6ca0-103">创建团队</span><span class="sxs-lookup"><span data-stu-id="e6ca0-103">Create team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6ca0-104">新建[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="e6ca0-104">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6ca0-105">权限</span><span class="sxs-lookup"><span data-stu-id="e6ca0-105">Permissions</span></span>

<span data-ttu-id="e6ca0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6ca0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6ca0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6ca0-108">Permission type</span></span>                        | <span data-ttu-id="e6ca0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6ca0-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e6ca0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6ca0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6ca0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6ca0-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="e6ca0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6ca0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6ca0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6ca0-113">Not supported.</span></span>                              |
| <span data-ttu-id="e6ca0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6ca0-114">Application</span></span>                            | <span data-ttu-id="e6ca0-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6ca0-115">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e6ca0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6ca0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="e6ca0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6ca0-117">Request headers</span></span>

| <span data-ttu-id="e6ca0-118">标头</span><span class="sxs-lookup"><span data-stu-id="e6ca0-118">Header</span></span>        | <span data-ttu-id="e6ca0-119">值</span><span class="sxs-lookup"><span data-stu-id="e6ca0-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="e6ca0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6ca0-120">Authorization</span></span> | <span data-ttu-id="e6ca0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6ca0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e6ca0-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6ca0-123">Content-Type</span></span>  | <span data-ttu-id="e6ca0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e6ca0-124">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="e6ca0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6ca0-125">Request body</span></span>

<span data-ttu-id="e6ca0-126">在请求正文中，提供 [team](../resources/team.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6ca0-126">In the request body, supply a JSON representation of [plannerBucket](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e6ca0-127">响应</span><span class="sxs-lookup"><span data-stu-id="e6ca0-127">Response</span></span>

<span data-ttu-id="e6ca0-128">如果成功，则此 API 将返回包含 [teamsAsyncOperation](../resources/teamsasyncoperation.md) 链接的 `202 Accepted` 响应。</span><span class="sxs-lookup"><span data-stu-id="e6ca0-128">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="e6ca0-129">示例</span><span class="sxs-lookup"><span data-stu-id="e6ca0-129">Examples</span></span>

### <a name="example---delegated-permissions"></a><span data-ttu-id="e6ca0-130">示例 - 委派权限</span><span class="sxs-lookup"><span data-stu-id="e6ca0-130">Example - delegated permissions</span></span>

<span data-ttu-id="e6ca0-131">以下是最小请求的示例。</span><span class="sxs-lookup"><span data-stu-id="e6ca0-131">Here is an example of a minimal request.</span></span> <span data-ttu-id="e6ca0-132">通过省略其他属性，客户端可以隐式采用 `template` 表示的预定义模板的默认值。</span><span class="sxs-lookup"><span data-stu-id="e6ca0-132">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="e6ca0-133">请求</span><span class="sxs-lookup"><span data-stu-id="e6ca0-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
}
```

##### <a name="response"></a><span data-ttu-id="e6ca0-134">响应</span><span class="sxs-lookup"><span data-stu-id="e6ca0-134">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---create-a-team-with-an-app-installed-multiple-channels-with-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="e6ca0-135">示例 - 通过使用委派权限安装的应用以及带固定选项卡的多个渠道创建团队。</span><span class="sxs-lookup"><span data-stu-id="e6ca0-135">Example - create a team with an app installed, multiple channels with pinned tabs using delegated permissions</span></span>

<span data-ttu-id="e6ca0-136">以下是具有完整有效负载的请求。</span><span class="sxs-lookup"><span data-stu-id="e6ca0-136">Here is request with a full payload.</span></span> <span data-ttu-id="e6ca0-137">客户端可以覆盖基础模板中的值，并将数组值项添加到 `specialization` 的验证规则允许的区间。</span><span class="sxs-lookup"><span data-stu-id="e6ca0-137">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="e6ca0-138">请求</span><span class="sxs-lookup"><span data-stu-id="e6ca0-138">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
    "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
    "visibility": "Private",
    "displayName": "Sample Engineering Team",
    "description": "This is a sample engineering team, used to showcase the range of properties supported by this API",
    "channels": [
        {
            "displayName": "Announcements 📢",
            "isFavoriteByDefault": true,
            "description": "This is a sample announcements channel that is favorited by default. Use this channel to make important team, product, and service announcements."
        },
        {
            "displayName": "Training 🏋️",
            "isFavoriteByDefault": true,
            "description": "This is a sample training channel, that is favorited by default, and contains an example of pinned website and YouTube tabs.",
            "tabs": [
                {
                    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.web')",
                    "name": "A Pinned Website",
                    "configuration": {
                        "contentUrl": "https://docs.microsoft.com/en-us/microsoftteams/microsoft-teams"
                    }
                },
                {
                    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.youtube')",
                    "name": "A Pinned YouTube Video",
                    "configuration": {
                        "contentUrl": "https://tabs.teams.microsoft.com/Youtube/Home/YoutubeTab?videoId=X8krAMdGvCQ",
                        "websiteUrl": "https://www.youtube.com/watch?v=X8krAMdGvCQ"
                    }
                }
            ]
        },
        {
            "displayName": "Planning 📅 ",
            "description": "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.",
            "isFavoriteByDefault": false
        },
        {
            "displayName": "Issues and Feedback 🐞",
            "description": "This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu."
        }
    ],
    "memberSettings": {
        "allowCreateUpdateChannels": true,
        "allowDeleteChannels": true,
        "allowAddRemoveApps": true,
        "allowCreateUpdateRemoveTabs": true,
        "allowCreateUpdateRemoveConnectors": true
    },
    "guestSettings": {
        "allowCreateUpdateChannels": false,
        "allowDeleteChannels": false
    },
    "funSettings": {
        "allowGiphy": true,
        "giphyContentRating": "Moderate",
        "allowStickersAndMemes": true,
        "allowCustomMemes": true
    },
    "messagingSettings": {
        "allowUserEditMessages": true,
        "allowUserDeleteMessages": true,
        "allowOwnerDeleteMessages": true,
        "allowTeamMentions": true,
        "allowChannelMentions": true
    },
    "installedApps": [
        {
            "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
        },
        {
            "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="e6ca0-139">响应</span><span class="sxs-lookup"><span data-stu-id="e6ca0-139">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---application-permissions"></a><span data-ttu-id="e6ca0-140">示例 - 应用程序权限</span><span class="sxs-lookup"><span data-stu-id="e6ca0-140">Example - application permissions</span></span>

<span data-ttu-id="e6ca0-141">以下是使用应用程序权限的最小请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6ca0-141">Here is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="e6ca0-142">通过省略其他属性，客户端可以隐式采用 `template` 表示的预定义模板的默认值。</span><span class="sxs-lookup"><span data-stu-id="e6ca0-142">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span> <span data-ttu-id="e6ca0-143">通过应用程序权限发出请求时，必须在 `owners` 集合中指定[用户](../resources/user.md)。</span><span class="sxs-lookup"><span data-stu-id="e6ca0-143">When issuing a request with application permissions a [user](../resources/user.md) must be specified in the `owners` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="e6ca0-144">请求</span><span class="sxs-lookup"><span data-stu-id="e6ca0-144">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users('abc123')"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="e6ca0-145">响应</span><span class="sxs-lookup"><span data-stu-id="e6ca0-145">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

## <a name="see-also"></a><span data-ttu-id="e6ca0-146">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e6ca0-146">See also</span></span>

- [<span data-ttu-id="e6ca0-147">创建包含团队的组</span><span class="sxs-lookup"><span data-stu-id="e6ca0-147">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/team-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
