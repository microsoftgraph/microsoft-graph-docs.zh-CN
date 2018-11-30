---
title: 存档团队
description: '存档指定的团队。 '
ms.openlocfilehash: 414b45a3dd2f03aba29b3393db3ef547472a8950
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009821"
---
# <a name="archive-team"></a><span data-ttu-id="86db6-103">存档团队</span><span class="sxs-lookup"><span data-stu-id="86db6-103">Archive team</span></span>



<span data-ttu-id="86db6-104">存档指定的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="86db6-104">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="86db6-105">团队存档时，用户可以不再发送或团队中的任何频道上的邮件，类似编辑工作组的名称、 说明或其他设置，或通常对团队大多数的更改。</span><span class="sxs-lookup"><span data-stu-id="86db6-105">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="86db6-106">向团队的成员身份更改继续允许。</span><span class="sxs-lookup"><span data-stu-id="86db6-106">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="86db6-107">存档是异步操作。</span><span class="sxs-lookup"><span data-stu-id="86db6-107">Archiving is an async operation.</span></span> <span data-ttu-id="86db6-108">一旦异步操作已成功完成，此 API 响应后可能出现的存档团队。</span><span class="sxs-lookup"><span data-stu-id="86db6-108">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="86db6-109">才能存档团队，团队和[组](../resources/group.md)必须具有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="86db6-109">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="86db6-110">若要从其存档状态还原团队，使用 API 对[unarchive](team-unarchive.md)。</span><span class="sxs-lookup"><span data-stu-id="86db6-110">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="86db6-111">权限</span><span class="sxs-lookup"><span data-stu-id="86db6-111">Permissions</span></span>
<span data-ttu-id="86db6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86db6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86db6-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="86db6-114">Permission type</span></span>      | <span data-ttu-id="86db6-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86db6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86db6-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86db6-116">Delegated (work or school account)</span></span> | <span data-ttu-id="86db6-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86db6-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="86db6-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86db6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86db6-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="86db6-119">Not supported.</span></span>    |
|<span data-ttu-id="86db6-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="86db6-120">Application</span></span> | <span data-ttu-id="86db6-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86db6-121">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="86db6-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86db6-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="86db6-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="86db6-123">Request headers</span></span>
| <span data-ttu-id="86db6-124">标头</span><span class="sxs-lookup"><span data-stu-id="86db6-124">Header</span></span>       | <span data-ttu-id="86db6-125">值</span><span class="sxs-lookup"><span data-stu-id="86db6-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="86db6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="86db6-126">Authorization</span></span>  | <span data-ttu-id="86db6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="86db6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="86db6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="86db6-129">Request body</span></span>
<span data-ttu-id="86db6-130">在请求中，则可以_选择_包括`shouldSetSpoSiteReadOnlyForMembers`以 json 格式的参数正文，，如下所示。</span><span class="sxs-lookup"><span data-stu-id="86db6-130">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="86db6-131">此可选的参数定义是否与团队关联的 Sharepoint Online 网站上设置为只读的工作组成员的权限。</span><span class="sxs-lookup"><span data-stu-id="86db6-131">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="86db6-132">设置为 false 或省略正文完全将导致正在跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="86db6-132">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="86db6-133">响应</span><span class="sxs-lookup"><span data-stu-id="86db6-133">Response</span></span>

<span data-ttu-id="86db6-134">如果存档成功启动，此方法返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="86db6-134">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="86db6-135">响应还将包含`Location`标头，其中包含已创建以处理存档的团队[teamsAsyncOperation](../resources/teamsasyncoperation.md)的位置。</span><span class="sxs-lookup"><span data-stu-id="86db6-135">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="86db6-136">通过对此位置进行 GET 请求检查存档操作的状态。</span><span class="sxs-lookup"><span data-stu-id="86db6-136">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="86db6-137">示例</span><span class="sxs-lookup"><span data-stu-id="86db6-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="86db6-138">请求</span><span class="sxs-lookup"><span data-stu-id="86db6-138">Request</span></span>
<span data-ttu-id="86db6-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86db6-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="86db6-140">响应</span><span class="sxs-lookup"><span data-stu-id="86db6-140">Response</span></span>
<span data-ttu-id="86db6-141">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="86db6-141">The following is an example of a response.</span></span>
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
