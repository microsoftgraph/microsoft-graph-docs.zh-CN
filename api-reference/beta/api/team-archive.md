---
title: 存档团队
description: '将指定的团队存档。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a009dc7214627575b00b2537875e5561b0515d32
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889917"
---
# <a name="archive-team"></a><span data-ttu-id="56687-103">存档团队</span><span class="sxs-lookup"><span data-stu-id="56687-103">Archive team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56687-104">将指定的[团队](../resources/team.md)存档。</span><span class="sxs-lookup"><span data-stu-id="56687-104">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="56687-105">存档团队后, 用户将无法再发送或赞邮件在团队中的任何频道上, 编辑团队的名称、说明或其他设置, 或者通常对团队做出大多数更改。</span><span class="sxs-lookup"><span data-stu-id="56687-105">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="56687-106">仍允许对团队进行成员资格更改。</span><span class="sxs-lookup"><span data-stu-id="56687-106">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="56687-107">存档是一种异步操作。</span><span class="sxs-lookup"><span data-stu-id="56687-107">Archiving is an async operation.</span></span> <span data-ttu-id="56687-108">一旦异步操作成功完成, 则会存档团队, 这可能会在此 API 响应之后发生。</span><span class="sxs-lookup"><span data-stu-id="56687-108">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="56687-109">为了存档团队, 团队和[组](../resources/group.md)必须具有所有者。</span><span class="sxs-lookup"><span data-stu-id="56687-109">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="56687-110">若要从存档状态还原团队, 请使用 API[接档](team-unarchive.md)。</span><span class="sxs-lookup"><span data-stu-id="56687-110">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="56687-111">权限</span><span class="sxs-lookup"><span data-stu-id="56687-111">Permissions</span></span>
<span data-ttu-id="56687-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56687-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56687-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="56687-114">Permission type</span></span>      | <span data-ttu-id="56687-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56687-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56687-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56687-116">Delegated (work or school account)</span></span> | <span data-ttu-id="56687-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56687-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="56687-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56687-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56687-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="56687-119">Not supported.</span></span>    |
|<span data-ttu-id="56687-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="56687-120">Application</span></span> | <span data-ttu-id="56687-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56687-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="56687-122">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="56687-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="56687-123">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="56687-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="56687-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56687-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="56687-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="56687-125">Request headers</span></span>
| <span data-ttu-id="56687-126">标头</span><span class="sxs-lookup"><span data-stu-id="56687-126">Header</span></span>       | <span data-ttu-id="56687-127">值</span><span class="sxs-lookup"><span data-stu-id="56687-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="56687-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="56687-128">Authorization</span></span>  | <span data-ttu-id="56687-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="56687-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="56687-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="56687-131">Request body</span></span>
<span data-ttu-id="56687-132">在请求中, 可以_选择_将`shouldSetSpoSiteReadOnlyForMembers`参数包含在 JSON 正文中, 如下所示。</span><span class="sxs-lookup"><span data-stu-id="56687-132">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="56687-133">此可选参数定义是否在与团队关联的 Sharepoint Online 网站上将工作组成员的权限设置为只读。</span><span class="sxs-lookup"><span data-stu-id="56687-133">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="56687-134">将其设置为 false 或完全省略正文将导致跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="56687-134">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="56687-135">响应</span><span class="sxs-lookup"><span data-stu-id="56687-135">Response</span></span>

<span data-ttu-id="56687-136">如果成功启动存档, 此方法将`202 Accepted`返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="56687-136">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="56687-137">该响应还将包含一个`Location`标头, 其中包含为处理团队存档而创建的[teamsAsyncOperation](../resources/teamsasyncoperation.md)的位置。</span><span class="sxs-lookup"><span data-stu-id="56687-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="56687-138">通过向此位置发出 GET 请求, 检查存档操作的状态。</span><span class="sxs-lookup"><span data-stu-id="56687-138">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="56687-139">示例</span><span class="sxs-lookup"><span data-stu-id="56687-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="56687-140">请求</span><span class="sxs-lookup"><span data-stu-id="56687-140">Request</span></span>
<span data-ttu-id="56687-141">以下是请求的示例。</span><span class="sxs-lookup"><span data-stu-id="56687-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="56687-142">响应</span><span class="sxs-lookup"><span data-stu-id="56687-142">Response</span></span>
<span data-ttu-id="56687-143">下面是响应的一个示例。</span><span class="sxs-lookup"><span data-stu-id="56687-143">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-archive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
