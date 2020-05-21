---
title: 创建团队
description: 新建团队。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 410a2a98275e80d91c35dcf4f82357f8563cf314
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335435"
---
# <a name="create-team"></a><span data-ttu-id="9b4ba-103">创建团队</span><span class="sxs-lookup"><span data-stu-id="9b4ba-103">Create team</span></span>

<span data-ttu-id="9b4ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b4ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b4ba-105">新建[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-105">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b4ba-106">权限</span><span class="sxs-lookup"><span data-stu-id="9b4ba-106">Permissions</span></span>

<span data-ttu-id="9b4ba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b4ba-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b4ba-109">Permission type</span></span>                        | <span data-ttu-id="9b4ba-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b4ba-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="9b4ba-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b4ba-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b4ba-112">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b4ba-112">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="9b4ba-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b4ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b4ba-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-114">Not supported.</span></span>                              |
| <span data-ttu-id="9b4ba-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b4ba-115">Application</span></span>                            | <span data-ttu-id="9b4ba-116">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b4ba-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b4ba-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b4ba-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="9b4ba-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b4ba-118">Request headers</span></span>

| <span data-ttu-id="9b4ba-119">标头</span><span class="sxs-lookup"><span data-stu-id="9b4ba-119">Header</span></span>        | <span data-ttu-id="9b4ba-120">值</span><span class="sxs-lookup"><span data-stu-id="9b4ba-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="9b4ba-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b4ba-121">Authorization</span></span> | <span data-ttu-id="9b4ba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9b4ba-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9b4ba-124">Content-Type</span></span>  | <span data-ttu-id="9b4ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b4ba-125">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="9b4ba-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b4ba-126">Request body</span></span>

<span data-ttu-id="9b4ba-127">在请求正文中，提供 [team](../resources/team.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-127">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9b4ba-128">响应</span><span class="sxs-lookup"><span data-stu-id="9b4ba-128">Response</span></span>

<span data-ttu-id="9b4ba-129">如果成功，则此 API 将返回包含 [teamsAsyncOperation](../resources/teamsasyncoperation.md) 链接的 `202 Accepted` 响应。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-129">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="9b4ba-130">示例</span><span class="sxs-lookup"><span data-stu-id="9b4ba-130">Examples</span></span>

### <a name="example-1-delegated-permissions"></a><span data-ttu-id="9b4ba-131">示例 1：委派权限</span><span class="sxs-lookup"><span data-stu-id="9b4ba-131">Example 1: Delegated permissions</span></span>

<span data-ttu-id="9b4ba-132">下面是一个最小请求示例。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-132">The following is an example of a minimal request.</span></span> <span data-ttu-id="9b4ba-133">通过省略其他属性，客户端可以隐式采用 `template` 表示的预定义模板的默认值。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-133">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="9b4ba-134">请求</span><span class="sxs-lookup"><span data-stu-id="9b4ba-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9b4ba-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b4ba-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post"
}-->
```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description"
}
```
# <a name="c"></a>[<span data-ttu-id="9b4ba-136">C#</span><span class="sxs-lookup"><span data-stu-id="9b4ba-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b4ba-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b4ba-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b4ba-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b4ba-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9b4ba-139">响应</span><span class="sxs-lookup"><span data-stu-id="9b4ba-139">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-2-application-permissions"></a><span data-ttu-id="9b4ba-140">示例 2：应用权限</span><span class="sxs-lookup"><span data-stu-id="9b4ba-140">Example 2: Application permissions</span></span>

<span data-ttu-id="9b4ba-141">下面是使用应用程序权限的最小请求示例。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-141">The following is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="9b4ba-142">通过省略其他属性，客户端可以隐式采用 `template` 表示的预定义模板的默认值。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-142">By omitting other properties, the client is implicitly taking defaults from the predefined template represented by `template`.</span></span> <span data-ttu-id="9b4ba-143">通过应用程序权限发出请求时，必须在 `owners` 集合中指定[用户](../resources/user.md)。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-143">When issuing a request with application permissions, a [user](../resources/user.md) must be specified in the `owners` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="9b4ba-144">请求</span><span class="sxs-lookup"><span data-stu-id="9b4ba-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9b4ba-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b4ba-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post_minimal"
}-->
```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users('userId')"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="9b4ba-146">C#</span><span class="sxs-lookup"><span data-stu-id="9b4ba-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b4ba-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b4ba-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-post-minimal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b4ba-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b4ba-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-post-minimal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9b4ba-149">响应</span><span class="sxs-lookup"><span data-stu-id="9b4ba-149">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post_minimal",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-3-create-a-team-with-multiple-channels-installed-apps-and-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="9b4ba-150">示例 3：通过委派的权限，创建一个包含多个频道、安装了应用且固定有选项卡的团队。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-150">Example 3: Create a team with multiple channels, installed apps, and pinned tabs using delegated permissions</span></span>

<span data-ttu-id="9b4ba-151">下面是具有完整有效负载的请求。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-151">The following is a request with a full payload.</span></span> <span data-ttu-id="9b4ba-152">客户端可以覆盖基础模板中的值，并将数组值项添加到 `specialization` 的验证规则允许的区间。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-152">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="9b4ba-153">请求</span><span class="sxs-lookup"><span data-stu-id="9b4ba-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9b4ba-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b4ba-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post_full_payload"
}-->
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
                        "contentUrl": "https://docs.microsoft.com/microsoftteams/microsoft-teams"
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
    "discoverySettings": {
        "showInTeamsSearchAndSuggestions": true
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
# <a name="c"></a>[<span data-ttu-id="9b4ba-155">C#</span><span class="sxs-lookup"><span data-stu-id="9b4ba-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-post-full-payload-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b4ba-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b4ba-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-post-full-payload-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b4ba-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b4ba-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-post-full-payload-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9b4ba-158">响应</span><span class="sxs-lookup"><span data-stu-id="9b4ba-158">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post_full_payload",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-4-create-a-team-from-group"></a><span data-ttu-id="9b4ba-159">示例 4：通过组来创建团队</span><span class="sxs-lookup"><span data-stu-id="9b4ba-159">Example 4: Create a team from group</span></span>

<span data-ttu-id="9b4ba-160">下面的示例展示了你可如何在给定 **groupId** 的情况下通过[组](../resources/group.md)来创建[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-160">The following example shows how you can create a new [team](../resources/team.md) from a [group](../resources/group.md), given a **groupId**.</span></span>

<span data-ttu-id="9b4ba-161">此调用需注意以下几点：</span><span class="sxs-lookup"><span data-stu-id="9b4ba-161">A few thing to note about this call:</span></span>

* <span data-ttu-id="9b4ba-162">要创建团队，从中创建团队的组必须至少有一名所有者。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-162">In order to create a team, the group you're creating it from must have a least one owner.</span></span>
* <span data-ttu-id="9b4ba-163">所创建的团队将始终从组的显示名称、可见性、规范和所有者继承。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-163">The team that's created will always inherit from the group's display name, visibility, specialization, and owners.</span></span> <span data-ttu-id="9b4ba-164">因此，在使用 **group@odata.bind** 属性进行此调用时，如果包含团队的 **displayName**、**visibility**、**specialization** 或 **owners@odata.bind** 属性，则将返回错误。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-164">Therefore, when making this call with the **group@odata.bind** property, the inclusion of team **displayName**, **visibility**, **specialization**, or **owners@odata.bind** properties will return an error.</span></span>
* <span data-ttu-id="9b4ba-165">如果在不到 15 分钟之前创建组，则可能会因为重复延迟导致“创建团队呼叫”失败并显示错误代码 404。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-165">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="9b4ba-166">建议重试“创建团队”调用三次，每次调用之间延迟 10 秒。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-166">We recommend that you retry the Create team call three times, with a 10 second delay between calls.</span></span>


#### <a name="request"></a><span data-ttu-id="9b4ba-167">请求</span><span class="sxs-lookup"><span data-stu-id="9b4ba-167">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9b4ba-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b4ba-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('groupId')"
}
```
# <a name="c"></a>[<span data-ttu-id="9b4ba-169">C#</span><span class="sxs-lookup"><span data-stu-id="9b4ba-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-team-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b4ba-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b4ba-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-team-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b4ba-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b4ba-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-team-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9b4ba-172">响应</span><span class="sxs-lookup"><span data-stu-id="9b4ba-172">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_from_group",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-5-create-a-team-from-a-group-with-multiple-channels-installed-apps-and-pinned-tabs"></a><span data-ttu-id="9b4ba-173">示例 5：通过组创建一个包含多个频道、安装了应用且固定有选项卡的团队</span><span class="sxs-lookup"><span data-stu-id="9b4ba-173">Example 5: Create a team from a group with multiple channels, installed apps, and pinned tabs</span></span>

