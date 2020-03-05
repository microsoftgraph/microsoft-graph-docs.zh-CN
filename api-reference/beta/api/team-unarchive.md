---
title: 解档团队
description: 还原存档的团队。 这将恢复用户发送邮件和编辑团队的能力，abiding 受租户和团队设置的支持。 使用存档 API 存档团队。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cc443242432199217c91d018e2a891fd21eb235c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452559"
---
# <a name="unarchive-team"></a><span data-ttu-id="e62dd-105">解档团队</span><span class="sxs-lookup"><span data-stu-id="e62dd-105">Unarchive team</span></span>

<span data-ttu-id="e62dd-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e62dd-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e62dd-107">还原存档的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="e62dd-107">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="e62dd-108">这将恢复用户发送邮件和编辑团队的能力，abiding 受租户和团队设置的支持。</span><span class="sxs-lookup"><span data-stu-id="e62dd-108">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="e62dd-109">使用[存档](team-archive.md)API 存档团队。</span><span class="sxs-lookup"><span data-stu-id="e62dd-109">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="e62dd-110">Unarchiving 是一种异步操作。</span><span class="sxs-lookup"><span data-stu-id="e62dd-110">Unarchiving is an async operation.</span></span> <span data-ttu-id="e62dd-111">异步操作成功完成后，团队即为 unarchived，这可能会在此 API 的响应之后发生。</span><span class="sxs-lookup"><span data-stu-id="e62dd-111">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="e62dd-112">权限</span><span class="sxs-lookup"><span data-stu-id="e62dd-112">Permissions</span></span>
<span data-ttu-id="e62dd-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e62dd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e62dd-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="e62dd-115">Permission type</span></span>      | <span data-ttu-id="e62dd-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e62dd-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e62dd-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e62dd-117">Delegated (work or school account)</span></span> | <span data-ttu-id="e62dd-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e62dd-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e62dd-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e62dd-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e62dd-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="e62dd-120">Not supported.</span></span>    |
|<span data-ttu-id="e62dd-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="e62dd-121">Application</span></span> | <span data-ttu-id="e62dd-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e62dd-122">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="e62dd-123">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="e62dd-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e62dd-124">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="e62dd-124">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e62dd-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e62dd-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="e62dd-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="e62dd-126">Request headers</span></span>
| <span data-ttu-id="e62dd-127">标头</span><span class="sxs-lookup"><span data-stu-id="e62dd-127">Header</span></span>       | <span data-ttu-id="e62dd-128">值</span><span class="sxs-lookup"><span data-stu-id="e62dd-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e62dd-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="e62dd-129">Authorization</span></span>  | <span data-ttu-id="e62dd-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e62dd-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e62dd-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="e62dd-132">Request body</span></span>
<span data-ttu-id="e62dd-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e62dd-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e62dd-134">响应</span><span class="sxs-lookup"><span data-stu-id="e62dd-134">Response</span></span>

<span data-ttu-id="e62dd-135">如果 unarchiving 成功启动，此方法将`202 Accepted`返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="e62dd-135">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="e62dd-136">该响应还将包含一个`Location`标头，其中包含为处理团队的 unarchiving 而创建的[teamsAsyncOperation](../resources/teamsasyncoperation.md)的位置。</span><span class="sxs-lookup"><span data-stu-id="e62dd-136">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="e62dd-137">通过向此位置发出 GET 请求，检查 unarchiving 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="e62dd-137">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="e62dd-138">示例</span><span class="sxs-lookup"><span data-stu-id="e62dd-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e62dd-139">请求</span><span class="sxs-lookup"><span data-stu-id="e62dd-139">Request</span></span>
<span data-ttu-id="e62dd-140">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="e62dd-140">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="e62dd-141">响应</span><span class="sxs-lookup"><span data-stu-id="e62dd-141">Response</span></span>
<span data-ttu-id="e62dd-142">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="e62dd-142">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
