---
title: 存档团队
description: '存档指定的团队。 '
ms.openlocfilehash: 70a7015229784ffda78dc9020a0f847d68027d22
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041748"
---
# <a name="archive-team"></a><span data-ttu-id="44b2c-103">存档团队</span><span class="sxs-lookup"><span data-stu-id="44b2c-103">Archive team</span></span>

> <span data-ttu-id="44b2c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="44b2c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44b2c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="44b2c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44b2c-106">存档指定的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="44b2c-106">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="44b2c-107">团队存档时，用户可以不再发送或团队中的任何频道上的邮件，类似编辑工作组的名称、 说明或其他设置，或通常对团队大多数的更改。</span><span class="sxs-lookup"><span data-stu-id="44b2c-107">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="44b2c-108">向团队的成员身份更改继续允许。</span><span class="sxs-lookup"><span data-stu-id="44b2c-108">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="44b2c-109">存档是异步操作。</span><span class="sxs-lookup"><span data-stu-id="44b2c-109">Archiving is an async operation.</span></span> <span data-ttu-id="44b2c-110">一旦异步操作已成功完成，此 API 响应后可能出现的存档团队。</span><span class="sxs-lookup"><span data-stu-id="44b2c-110">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="44b2c-111">才能存档团队，团队和[组](../resources/group.md)必须具有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="44b2c-111">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="44b2c-112">若要从其存档状态还原团队，使用 API 对[unarchive](team-unarchive.md)。</span><span class="sxs-lookup"><span data-stu-id="44b2c-112">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="44b2c-113">权限</span><span class="sxs-lookup"><span data-stu-id="44b2c-113">Permissions</span></span>
<span data-ttu-id="44b2c-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44b2c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44b2c-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="44b2c-116">Permission type</span></span>      | <span data-ttu-id="44b2c-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44b2c-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44b2c-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44b2c-118">Delegated (work or school account)</span></span> | <span data-ttu-id="44b2c-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44b2c-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="44b2c-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44b2c-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44b2c-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="44b2c-121">Not supported.</span></span>    |
|<span data-ttu-id="44b2c-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="44b2c-122">Application</span></span> | <span data-ttu-id="44b2c-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44b2c-123">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="44b2c-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44b2c-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="44b2c-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="44b2c-125">Request headers</span></span>
| <span data-ttu-id="44b2c-126">标头</span><span class="sxs-lookup"><span data-stu-id="44b2c-126">Header</span></span>       | <span data-ttu-id="44b2c-127">值</span><span class="sxs-lookup"><span data-stu-id="44b2c-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="44b2c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="44b2c-128">Authorization</span></span>  | <span data-ttu-id="44b2c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="44b2c-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="44b2c-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="44b2c-131">Request body</span></span>
<span data-ttu-id="44b2c-132">在请求中，则可以_选择_包括`shouldSetSpoSiteReadOnlyForMembers`以 json 格式的参数正文，，如下所示。</span><span class="sxs-lookup"><span data-stu-id="44b2c-132">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="44b2c-133">此可选的参数定义是否与团队关联的 Sharepoint Online 网站上设置为只读的工作组成员的权限。</span><span class="sxs-lookup"><span data-stu-id="44b2c-133">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="44b2c-134">设置为 false 或省略正文完全将导致正在跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="44b2c-134">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="44b2c-135">响应</span><span class="sxs-lookup"><span data-stu-id="44b2c-135">Response</span></span>

<span data-ttu-id="44b2c-136">如果存档成功启动，此方法返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="44b2c-136">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="44b2c-137">响应还将包含`Location`标头，其中包含已创建以处理存档的团队[teamsAsyncOperation](../resources/teamsasyncoperation.md)的位置。</span><span class="sxs-lookup"><span data-stu-id="44b2c-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="44b2c-138">通过对此位置进行 GET 请求检查存档操作的状态。</span><span class="sxs-lookup"><span data-stu-id="44b2c-138">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="44b2c-139">示例</span><span class="sxs-lookup"><span data-stu-id="44b2c-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="44b2c-140">请求</span><span class="sxs-lookup"><span data-stu-id="44b2c-140">Request</span></span>
<span data-ttu-id="44b2c-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44b2c-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="44b2c-142">响应</span><span class="sxs-lookup"><span data-stu-id="44b2c-142">Response</span></span>
<span data-ttu-id="44b2c-143">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="44b2c-143">The following is an example of a response.</span></span>
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