<span data-ttu-id="9b4ba-174">下列请求会对具有扩展属性的现有组进行转换，这将创建安装了应用且带有固定选项卡和多个频道的团队。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-174">The following is a request that converts an existing group with extended properties which will create the team with multiple channels, installed apps, and pinned tabs.</span></span>

<span data-ttu-id="9b4ba-175">若要了解有关受支持的基本模板类型和受支持的属性的更多信息，请参阅 [Teams 模板入门](/MicrosoftTeams/get-started-with-teams-templates)。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-175">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="9b4ba-176">请求</span><span class="sxs-lookup"><span data-stu-id="9b4ba-176">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9b4ba-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b4ba-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('groupId')",
  "channels": [
        {
            "displayName": "Class Announcements 📢",
            "isFavoriteByDefault": true
        },
        {
            "displayName": "Homework 🏋️",
            "isFavoriteByDefault": true,
        }
    ],
    "memberSettings": {
        "allowCreateUpdateChannels": false,
        "allowDeleteChannels": false,
        "allowAddRemoveApps": false,
        "allowCreateUpdateRemoveTabs": false,
        "allowCreateUpdateRemoveConnectors": false
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
# <a name="c"></a>[<span data-ttu-id="9b4ba-178">C#</span><span class="sxs-lookup"><span data-stu-id="9b4ba-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-team-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b4ba-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b4ba-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-team-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b4ba-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b4ba-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-team-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9b4ba-181">响应</span><span class="sxs-lookup"><span data-stu-id="9b4ba-181">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_group",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-6-create-a-team-with-a-non-standard-base-template-type"></a><span data-ttu-id="9b4ba-182">示例 6：创建具有非标准基本模板类型的团队</span><span class="sxs-lookup"><span data-stu-id="9b4ba-182">Example 6: Create a team with a non-standard base template type</span></span>

<span data-ttu-id="9b4ba-183">基本模板类型是 Microsoft 为特定行业创建的特殊模板。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-183">Base template types are special templates that Microsoft created for specific industries.</span></span> <span data-ttu-id="9b4ba-184">这些基本模板通常包含商店中不提供的专有应用以及 Microsoft Teams 模板中尚未单独支持的团队属性。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-184">These base templates often contain proprietary apps that aren't available in the store and team properties that are not yet supported individually in Microsoft Teams templates.</span></span>

<span data-ttu-id="9b4ba-185">若要从非标准基本模板创建团队，你要将请求正文中的 `template@odata.bind` 属性从 `standard` 更改为指向你要创建的特定基本模板。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-185">To create a team from a non-standard base template, you’ll want to change the `template@odata.bind` property in the request body from `standard` to point to the specific base template you’d like to create.</span></span>

<span data-ttu-id="9b4ba-186">若要了解有关受支持的基本模板类型的更多信息，请参阅 [Teams 模板入门](/MicrosoftTeams/get-started-with-teams-templates)。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-186">To learn more about supported base template types, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="9b4ba-187">请求</span><span class="sxs-lookup"><span data-stu-id="9b4ba-187">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9b4ba-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b4ba-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_non_standard"
}-->
```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('educationClass')",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description"
}
```
# <a name="c"></a>[<span data-ttu-id="9b4ba-189">C#</span><span class="sxs-lookup"><span data-stu-id="9b4ba-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-team-from-non-standard-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b4ba-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b4ba-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-team-from-non-standard-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b4ba-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b4ba-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-team-from-non-standard-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9b4ba-192">响应</span><span class="sxs-lookup"><span data-stu-id="9b4ba-192">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_non_standard",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

