---
title: 存档团队
description: '存档指定的团队。 '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 984fbd7692f28ab2ebf8f3be0411447b51bf2d13
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866190"
---
# <a name="archive-team"></a><span data-ttu-id="df75d-103">存档团队</span><span class="sxs-lookup"><span data-stu-id="df75d-103">Archive team</span></span>

> <span data-ttu-id="df75d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="df75d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df75d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="df75d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df75d-106">存档指定的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="df75d-106">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="df75d-107">团队存档时，用户可以不再发送或团队中的任何频道上的邮件，类似编辑工作组的名称、 说明或其他设置，或通常对团队大多数的更改。</span><span class="sxs-lookup"><span data-stu-id="df75d-107">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="df75d-108">向团队的成员身份更改继续允许。</span><span class="sxs-lookup"><span data-stu-id="df75d-108">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="df75d-109">存档是异步操作。</span><span class="sxs-lookup"><span data-stu-id="df75d-109">Archiving is an async operation.</span></span> <span data-ttu-id="df75d-110">一旦异步操作已成功完成，此 API 响应后可能出现的存档团队。</span><span class="sxs-lookup"><span data-stu-id="df75d-110">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="df75d-111">才能存档团队，团队和[组](../resources/group.md)必须具有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="df75d-111">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="df75d-112">若要从其存档状态还原团队，使用 API 对[unarchive](team-unarchive.md)。</span><span class="sxs-lookup"><span data-stu-id="df75d-112">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="df75d-113">权限</span><span class="sxs-lookup"><span data-stu-id="df75d-113">Permissions</span></span>
<span data-ttu-id="df75d-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df75d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df75d-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="df75d-116">Permission type</span></span>      | <span data-ttu-id="df75d-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df75d-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df75d-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df75d-118">Delegated (work or school account)</span></span> | <span data-ttu-id="df75d-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df75d-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="df75d-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df75d-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df75d-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="df75d-121">Not supported.</span></span>    |
|<span data-ttu-id="df75d-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="df75d-122">Application</span></span> | <span data-ttu-id="df75d-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df75d-123">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="df75d-124">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="df75d-124">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="df75d-125">全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。</span><span class="sxs-lookup"><span data-stu-id="df75d-125">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="df75d-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df75d-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="df75d-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="df75d-127">Request headers</span></span>
| <span data-ttu-id="df75d-128">标头</span><span class="sxs-lookup"><span data-stu-id="df75d-128">Header</span></span>       | <span data-ttu-id="df75d-129">值</span><span class="sxs-lookup"><span data-stu-id="df75d-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df75d-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="df75d-130">Authorization</span></span>  | <span data-ttu-id="df75d-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="df75d-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df75d-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="df75d-133">Request body</span></span>
<span data-ttu-id="df75d-134">在请求中，则可以_选择_包括`shouldSetSpoSiteReadOnlyForMembers`以 json 格式的参数正文，，如下所示。</span><span class="sxs-lookup"><span data-stu-id="df75d-134">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="df75d-135">此可选的参数定义是否与团队关联的 Sharepoint Online 网站上设置为只读的工作组成员的权限。</span><span class="sxs-lookup"><span data-stu-id="df75d-135">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="df75d-136">设置为 false 或省略正文完全将导致正在跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="df75d-136">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="df75d-137">响应</span><span class="sxs-lookup"><span data-stu-id="df75d-137">Response</span></span>

<span data-ttu-id="df75d-138">如果存档成功启动，此方法返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="df75d-138">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="df75d-139">响应还将包含`Location`标头，其中包含已创建以处理存档的团队[teamsAsyncOperation](../resources/teamsasyncoperation.md)的位置。</span><span class="sxs-lookup"><span data-stu-id="df75d-139">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="df75d-140">通过对此位置进行 GET 请求检查存档操作的状态。</span><span class="sxs-lookup"><span data-stu-id="df75d-140">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="df75d-141">示例</span><span class="sxs-lookup"><span data-stu-id="df75d-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="df75d-142">请求</span><span class="sxs-lookup"><span data-stu-id="df75d-142">Request</span></span>
<span data-ttu-id="df75d-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df75d-143">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="df75d-144">响应</span><span class="sxs-lookup"><span data-stu-id="df75d-144">Response</span></span>
<span data-ttu-id="df75d-145">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="df75d-145">The following is an example of a response.</span></span>
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
