---
title: 存档团队
description: '存档指定的团队。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 594be32469abb7e75247936c9e32373ab3c3b95d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976371"
---
# <a name="archive-team"></a><span data-ttu-id="99ecc-103">存档团队</span><span class="sxs-lookup"><span data-stu-id="99ecc-103">Archive team</span></span>

<span data-ttu-id="99ecc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99ecc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99ecc-p101">Archive the specified [team](../resources/team.md). When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team. Membership changes to the team continue to be allowed.</span><span class="sxs-lookup"><span data-stu-id="99ecc-p101">Archive the specified [team](../resources/team.md). When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team. Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="99ecc-p102">Archiving is an async operation. A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span><span class="sxs-lookup"><span data-stu-id="99ecc-p102">Archiving is an async operation. A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="99ecc-110">要对团队存档，团队和[组](../resources/group.md)都必须有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="99ecc-110">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="99ecc-111">要从存档状态还原团队，请使用 API [取消存档](team-unarchive.md)。</span><span class="sxs-lookup"><span data-stu-id="99ecc-111">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="99ecc-112">权限</span><span class="sxs-lookup"><span data-stu-id="99ecc-112">Permissions</span></span>
<span data-ttu-id="99ecc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99ecc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99ecc-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="99ecc-115">Permission type</span></span>      | <span data-ttu-id="99ecc-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99ecc-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99ecc-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99ecc-117">Delegated (work or school account)</span></span> | <span data-ttu-id="99ecc-118">TeamSettings.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99ecc-118">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="99ecc-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99ecc-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99ecc-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="99ecc-120">Not supported.</span></span>    |
|<span data-ttu-id="99ecc-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="99ecc-121">Application</span></span> | <span data-ttu-id="99ecc-122">TeamSettings \*、TeamSettings、all、、all、所有读写。 all</span><span class="sxs-lookup"><span data-stu-id="99ecc-122">TeamSettings.ReadWrite.Group\*, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="99ecc-123">**注意** ：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="99ecc-123">**Note** : Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="99ecc-p104">**Note** : This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span><span class="sxs-lookup"><span data-stu-id="99ecc-p104">**Note** : This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="99ecc-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99ecc-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="99ecc-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="99ecc-127">Request headers</span></span>
| <span data-ttu-id="99ecc-128">标头</span><span class="sxs-lookup"><span data-stu-id="99ecc-128">Header</span></span>       | <span data-ttu-id="99ecc-129">值</span><span class="sxs-lookup"><span data-stu-id="99ecc-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="99ecc-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="99ecc-130">Authorization</span></span>  | <span data-ttu-id="99ecc-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="99ecc-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="99ecc-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="99ecc-133">Request body</span></span>
<span data-ttu-id="99ecc-134">在请求中，可 _选择性地_ 在 JSON 正文中包括 `shouldSetSpoSiteReadOnlyForMembers` 参数，如下所示。</span><span class="sxs-lookup"><span data-stu-id="99ecc-134">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="99ecc-p106">This optional parameter defines whether to set permissions for team members to read-only on the SharePoint Online site associated with the team. Setting it to false or omitting the body altogether will result in this step being skipped.</span><span class="sxs-lookup"><span data-stu-id="99ecc-p106">This optional parameter defines whether to set permissions for team members to read-only on the SharePoint Online site associated with the team. Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="99ecc-137">响应</span><span class="sxs-lookup"><span data-stu-id="99ecc-137">Response</span></span>

<span data-ttu-id="99ecc-138">如果成功开始存档，此方法将返回一个 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="99ecc-138">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="99ecc-139">响应还将包含一个 `Location` 标头，后者包含创建用于处理团队存档操作的 [teamsAsyncOperation](../resources/teamsasyncoperation.md) 的位置。</span><span class="sxs-lookup"><span data-stu-id="99ecc-139">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="99ecc-140">可通过向此位置发出 GET 请求，查看存档操作的状态。</span><span class="sxs-lookup"><span data-stu-id="99ecc-140">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="99ecc-141">示例</span><span class="sxs-lookup"><span data-stu-id="99ecc-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="99ecc-142">请求</span><span class="sxs-lookup"><span data-stu-id="99ecc-142">Request</span></span>
<span data-ttu-id="99ecc-143">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="99ecc-143">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99ecc-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="99ecc-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
# <a name="c"></a>[<span data-ttu-id="99ecc-145">C#</span><span class="sxs-lookup"><span data-stu-id="99ecc-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/archive-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99ecc-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99ecc-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/archive-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99ecc-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99ecc-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/archive-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99ecc-148">Java</span><span class="sxs-lookup"><span data-stu-id="99ecc-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/archive-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="99ecc-149">响应</span><span class="sxs-lookup"><span data-stu-id="99ecc-149">Response</span></span>
<span data-ttu-id="99ecc-150">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="99ecc-150">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "name": "archive_team"
}-->
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


