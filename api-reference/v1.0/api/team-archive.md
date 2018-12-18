---
title: 存档团队
description: '存档指定的团队。 '
author: nkramer
ms.openlocfilehash: bd673db676bebad2213710b8005abd28d074f1ca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301244"
---
# <a name="archive-team"></a><span data-ttu-id="b2d74-103">存档团队</span><span class="sxs-lookup"><span data-stu-id="b2d74-103">Archive team</span></span>



<span data-ttu-id="b2d74-104">存档指定的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="b2d74-104">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="b2d74-105">团队存档时，用户可以不再发送或团队中的任何频道上的邮件，类似编辑工作组的名称、 说明或其他设置，或通常对团队大多数的更改。</span><span class="sxs-lookup"><span data-stu-id="b2d74-105">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="b2d74-106">向团队的成员身份更改继续允许。</span><span class="sxs-lookup"><span data-stu-id="b2d74-106">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="b2d74-107">存档是异步操作。</span><span class="sxs-lookup"><span data-stu-id="b2d74-107">Archiving is an async operation.</span></span> <span data-ttu-id="b2d74-108">一旦异步操作已成功完成，此 API 响应后可能出现的存档团队。</span><span class="sxs-lookup"><span data-stu-id="b2d74-108">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="b2d74-109">才能存档团队，团队和[组](../resources/group.md)必须具有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="b2d74-109">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="b2d74-110">若要从其存档状态还原团队，使用 API 对[unarchive](team-unarchive.md)。</span><span class="sxs-lookup"><span data-stu-id="b2d74-110">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b2d74-111">权限</span><span class="sxs-lookup"><span data-stu-id="b2d74-111">Permissions</span></span>
<span data-ttu-id="b2d74-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2d74-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2d74-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2d74-114">Permission type</span></span>      | <span data-ttu-id="b2d74-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2d74-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2d74-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2d74-116">Delegated (work or school account)</span></span> | <span data-ttu-id="b2d74-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2d74-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b2d74-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2d74-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2d74-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2d74-119">Not supported.</span></span>    |
|<span data-ttu-id="b2d74-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2d74-120">Application</span></span> | <span data-ttu-id="b2d74-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2d74-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="b2d74-122">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="b2d74-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b2d74-123">全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。</span><span class="sxs-lookup"><span data-stu-id="b2d74-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b2d74-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2d74-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="b2d74-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2d74-125">Request headers</span></span>
| <span data-ttu-id="b2d74-126">标头</span><span class="sxs-lookup"><span data-stu-id="b2d74-126">Header</span></span>       | <span data-ttu-id="b2d74-127">值</span><span class="sxs-lookup"><span data-stu-id="b2d74-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b2d74-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2d74-128">Authorization</span></span>  | <span data-ttu-id="b2d74-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2d74-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b2d74-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2d74-131">Request body</span></span>
<span data-ttu-id="b2d74-132">在请求中，则可以_选择_包括`shouldSetSpoSiteReadOnlyForMembers`以 json 格式的参数正文，，如下所示。</span><span class="sxs-lookup"><span data-stu-id="b2d74-132">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="b2d74-133">此可选的参数定义是否与团队关联的 Sharepoint Online 网站上设置为只读的工作组成员的权限。</span><span class="sxs-lookup"><span data-stu-id="b2d74-133">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="b2d74-134">设置为 false 或省略正文完全将导致正在跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="b2d74-134">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="b2d74-135">响应</span><span class="sxs-lookup"><span data-stu-id="b2d74-135">Response</span></span>

<span data-ttu-id="b2d74-136">如果存档成功启动，此方法返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="b2d74-136">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="b2d74-137">响应还将包含`Location`标头，其中包含已创建以处理存档的团队[teamsAsyncOperation](../resources/teamsasyncoperation.md)的位置。</span><span class="sxs-lookup"><span data-stu-id="b2d74-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="b2d74-138">通过对此位置进行 GET 请求检查存档操作的状态。</span><span class="sxs-lookup"><span data-stu-id="b2d74-138">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="b2d74-139">示例</span><span class="sxs-lookup"><span data-stu-id="b2d74-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b2d74-140">请求</span><span class="sxs-lookup"><span data-stu-id="b2d74-140">Request</span></span>
<span data-ttu-id="b2d74-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b2d74-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="b2d74-142">响应</span><span class="sxs-lookup"><span data-stu-id="b2d74-142">Response</span></span>
<span data-ttu-id="b2d74-143">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="b2d74-143">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
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
