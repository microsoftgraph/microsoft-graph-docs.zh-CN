---
title: Unarchive 团队
description: 还原存档的团队。 这将还原发送消息和编辑团队，遵守租户和工作组设置用户的功能。 工作组已存档使用存档 API。
ms.openlocfilehash: 7507a58ef75939110d0c740e20d8540838bda204
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222609"
---
# <a name="unarchive-team"></a><span data-ttu-id="3e31d-105">Unarchive 团队</span><span class="sxs-lookup"><span data-stu-id="3e31d-105">Unarchive team</span></span>



<span data-ttu-id="3e31d-106">还原存档的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="3e31d-106">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="3e31d-107">这将还原发送消息和编辑团队，遵守租户和工作组设置用户的功能。</span><span class="sxs-lookup"><span data-stu-id="3e31d-107">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="3e31d-108">工作组已存档使用[存档](team-archive.md)API。</span><span class="sxs-lookup"><span data-stu-id="3e31d-108">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="3e31d-109">Unarchiving 是异步操作。</span><span class="sxs-lookup"><span data-stu-id="3e31d-109">Unarchiving is an async operation.</span></span> <span data-ttu-id="3e31d-110">一旦异步操作已成功完成，此 API 响应后可能出现的团队未存档。</span><span class="sxs-lookup"><span data-stu-id="3e31d-110">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e31d-111">权限</span><span class="sxs-lookup"><span data-stu-id="3e31d-111">Permissions</span></span>
<span data-ttu-id="3e31d-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e31d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e31d-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e31d-114">Permission type</span></span>      | <span data-ttu-id="3e31d-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e31d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e31d-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e31d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="3e31d-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e31d-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3e31d-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e31d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e31d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e31d-119">Not supported.</span></span>    |
|<span data-ttu-id="3e31d-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e31d-120">Application</span></span> | <span data-ttu-id="3e31d-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e31d-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="3e31d-122">**注意**： 此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="3e31d-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3e31d-123">全局管理员和 Microsoft 团队服务管理员可以访问团队它们不是的成员。</span><span class="sxs-lookup"><span data-stu-id="3e31d-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3e31d-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e31d-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="3e31d-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e31d-125">Request headers</span></span>
| <span data-ttu-id="3e31d-126">标头</span><span class="sxs-lookup"><span data-stu-id="3e31d-126">Header</span></span>       | <span data-ttu-id="3e31d-127">值</span><span class="sxs-lookup"><span data-stu-id="3e31d-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3e31d-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e31d-128">Authorization</span></span>  | <span data-ttu-id="3e31d-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e31d-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e31d-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e31d-131">Request body</span></span>
<span data-ttu-id="3e31d-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3e31d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e31d-133">响应</span><span class="sxs-lookup"><span data-stu-id="3e31d-133">Response</span></span>

<span data-ttu-id="3e31d-134">如果 unarchiving 已成功启动，此方法返回`202 Accepted`响应代码。</span><span class="sxs-lookup"><span data-stu-id="3e31d-134">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="3e31d-135">响应还将包含`Location`标头，其中包含的[teamsAsyncOperation](../resources/teamsasyncoperation.md)创建处理 unarchiving 团队的位置。</span><span class="sxs-lookup"><span data-stu-id="3e31d-135">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="3e31d-136">通过对此位置进行 GET 请求检查 unarchiving 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="3e31d-136">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="3e31d-137">示例</span><span class="sxs-lookup"><span data-stu-id="3e31d-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3e31d-138">请求</span><span class="sxs-lookup"><span data-stu-id="3e31d-138">Request</span></span>
<span data-ttu-id="3e31d-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3e31d-139">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="3e31d-140">响应</span><span class="sxs-lookup"><span data-stu-id="3e31d-140">Response</span></span>
<span data-ttu-id="3e31d-141">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="3e31d-141">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
