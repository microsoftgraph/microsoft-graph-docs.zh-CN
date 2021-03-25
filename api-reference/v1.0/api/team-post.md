---
title: 创建团队
description: 新建团队。
author: anandjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6a6a26b350f27d81d9a5ae0d5279bf62058fa161
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202637"
---
# <a name="create-team"></a><span data-ttu-id="a89be-103">创建团队</span><span class="sxs-lookup"><span data-stu-id="a89be-103">Create team</span></span>

<span data-ttu-id="a89be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a89be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a89be-105">新建[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="a89be-105">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a89be-106">权限</span><span class="sxs-lookup"><span data-stu-id="a89be-106">Permissions</span></span>

<span data-ttu-id="a89be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a89be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a89be-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a89be-109">Permission type</span></span>                        | <span data-ttu-id="a89be-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a89be-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a89be-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a89be-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a89be-112">Team.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a89be-112">Team.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="a89be-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a89be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a89be-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a89be-114">Not supported.</span></span>                              |
| <span data-ttu-id="a89be-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a89be-115">Application</span></span>                            | <span data-ttu-id="a89be-116">Team.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a89be-116">Team.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="a89be-117">**注意**：Teamwork.Migrate.All 权限 *仅* 支持 [迁移](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)。</span><span class="sxs-lookup"><span data-stu-id="a89be-117">**Note**: The Teamwork.Migrate.All permission is *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="a89be-118">将来，Microsoft 可能要求你或你的客户根据导入的数据量支付其他费用。</span><span class="sxs-lookup"><span data-stu-id="a89be-118">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

## <a name="http-request"></a><span data-ttu-id="a89be-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a89be-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="a89be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a89be-120">Request headers</span></span>

| <span data-ttu-id="a89be-121">标头</span><span class="sxs-lookup"><span data-stu-id="a89be-121">Header</span></span>        | <span data-ttu-id="a89be-122">值</span><span class="sxs-lookup"><span data-stu-id="a89be-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="a89be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a89be-123">Authorization</span></span> | <span data-ttu-id="a89be-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a89be-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a89be-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a89be-126">Content-Type</span></span>  | <span data-ttu-id="a89be-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a89be-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a89be-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a89be-129">Request body</span></span>

<span data-ttu-id="a89be-130">在请求正文中，提供 [team](../resources/team.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a89be-130">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a89be-131">响应</span><span class="sxs-lookup"><span data-stu-id="a89be-131">Response</span></span>

<span data-ttu-id="a89be-132">如果成功，则此 API 将返回包含 [teamsAsyncOperation](../resources/teamsasyncoperation.md) 链接的 `202 Accepted` 响应。</span><span class="sxs-lookup"><span data-stu-id="a89be-132">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="a89be-133">示例</span><span class="sxs-lookup"><span data-stu-id="a89be-133">Examples</span></span>

### <a name="example-1-delegated-permissions"></a><span data-ttu-id="a89be-134">示例 1：委派权限</span><span class="sxs-lookup"><span data-stu-id="a89be-134">Example 1: Delegated permissions</span></span>

<span data-ttu-id="a89be-135">下面是一个最小请求示例。</span><span class="sxs-lookup"><span data-stu-id="a89be-135">The following is an example of a minimal request.</span></span> <span data-ttu-id="a89be-136">通过省略其他属性，客户端可以隐式采用 `template` 表示的预定义模板的默认值。</span><span class="sxs-lookup"><span data-stu-id="a89be-136">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="a89be-137">请求</span><span class="sxs-lookup"><span data-stu-id="a89be-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a89be-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a89be-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description"
}
```


---


##### <a name="response"></a><span data-ttu-id="a89be-139">响应</span><span class="sxs-lookup"><span data-stu-id="a89be-139">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
Content-Length: 0
```

### <a name="example-2-application-permissions"></a><span data-ttu-id="a89be-140">示例 2：应用权限</span><span class="sxs-lookup"><span data-stu-id="a89be-140">Example 2: Application permissions</span></span>

<span data-ttu-id="a89be-141">下面是使用应用程序权限的最小请求示例。</span><span class="sxs-lookup"><span data-stu-id="a89be-141">The following is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="a89be-142">通过省略其他属性，客户端可以隐式采用 `template` 表示的预定义模板的默认值。</span><span class="sxs-lookup"><span data-stu-id="a89be-142">By omitting other properties, the client is implicitly taking defaults from the predefined template represented by `template`.</span></span> <span data-ttu-id="a89be-143">通过应用程序权限发出请求时，必须在 `members` 集合中指定[用户](../resources/user.md)。</span><span class="sxs-lookup"><span data-stu-id="a89be-143">When issuing a request with application permissions, a [user](../resources/user.md) must be specified in the `members` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="a89be-144">请求</span><span class="sxs-lookup"><span data-stu-id="a89be-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a89be-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="a89be-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post_minimal"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
   "displayName":"My Sample Team",
   "description":"My Sample Team’s Description",
   "members":[
      {
         "@odata.type":"#microsoft.graph.aadUserConversationMember",
         "roles":[
            "owner"
         ],
         "user@odata.bind":"https://graph.microsoft.com/v1.0/users('0040b377-61d8-43db-94f5-81374122dc7e')"
      }
   ]
}
```


---


#### <a name="response"></a><span data-ttu-id="a89be-146">响应</span><span class="sxs-lookup"><span data-stu-id="a89be-146">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post_minimal",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
Content-Length: 0
```

