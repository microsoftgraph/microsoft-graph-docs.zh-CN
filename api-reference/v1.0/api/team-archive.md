---
title: 存档团队
description: '存档指定的团队。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d849f4166e0481accb991c6f318e486917e562e3
ms.sourcegitcommit: 435d80cfa71574c06d24780c591d4303a5cd9636
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2020
ms.locfileid: "42572389"
---
# <a name="archive-team"></a><span data-ttu-id="390b6-103">存档团队</span><span class="sxs-lookup"><span data-stu-id="390b6-103">Archive team</span></span>

<span data-ttu-id="390b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="390b6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="390b6-105">存档指定的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="390b6-105">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="390b6-106">存档团队后，用户无法再团队中的任意频道上发送或点赞消息，无法再编辑团队名称、说明和其他设置，且通常也无法再对团队进行大部分更改。</span><span class="sxs-lookup"><span data-stu-id="390b6-106">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="390b6-107">仍可向团队进行成员身份更改。</span><span class="sxs-lookup"><span data-stu-id="390b6-107">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="390b6-108">存档属于异步操作。</span><span class="sxs-lookup"><span data-stu-id="390b6-108">Archiving is an async operation.</span></span> <span data-ttu-id="390b6-109">该异步操作成功完成后，团队即已存档，此 API 作出响应后就可能出现此情况。</span><span class="sxs-lookup"><span data-stu-id="390b6-109">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="390b6-110">要对团队存档，团队和[组](../resources/group.md)都必须有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="390b6-110">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="390b6-111">要从存档状态还原团队，请使用 API [取消存档](team-unarchive.md)。</span><span class="sxs-lookup"><span data-stu-id="390b6-111">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="390b6-112">权限</span><span class="sxs-lookup"><span data-stu-id="390b6-112">Permissions</span></span>
<span data-ttu-id="390b6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="390b6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="390b6-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="390b6-115">Permission type</span></span>      | <span data-ttu-id="390b6-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="390b6-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="390b6-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="390b6-117">Delegated (work or school account)</span></span> | <span data-ttu-id="390b6-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="390b6-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="390b6-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="390b6-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="390b6-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="390b6-120">Not supported.</span></span>    |
|<span data-ttu-id="390b6-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="390b6-121">Application</span></span> | <span data-ttu-id="390b6-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="390b6-122">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="390b6-123">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="390b6-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="390b6-124">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="390b6-124">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="390b6-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="390b6-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="390b6-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="390b6-126">Request headers</span></span>
| <span data-ttu-id="390b6-127">标头</span><span class="sxs-lookup"><span data-stu-id="390b6-127">Header</span></span>       | <span data-ttu-id="390b6-128">值</span><span class="sxs-lookup"><span data-stu-id="390b6-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="390b6-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="390b6-129">Authorization</span></span>  | <span data-ttu-id="390b6-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="390b6-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="390b6-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="390b6-132">Request body</span></span>
<span data-ttu-id="390b6-133">在请求中，可_选择性地_在 JSON 正文中包括 `shouldSetSpoSiteReadOnlyForMembers` 参数，如下所示。</span><span class="sxs-lookup"><span data-stu-id="390b6-133">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="390b6-134">此可选参数定义了是否在与团队关联的 Sharepoint Online 网站上将团队成员的权限设置为“只读”。</span><span class="sxs-lookup"><span data-stu-id="390b6-134">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="390b6-135">如果将其设置为 false 或完全省略正文，将导致跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="390b6-135">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

>[!IMPORTANT]
><span data-ttu-id="390b6-136">应用程序上下文不支持 `shouldSetSpoSiteReadOnlyForMembers` 参数。</span><span class="sxs-lookup"><span data-stu-id="390b6-136">The `shouldSetSpoSiteReadOnlyForMembers` parameter is not supported in the application context.</span></span>

## <a name="response"></a><span data-ttu-id="390b6-137">响应</span><span class="sxs-lookup"><span data-stu-id="390b6-137">Response</span></span>

<span data-ttu-id="390b6-138">如果成功开始存档，此方法将返回一个 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="390b6-138">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="390b6-139">响应还将包含一个 `Location` 标头，后者包含创建用于处理团队存档操作的 [teamsAsyncOperation](../resources/teamsasyncoperation.md) 的位置。</span><span class="sxs-lookup"><span data-stu-id="390b6-139">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="390b6-140">可通过向此位置发出 GET 请求，查看存档操作的状态。</span><span class="sxs-lookup"><span data-stu-id="390b6-140">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="390b6-141">示例</span><span class="sxs-lookup"><span data-stu-id="390b6-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="390b6-142">请求</span><span class="sxs-lookup"><span data-stu-id="390b6-142">Request</span></span>
<span data-ttu-id="390b6-143">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="390b6-143">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="390b6-144">响应</span><span class="sxs-lookup"><span data-stu-id="390b6-144">Response</span></span>
<span data-ttu-id="390b6-145">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="390b6-145">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