### <a name="example-7-create-a-team-with-a-non-standard-base-template-type-with-extended-properties"></a><span data-ttu-id="9b4ba-193">示例 7：通过扩展属性创建具有非标准基本模板类型的团队</span><span class="sxs-lookup"><span data-stu-id="9b4ba-193">Example 7: Create a team with a non-standard base template type with extended properties</span></span>

<span data-ttu-id="9b4ba-194">基本模板类型可以使用其他属性进行扩展，使你可以使用其他团队设置、渠道、应用或选项卡构建现有基本模板。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-194">Base template types can be extended with additional properties, enabling you to build on an existing base template with additional team settings, channels, apps, or tabs.</span></span>

<span data-ttu-id="9b4ba-195">若要了解有关受支持的基本模板类型和受支持的属性的更多信息，请参阅 [Teams 模板入门](/MicrosoftTeams/get-started-with-teams-templates)。</span><span class="sxs-lookup"><span data-stu-id="9b4ba-195">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="9b4ba-196">请求</span><span class="sxs-lookup"><span data-stu-id="9b4ba-196">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9b4ba-197">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b4ba-197">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_non_standard2"
}-->
```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('educationClass')",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description",
  "channels": [
        {
            "displayName": "Class Announcements 📢",
            "isFavoriteByDefault": true
        },
        {
            "displayName": "Homework 🏋️",
            "isFavoriteByDefault": true,
        }
    ],
    "memberSettings": {
        "allowCreateUpdateChannels": false,
        "allowDeleteChannels": false,
        "allowAddRemoveApps": false,
        "allowCreateUpdateRemoveTabs": false,
        "allowCreateUpdateRemoveConnectors": false
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
# <a name="c"></a>[<span data-ttu-id="9b4ba-198">C#</span><span class="sxs-lookup"><span data-stu-id="9b4ba-198">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/convert-team-from-non-standard2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b4ba-199">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b4ba-199">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/convert-team-from-non-standard2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b4ba-200">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b4ba-200">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/convert-team-from-non-standard2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9b4ba-201">响应</span><span class="sxs-lookup"><span data-stu-id="9b4ba-201">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_non_standard2",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
Content-Length: 0
```

## <a name="see-also"></a><span data-ttu-id="9b4ba-202">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9b4ba-202">See also</span></span>

- [<span data-ttu-id="9b4ba-203">可用模板</span><span class="sxs-lookup"><span data-stu-id="9b4ba-203">Available templates</span></span>](/MicrosoftTeams/get-started-with-teams-templates)
- [<span data-ttu-id="9b4ba-204">Teams 零售模板入门</span><span class="sxs-lookup"><span data-stu-id="9b4ba-204">Getting started with Retail Teams templates</span></span>](https://docs.microsoft.com/MicrosoftTeams/get-started-with-retail-teams-templates)
- [<span data-ttu-id="9b4ba-205">Teams 医疗保健模板入门</span><span class="sxs-lookup"><span data-stu-id="9b4ba-205">Getting started with Healthcare Teams templates</span></span>](https://docs.microsoft.com/MicrosoftTeams/healthcare/healthcare-templates)
- [<span data-ttu-id="9b4ba-206">创建包含团队的组</span><span class="sxs-lookup"><span data-stu-id="9b4ba-206">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