### <a name="example-3-create-a-team-with-multiple-channels-installed-apps-and-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="a89be-147">示例 3：通过委派的权限，创建一个包含多个频道、安装了应用且固定有选项卡的团队。</span><span class="sxs-lookup"><span data-stu-id="a89be-147">Example 3: Create a team with multiple channels, installed apps, and pinned tabs using delegated permissions</span></span>

<span data-ttu-id="a89be-148">下面是具有完整有效负载的请求。</span><span class="sxs-lookup"><span data-stu-id="a89be-148">The following is a request with a full payload.</span></span> <span data-ttu-id="a89be-149">客户端可以覆盖基础模板中的值，并将数组值项添加到 `specialization` 的验证规则允许的区间。</span><span class="sxs-lookup"><span data-stu-id="a89be-149">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="a89be-150">请求</span><span class="sxs-lookup"><span data-stu-id="a89be-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a89be-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="a89be-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_post_full_payload"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
    "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
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
                    "displayName": "A Pinned Website",
                    "configuration": {
                        "contentUrl": "https://docs.microsoft.com/microsoftteams/microsoft-teams"
                    }
                },
                {
                    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.youtube')",
                    "displayName": "A Pinned YouTube Video",
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
---

#### <a name="response"></a><span data-ttu-id="a89be-152">响应</span><span class="sxs-lookup"><span data-stu-id="a89be-152">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_post_full_payload",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('958e8cf8-169a-42aa-8599-5c1c5479c0ca')/operations('00000000-0000-0000-0000-000000000000')
Content-Location: /teams('958e8cf8-169a-42aa-8599-5c1c5479c0ca')
Content-Length: 0
```

### <a name="example-4-create-a-team-from-group"></a><span data-ttu-id="a89be-153">示例 4：通过组来创建团队</span><span class="sxs-lookup"><span data-stu-id="a89be-153">Example 4: Create a team from group</span></span>

<span data-ttu-id="a89be-154">下面的示例展示了你可如何在给定 **groupId** 的情况下通过 [组](../resources/group.md)来创建 [团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="a89be-154">The following example shows how you can create a new [team](../resources/team.md) from a [group](../resources/group.md), given a **groupId**.</span></span>

<span data-ttu-id="a89be-155">此调用需注意以下几点：</span><span class="sxs-lookup"><span data-stu-id="a89be-155">A few things to note about this call:</span></span>

* <span data-ttu-id="a89be-156">要创建团队，从中创建团队的组必须至少有一名所有者。</span><span class="sxs-lookup"><span data-stu-id="a89be-156">In order to create a team, the group you're creating it from must have a least one owner.</span></span>
* <span data-ttu-id="a89be-157">所创建的团队将始终从组的显示名称、可见性、规范和成员继承。</span><span class="sxs-lookup"><span data-stu-id="a89be-157">The team that's created will always inherit from the group's display name, visibility, specialization, and members.</span></span> <span data-ttu-id="a89be-158">因此，在使用 **group@odata.bind** 属性进行此调用时，如果包含团队的 **displayName**、**visibility**、**specialization** 或 **members@odata.bind** 属性，则将返回错误。</span><span class="sxs-lookup"><span data-stu-id="a89be-158">Therefore, when making this call with the **group@odata.bind** property, the inclusion of team **displayName**, **visibility**, **specialization**, or **members@odata.bind** properties will return an error.</span></span>
* <span data-ttu-id="a89be-159">如果在不到 15 分钟之前创建组，则可能会因为重复延迟导致“创建团队呼叫”失败并显示错误代码 404。</span><span class="sxs-lookup"><span data-stu-id="a89be-159">If the group was created less than 15 minutes ago, it's possible for the Create team call to fail with a 404 error code due to replication delays.</span></span> <span data-ttu-id="a89be-160">建议重试“创建团队”调用三次，每次调用之间延迟 10 秒。</span><span class="sxs-lookup"><span data-stu-id="a89be-160">We recommend that you retry the Create team call three times, with a 10 second delay between calls.</span></span>

#### <a name="request"></a><span data-ttu-id="a89be-161">请求</span><span class="sxs-lookup"><span data-stu-id="a89be-161">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a89be-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="a89be-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_team_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
  "group@odata.bind": "https://graph.microsoft.com/v1.0/groups('71392b2f-1765-406e-86af-5907d9bdb2ab')"
}
```

---

---
#### <a name="response"></a><span data-ttu-id="a89be-163">响应</span><span class="sxs-lookup"><span data-stu-id="a89be-163">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_team_from_group",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('71392b2f-1765-406e-86af-5907d9bdb2ab')/operations('9698b2b8-9636-4f49-b7a8-10dadfa7062a')
Content-Location: /teams('71392b2f-1765-406e-86af-5907d9bdb2ab')
Content-Length: 0
```

### <a name="example-5-create-a-team-from-a-group-with-multiple-channels-installed-apps-and-pinned-tabs"></a><span data-ttu-id="a89be-164">示例 5：通过组创建一个包含多个频道、安装了应用且固定有选项卡的团队</span><span class="sxs-lookup"><span data-stu-id="a89be-164">Example 5: Create a team from a group with multiple channels, installed apps, and pinned tabs</span></span>

<span data-ttu-id="a89be-165">下列请求会对具有扩展属性的现有组进行转换，这将创建安装了应用且带有固定选项卡和多个频道的团队。</span><span class="sxs-lookup"><span data-stu-id="a89be-165">The following is a request that converts an existing group with extended properties which will create the team with multiple channels, installed apps, and pinned tabs.</span></span>

<span data-ttu-id="a89be-166">若要了解有关受支持的基本模板类型和受支持的属性的更多信息，请参阅 [Teams 模板入门](/MicrosoftTeams/get-started-with-teams-templates)。</span><span class="sxs-lookup"><span data-stu-id="a89be-166">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="a89be-167">请求</span><span class="sxs-lookup"><span data-stu-id="a89be-167">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a89be-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="a89be-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
   "group@odata.bind":"https://graph.microsoft.com/v1.0/groups('dbd8de4f-5d47-48da-87f1-594bed003375')",
   "channels":[
      {
         "displayName":"Class Announcements 📢",
         "isFavoriteByDefault":true
      },
      {
         "displayName":"Homework 🏋️",
         "isFavoriteByDefault":true
      }
   ],
   "memberSettings":{
      "allowCreateUpdateChannels":false,
      "allowDeleteChannels":false,
      "allowAddRemoveApps":false,
      "allowCreateUpdateRemoveTabs":false,
      "allowCreateUpdateRemoveConnectors":false
   },
   "installedApps":[
      {
         "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
      },
      {
         "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
      }
   ]
}
```


---

---
#### <a name="response"></a><span data-ttu-id="a89be-169">响应</span><span class="sxs-lookup"><span data-stu-id="a89be-169">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_group",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
Content-Length: 0
```

### <a name="example-6-create-a-team-with-a-non-standard-base-template-type"></a><span data-ttu-id="a89be-170">示例 6：创建具有非标准基本模板类型的团队</span><span class="sxs-lookup"><span data-stu-id="a89be-170">Example 6: Create a team with a non-standard base template type</span></span>

<span data-ttu-id="a89be-171">基本模板类型是 Microsoft 为特定行业创建的特殊模板。</span><span class="sxs-lookup"><span data-stu-id="a89be-171">Base template types are special templates that Microsoft created for specific industries.</span></span> <span data-ttu-id="a89be-172">这些基本模板通常包含商店中不提供的专有应用以及 Microsoft Teams 模板中尚未单独支持的团队属性。</span><span class="sxs-lookup"><span data-stu-id="a89be-172">These base templates often contain proprietary apps that aren't available in the store and team properties that are not yet supported individually in Microsoft Teams templates.</span></span>

<span data-ttu-id="a89be-173">若要从非标准基本模板创建团队，你要将请求正文中的 `template@odata.bind` 属性从 `standard` 更改为指向你要创建的特定基本模板。</span><span class="sxs-lookup"><span data-stu-id="a89be-173">To create a team from a non-standard base template, you’ll want to change the `template@odata.bind` property in the request body from `standard` to point to the specific base template you’d like to create.</span></span>

<span data-ttu-id="a89be-174">若要了解有关受支持的基本模板类型的更多信息，请参阅 [Teams 模板入门](/MicrosoftTeams/get-started-with-teams-templates)。</span><span class="sxs-lookup"><span data-stu-id="a89be-174">To learn more about supported base template types, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="a89be-175">请求</span><span class="sxs-lookup"><span data-stu-id="a89be-175">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a89be-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="a89be-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_non_standard"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
  "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('educationClass')",
  "displayName": "My Class Team",
  "description": "My Class Team’s Description"
}
```


---

---

#### <a name="response"></a><span data-ttu-id="a89be-177">响应</span><span class="sxs-lookup"><span data-stu-id="a89be-177">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_non_standard",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
Content-Length: 0
```

### <a name="example-7-create-a-team-with-a-non-standard-base-template-type-with-extended-properties"></a><span data-ttu-id="a89be-178">示例 7：通过扩展属性创建具有非标准基本模板类型的团队</span><span class="sxs-lookup"><span data-stu-id="a89be-178">Example 7: Create a team with a non-standard base template type with extended properties</span></span>

<span data-ttu-id="a89be-179">基本模板类型可以使用其他属性进行扩展，使你可以使用其他团队设置、渠道、应用或选项卡构建现有基本模板。</span><span class="sxs-lookup"><span data-stu-id="a89be-179">Base template types can be extended with additional properties, enabling you to build on an existing base template with additional team settings, channels, apps, or tabs.</span></span>

<span data-ttu-id="a89be-180">若要了解有关受支持的基本模板类型和受支持的属性的更多信息，请参阅 [Teams 模板入门](/MicrosoftTeams/get-started-with-teams-templates)。</span><span class="sxs-lookup"><span data-stu-id="a89be-180">To learn more about supported base template types and supported properties, see [Get started with Teams templates](/MicrosoftTeams/get-started-with-teams-templates).</span></span>

#### <a name="request"></a><span data-ttu-id="a89be-181">请求</span><span class="sxs-lookup"><span data-stu-id="a89be-181">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a89be-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="a89be-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "convert_team_from_non_standard2"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
   "template@odata.bind":"https://graph.microsoft.com/v1.0/teamsTemplates('educationClass')",
   "displayName":"My Class Team",
   "description":"My Class Team’s Description",
   "channels":[
      {
         "displayName":"Class Announcements 📢",
         "isFavoriteByDefault":true
      },
      {
         "displayName":"Homework 🏋️",
         "isFavoriteByDefault":true
      }
   ],
   "memberSettings":{
      "allowCreateUpdateChannels":false,
      "allowDeleteChannels":false,
      "allowAddRemoveApps":false,
      "allowCreateUpdateRemoveTabs":false,
      "allowCreateUpdateRemoveConnectors":false
   },
   "installedApps":[
      {
         "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
      },
      {
         "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
      }
   ]
}
```


---

---
#### <a name="response"></a><span data-ttu-id="a89be-183">响应</span><span class="sxs-lookup"><span data-stu-id="a89be-183">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "convert_team_from_non_standard2",
  "@odata.type": "microsoft.graph.team"
}-->
```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
Content-Length: 0
```

