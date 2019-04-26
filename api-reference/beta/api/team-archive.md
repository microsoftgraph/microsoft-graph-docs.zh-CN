---
title: 存档团队
description: '存档指定的团队。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9ecef149a8cebf297487c3060bdc51793df8d921
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335400"
---
# <a name="archive-team"></a><span data-ttu-id="e95b1-103">存档团队</span><span class="sxs-lookup"><span data-stu-id="e95b1-103">Archive team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e95b1-104">存档指定的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="e95b1-104">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="e95b1-105">存档团队后，用户无法再团队中的任意频道上发送或点赞消息，无法再编辑团队名称、说明和其他设置，且通常也无法再对团队进行大部分更改。</span><span class="sxs-lookup"><span data-stu-id="e95b1-105">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="e95b1-106">仍可向团队进行成员身份更改。</span><span class="sxs-lookup"><span data-stu-id="e95b1-106">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="e95b1-107">存档属于异步操作。</span><span class="sxs-lookup"><span data-stu-id="e95b1-107">Archiving is an async operation.</span></span> <span data-ttu-id="e95b1-108">该异步操作成功完成后，团队即已存档，此 API 作出响应后就可能出现此情况。</span><span class="sxs-lookup"><span data-stu-id="e95b1-108">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="e95b1-109">要对团队存档，团队和[组](../resources/group.md)都必须有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="e95b1-109">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="e95b1-110">要从存档状态还原团队，请使用 API [取消存档](team-unarchive.md)。</span><span class="sxs-lookup"><span data-stu-id="e95b1-110">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e95b1-111">权限</span><span class="sxs-lookup"><span data-stu-id="e95b1-111">Permissions</span></span>
<span data-ttu-id="e95b1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e95b1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e95b1-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="e95b1-114">Permission type</span></span>      | <span data-ttu-id="e95b1-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e95b1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e95b1-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e95b1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e95b1-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e95b1-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e95b1-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e95b1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e95b1-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e95b1-119">Not supported.</span></span>    |
|<span data-ttu-id="e95b1-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="e95b1-120">Application</span></span> | <span data-ttu-id="e95b1-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e95b1-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="e95b1-122">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="e95b1-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e95b1-123">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="e95b1-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e95b1-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e95b1-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="e95b1-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="e95b1-125">Request headers</span></span>
| <span data-ttu-id="e95b1-126">标头</span><span class="sxs-lookup"><span data-stu-id="e95b1-126">Header</span></span>       | <span data-ttu-id="e95b1-127">值</span><span class="sxs-lookup"><span data-stu-id="e95b1-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e95b1-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="e95b1-128">Authorization</span></span>  | <span data-ttu-id="e95b1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e95b1-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e95b1-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e95b1-131">Request body</span></span>
<span data-ttu-id="e95b1-132">在请求中，可_选择性地_在 JSON 正文中包括 `shouldSetSpoSiteReadOnlyForMembers` 参数，如下所示。</span><span class="sxs-lookup"><span data-stu-id="e95b1-132">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="e95b1-133">此可选参数定义了是否在与团队关联的 Sharepoint Online 网站上将团队成员的权限设置为“只读”。</span><span class="sxs-lookup"><span data-stu-id="e95b1-133">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="e95b1-134">如果将其设置为 false 或完全省略正文，将导致跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="e95b1-134">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="e95b1-135">响应</span><span class="sxs-lookup"><span data-stu-id="e95b1-135">Response</span></span>

<span data-ttu-id="e95b1-136">如果成功开始存档，此方法将返回一个 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e95b1-136">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="e95b1-137">响应还将包含一个 `Location` 标头，后者包含创建用于处理团队存档操作的 [teamsAsyncOperation](../resources/teamsasyncoperation.md) 的位置。</span><span class="sxs-lookup"><span data-stu-id="e95b1-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="e95b1-138">可通过向此位置发出 GET 请求，查看存档操作的状态。</span><span class="sxs-lookup"><span data-stu-id="e95b1-138">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="e95b1-139">示例</span><span class="sxs-lookup"><span data-stu-id="e95b1-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e95b1-140">请求</span><span class="sxs-lookup"><span data-stu-id="e95b1-140">Request</span></span>
<span data-ttu-id="e95b1-141">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="e95b1-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="e95b1-142">响应</span><span class="sxs-lookup"><span data-stu-id="e95b1-142">Response</span></span>
<span data-ttu-id="e95b1-143">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="e95b1-143">The following is an example of a response.</span></span>
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
  "suppressions": []
}
-->
