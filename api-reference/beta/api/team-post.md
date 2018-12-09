---
title: 创建工作组
description: 创建新的团队。
ms.openlocfilehash: 3f2fa97af217d6109f169e5b2ef75a0c71bde2e7
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2018
ms.locfileid: "27210140"
---
# <a name="create-team"></a><span data-ttu-id="ca31b-103">创建工作组</span><span class="sxs-lookup"><span data-stu-id="ca31b-103">Create team</span></span>

> <span data-ttu-id="ca31b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ca31b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca31b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ca31b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca31b-106">创建新的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="ca31b-106">Create a new [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca31b-107">权限</span><span class="sxs-lookup"><span data-stu-id="ca31b-107">Permissions</span></span>

<span data-ttu-id="ca31b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca31b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca31b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca31b-110">Permission type</span></span>                        | <span data-ttu-id="ca31b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca31b-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ca31b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca31b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca31b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca31b-113">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="ca31b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca31b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca31b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca31b-115">Not supported.</span></span>                              |
| <span data-ttu-id="ca31b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca31b-116">Application</span></span>                            | <span data-ttu-id="ca31b-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca31b-117">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ca31b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca31b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams
```

## <a name="request-headers"></a><span data-ttu-id="ca31b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca31b-119">Request headers</span></span>

| <span data-ttu-id="ca31b-120">标头</span><span class="sxs-lookup"><span data-stu-id="ca31b-120">Header</span></span>        | <span data-ttu-id="ca31b-121">值</span><span class="sxs-lookup"><span data-stu-id="ca31b-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="ca31b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca31b-122">Authorization</span></span> | <span data-ttu-id="ca31b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca31b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca31b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca31b-125">Content-Type</span></span>  | <span data-ttu-id="ca31b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca31b-126">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="ca31b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca31b-127">Request body</span></span>

<span data-ttu-id="ca31b-128">在请求正文中，提供一个[团队](../resources/team.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca31b-128">In the request body, supply a JSON representation of a [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ca31b-129">响应</span><span class="sxs-lookup"><span data-stu-id="ca31b-129">Response</span></span>

<span data-ttu-id="ca31b-130">如果成功，此 API 返回`202 Accepted`响应，其中包含指向[teamsAsyncOperation](../resources/teamsasyncoperation.md)的链接。</span><span class="sxs-lookup"><span data-stu-id="ca31b-130">If successful, this API returns a `202 Accepted` response containing a link to the [teamsAsyncOperation](../resources/teamsasyncoperation.md).</span></span>

## <a name="examples"></a><span data-ttu-id="ca31b-131">示例</span><span class="sxs-lookup"><span data-stu-id="ca31b-131">Examples</span></span>

### <a name="example---delegated-permissions"></a><span data-ttu-id="ca31b-132">示例-委派权限</span><span class="sxs-lookup"><span data-stu-id="ca31b-132">Example - delegated permissions</span></span>

<span data-ttu-id="ca31b-133">下面是请求的一个内容最少示例。</span><span class="sxs-lookup"><span data-stu-id="ca31b-133">Here is an example of a minimal request.</span></span> <span data-ttu-id="ca31b-134">通过省略其他属性，客户端隐式正在由预定义模板中的默认值`template`。</span><span class="sxs-lookup"><span data-stu-id="ca31b-134">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span>

#### <a name="request"></a><span data-ttu-id="ca31b-135">请求</span><span class="sxs-lookup"><span data-stu-id="ca31b-135">Request</span></span>

```http
POST https://graph.microsoft.com/beta/teams
Content-Type: application/json
{
  "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates/standard",
  "displayName": "My Sample Team",
  "description": "My Sample Team’s Description",
}
```

##### <a name="response"></a><span data-ttu-id="ca31b-136">响应</span><span class="sxs-lookup"><span data-stu-id="ca31b-136">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---create-a-team-with-an-app-installed-multiple-channels-with-pinned-tabs-using-delegated-permissions"></a><span data-ttu-id="ca31b-137">示例-使用安装应用程序创建团队，与使用固定选项卡的多个通道委派权限</span><span class="sxs-lookup"><span data-stu-id="ca31b-137">Example - create a team with an app installed, multiple channels with pinned tabs using delegated permissions</span></span>

<span data-ttu-id="ca31b-138">下面是与完全负载的请求。</span><span class="sxs-lookup"><span data-stu-id="ca31b-138">Here is request with a full payload.</span></span> <span data-ttu-id="ca31b-139">客户端可以重写基本模板中的值并将添加到允许的有效性规则的范围内的数组值项`specialization`。</span><span class="sxs-lookup"><span data-stu-id="ca31b-139">The client can override values in the base template and add to array-valued items to the extent allowed by validation rules for the `specialization`.</span></span>

#### <a name="request"></a><span data-ttu-id="ca31b-140">请求</span><span class="sxs-lookup"><span data-stu-id="ca31b-140">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="ca31b-141">响应</span><span class="sxs-lookup"><span data-stu-id="ca31b-141">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

### <a name="example---application-permissions"></a><span data-ttu-id="ca31b-142">示例-应用程序权限</span><span class="sxs-lookup"><span data-stu-id="ca31b-142">Example - application permissions</span></span>

<span data-ttu-id="ca31b-143">下面是使用应用程序权限的最小请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca31b-143">Here is an example of a minimal request using application permissions.</span></span> <span data-ttu-id="ca31b-144">通过省略其他属性，客户端隐式正在由预定义模板中的默认值`template`。</span><span class="sxs-lookup"><span data-stu-id="ca31b-144">By omitting other properties, the client is implicitly taking defaults from the pre-defined template represented by `template`.</span></span> <span data-ttu-id="ca31b-145">当[用户](../resources/user.md)使用应用程序权限发出请求必须指定以`owners`集合。</span><span class="sxs-lookup"><span data-stu-id="ca31b-145">When issuing a request with application permissions a [user](../resources/user.md) must be specified in the `owners` collection.</span></span>

#### <a name="request"></a><span data-ttu-id="ca31b-146">请求</span><span class="sxs-lookup"><span data-stu-id="ca31b-146">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="ca31b-147">响应</span><span class="sxs-lookup"><span data-stu-id="ca31b-147">Response</span></span>

```http
HTTP/1.1 202 Accepted
Content-Type: application/json
Location: /teams/{teamId}/operations/{operationId}
Content-Location: /teams/{teamId}
{
}
```

## <a name="see-also"></a><span data-ttu-id="ca31b-148">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ca31b-148">See also</span></span>

- [<span data-ttu-id="ca31b-149">与团队创建组</span><span class="sxs-lookup"><span data-stu-id="ca31b-149">Creating a group with a team</span></span>](/graph/teams-create-group-and-team)