### <a name="example-8-create-a-team-in-migration-mode"></a><span data-ttu-id="a89be-184">示例 8：创建处于迁移模式的团队</span><span class="sxs-lookup"><span data-stu-id="a89be-184">Example 8: Create a team in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="a89be-185">请求</span><span class="sxs-lookup"><span data-stu-id="a89be-185">Request</span></span>

<span data-ttu-id="a89be-186">以下示例演示如何创建用于导入消息的团队。</span><span class="sxs-lookup"><span data-stu-id="a89be-186">The following example shows how to create a team for imported messages.</span></span>

><span data-ttu-id="a89be-187">**注意：** 将来，Microsoft 可能要求你或你的客户根据导入的数据量支付其他|</span><span class="sxs-lookup"><span data-stu-id="a89be-187">**Note:** In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.|</span></span>

><span data-ttu-id="a89be-188">**注意：** 在迁移模式下创建的团队仅支持 `standard` 模板。</span><span class="sxs-lookup"><span data-stu-id="a89be-188">**Note:** Teams created in migration mode only support the `standard` template.</span></span>

```http
POST https://graph.microsoft.com/v1.0/teams
Content-Type: application/json

{
  "@microsoft.graph.teamCreationMode": "migration",
  "template@odata.bind": "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
  "createdDateTime": "2020-03-14T11:22:17.067Z"
}
```

