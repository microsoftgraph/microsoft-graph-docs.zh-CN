---
title: 删除频道
description: 删除频道。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1e2b1a6818a6b1a618d448aad2d04a9f063689d1
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289472"
---
# <a name="delete-channel"></a><span data-ttu-id="9cf41-103">删除频道</span><span class="sxs-lookup"><span data-stu-id="9cf41-103">Delete channel</span></span>

<span data-ttu-id="9cf41-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cf41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cf41-105">删除[频道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="9cf41-105">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="9cf41-106">**请注意**：应用程序权限和此 API 存在已知问题。</span><span class="sxs-lookup"><span data-stu-id="9cf41-106">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="9cf41-107">有关详细信息，请参阅[已知问题列表](/graph/known-issues#application-permissions)。</span><span class="sxs-lookup"><span data-stu-id="9cf41-107">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="9cf41-108">权限</span><span class="sxs-lookup"><span data-stu-id="9cf41-108">Permissions</span></span>
<span data-ttu-id="9cf41-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cf41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cf41-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cf41-111">Permission type</span></span>      | <span data-ttu-id="9cf41-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cf41-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cf41-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cf41-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9cf41-114">All、Group、all、All、All</span><span class="sxs-lookup"><span data-stu-id="9cf41-114">Channel.Delete.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="9cf41-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cf41-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cf41-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cf41-116">Not supported.</span></span>    |
|<span data-ttu-id="9cf41-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cf41-117">Application</span></span> | <span data-ttu-id="9cf41-118">除 "全部"、"删除"、"组"[RSC](https://aka.ms/teams-rsc)、"组"、"全部"、"所有"、"</span><span class="sxs-lookup"><span data-stu-id="9cf41-118">Channel.Delete.All, Channel.Delete.Group ([RSC](https://aka.ms/teams-rsc)), Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="9cf41-119">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="9cf41-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9cf41-120">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="9cf41-120">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9cf41-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cf41-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9cf41-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cf41-122">Request headers</span></span>
| <span data-ttu-id="9cf41-123">标头</span><span class="sxs-lookup"><span data-stu-id="9cf41-123">Header</span></span>       | <span data-ttu-id="9cf41-124">值</span><span class="sxs-lookup"><span data-stu-id="9cf41-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9cf41-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cf41-125">Authorization</span></span>  | <span data-ttu-id="9cf41-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cf41-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9cf41-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cf41-128">Request body</span></span>
<span data-ttu-id="9cf41-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9cf41-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cf41-130">响应</span><span class="sxs-lookup"><span data-stu-id="9cf41-130">Response</span></span>

<span data-ttu-id="9cf41-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9cf41-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9cf41-133">示例</span><span class="sxs-lookup"><span data-stu-id="9cf41-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cf41-134">请求</span><span class="sxs-lookup"><span data-stu-id="9cf41-134">Request</span></span>
<span data-ttu-id="9cf41-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9cf41-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9cf41-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cf41-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="c"></a>[<span data-ttu-id="9cf41-137">C#</span><span class="sxs-lookup"><span data-stu-id="9cf41-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cf41-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cf41-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cf41-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cf41-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9cf41-140">响应</span><span class="sxs-lookup"><span data-stu-id="9cf41-140">Response</span></span>

<span data-ttu-id="9cf41-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9cf41-141">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
