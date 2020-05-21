---
title: 解档团队
description: 还原存档的团队。 这将恢复用户发送邮件和编辑团队的能力，abiding 受租户和团队设置的支持。 使用存档 API 存档团队。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 119ab415814a41402c87846bbcfb41f0e2bdb542
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333642"
---
# <a name="unarchive-team"></a><span data-ttu-id="68275-105">解档团队</span><span class="sxs-lookup"><span data-stu-id="68275-105">Unarchive team</span></span>

<span data-ttu-id="68275-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68275-106">Namespace: microsoft.graph</span></span>



<span data-ttu-id="68275-107">还原存档的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="68275-107">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="68275-108">这将恢复用户发送邮件和编辑团队的能力，abiding 受租户和团队设置的支持。</span><span class="sxs-lookup"><span data-stu-id="68275-108">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="68275-109">使用[存档](team-archive.md)API 存档团队。</span><span class="sxs-lookup"><span data-stu-id="68275-109">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="68275-110">Unarchiving 是一种异步操作。</span><span class="sxs-lookup"><span data-stu-id="68275-110">Unarchiving is an async operation.</span></span> <span data-ttu-id="68275-111">异步操作成功完成后，团队即为 unarchived，这可能会在此 API 的响应之后发生。</span><span class="sxs-lookup"><span data-stu-id="68275-111">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="68275-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="68275-112">Permissions</span></span>
<span data-ttu-id="68275-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68275-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68275-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="68275-115">Permission type</span></span>      | <span data-ttu-id="68275-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68275-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68275-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68275-117">Delegated (work or school account)</span></span> | <span data-ttu-id="68275-118">TeamSettings、Group 写全部、所有的 ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="68275-118">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="68275-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68275-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68275-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="68275-120">Not supported.</span></span>    |
|<span data-ttu-id="68275-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="68275-121">Application</span></span> | <span data-ttu-id="68275-122">TeamSettings （[RSC](https://aka.ms/teams-rsc)）、TeamSettings、All、group、All、All 和 All。 all</span><span class="sxs-lookup"><span data-stu-id="68275-122">TeamSettings.Edit.Group ([RSC](https://aka.ms/teams-rsc)), TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="68275-123">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="68275-123">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="68275-124">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="68275-124">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="68275-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68275-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="68275-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="68275-126">Request headers</span></span>
| <span data-ttu-id="68275-127">标头</span><span class="sxs-lookup"><span data-stu-id="68275-127">Header</span></span>       | <span data-ttu-id="68275-128">值</span><span class="sxs-lookup"><span data-stu-id="68275-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="68275-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="68275-129">Authorization</span></span>  | <span data-ttu-id="68275-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="68275-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="68275-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="68275-132">Request body</span></span>
<span data-ttu-id="68275-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="68275-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68275-134">响应</span><span class="sxs-lookup"><span data-stu-id="68275-134">Response</span></span>

<span data-ttu-id="68275-135">如果 unarchiving 成功启动，此方法将返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="68275-135">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="68275-136">该响应还将包含一个 `Location` 标头，其中包含为处理团队的 unarchiving 而创建的[teamsAsyncOperation](../resources/teamsasyncoperation.md)的位置。</span><span class="sxs-lookup"><span data-stu-id="68275-136">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="68275-137">通过向此位置发出 GET 请求，检查 unarchiving 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="68275-137">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="68275-138">示例</span><span class="sxs-lookup"><span data-stu-id="68275-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="68275-139">请求</span><span class="sxs-lookup"><span data-stu-id="68275-139">Request</span></span>
<span data-ttu-id="68275-140">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="68275-140">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="68275-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="68275-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/unarchive
```
# <a name="c"></a>[<span data-ttu-id="68275-142">C#</span><span class="sxs-lookup"><span data-stu-id="68275-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unarchive-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68275-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68275-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unarchive-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68275-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68275-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unarchive-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="68275-145">Java</span><span class="sxs-lookup"><span data-stu-id="68275-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unarchive-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="68275-146">响应</span><span class="sxs-lookup"><span data-stu-id="68275-146">Response</span></span>
<span data-ttu-id="68275-147">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="68275-147">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "name": "unarchive_team"
}-->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
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