#### <a name="response"></a><span data-ttu-id="a89be-189">响应</span><span class="sxs-lookup"><span data-stu-id="a89be-189">Response</span></span>

```http
HTTP/1.1 202 Accepted
Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')/operations('3a6fdce1-c261-48bc-89de-1cfef658c0d5')
Content-Location: /teams('dbd8de4f-5d47-48da-87f1-594bed003375')
```

#### <a name="error-response"></a><span data-ttu-id="a89be-190">错误响应</span><span class="sxs-lookup"><span data-stu-id="a89be-190">Error response</span></span>

<span data-ttu-id="a89be-191">如果该请求成功，此方法返回 `400 Bad Request` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a89be-191">If the request is unsuccessful, this method returns a `400 Bad Request` response code.</span></span> 

```http
400 Bad Request
```

<span data-ttu-id="a89be-192">下面是出现此响应的常见原因：</span><span class="sxs-lookup"><span data-stu-id="a89be-192">The following are common reasons for this response:</span></span>

* <span data-ttu-id="a89be-193">**createdDateTime** 将在未来设置。</span><span class="sxs-lookup"><span data-stu-id="a89be-193">**createdDateTime** is set in the future.</span></span>
* <span data-ttu-id="a89be-194">正确指定了 **createdDateTime**，但缺少 **teamCreationMode** 实例属性或者将其设置成了无效值。</span><span class="sxs-lookup"><span data-stu-id="a89be-194">**createdDateTime** is correctly specified but the **teamCreationMode** instance attribute is missing or set to an invalid value.</span></span>

## <a name="see-also"></a><span data-ttu-id="a89be-195">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a89be-195">See also</span></span>

* [<span data-ttu-id="a89be-196">完成团队迁移</span><span class="sxs-lookup"><span data-stu-id="a89be-196">Complete migration for a team</span></span>](team-completemigration.md)
* [<span data-ttu-id="a89be-197">使用 Microsoft Graph 将第三方平台消息导入 Teams</span><span class="sxs-lookup"><span data-stu-id="a89be-197">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="a89be-198">创建频道</span><span class="sxs-lookup"><span data-stu-id="a89be-198">Create channel</span></span>](channel-post.md)
* [<span data-ttu-id="a89be-199">可用模板</span><span class="sxs-lookup"><span data-stu-id="a89be-199">Available templates</span></span>](/MicrosoftTeams/get-started-with-teams-templates)
* [<span data-ttu-id="a89be-200">Teams 零售模板入门</span><span class="sxs-lookup"><span data-stu-id="a89be-200">Getting started with Retail Teams templates</span></span>](/MicrosoftTeams/get-started-with-retail-teams-templates)
* [<span data-ttu-id="a89be-201">Teams 医疗保健模板入门</span><span class="sxs-lookup"><span data-stu-id="a89be-201">Getting started with Healthcare Teams templates</span></span>](/MicrosoftTeams/healthcare/healthcare-templates)
* [<span data-ttu-id="a89be-202">创建包含团队的组</span><span class="sxs-lookup"><span data-stu-id="a89be-202">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
