---
title: 删除频道
description: 删除频道。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0e488c24d598a61bf3448ab80acfcbaf133aedc2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273694"
---
# <a name="delete-channel"></a><span data-ttu-id="88c5a-103">删除频道</span><span class="sxs-lookup"><span data-stu-id="88c5a-103">Delete channel</span></span>



<span data-ttu-id="88c5a-104">删除[频道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="88c5a-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="88c5a-105">**请注意**：应用程序权限和此 API 存在已知问题。</span><span class="sxs-lookup"><span data-stu-id="88c5a-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="88c5a-106">有关详细信息，请参阅[已知问题列表](/graph/known-issues#application-permissions)。</span><span class="sxs-lookup"><span data-stu-id="88c5a-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

> <span data-ttu-id="88c5a-107">**注意**: 已删除频道中的数据将继续存储几周, 以允许团队所有者恢复已删除的频道。</span><span class="sxs-lookup"><span data-stu-id="88c5a-107">**Note**: The data in deleted channels will continue to be stored for several weeks to allow team owner to recovery deleted channel.</span></span> <span data-ttu-id="88c5a-108">在这段时间内, 可能不会创建具有相同 displayName 的新通道。</span><span class="sxs-lookup"><span data-stu-id="88c5a-108">During that time, a new channel with the same displayName may not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="88c5a-109">权限</span><span class="sxs-lookup"><span data-stu-id="88c5a-109">Permissions</span></span>
<span data-ttu-id="88c5a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88c5a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88c5a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="88c5a-112">Permission type</span></span>      | <span data-ttu-id="88c5a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88c5a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88c5a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88c5a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="88c5a-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88c5a-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="88c5a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88c5a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88c5a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="88c5a-117">Not supported.</span></span>    |
|<span data-ttu-id="88c5a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="88c5a-118">Application</span></span> | <span data-ttu-id="88c5a-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88c5a-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="88c5a-120">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="88c5a-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="88c5a-121">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="88c5a-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="88c5a-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88c5a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="88c5a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="88c5a-123">Request headers</span></span>
| <span data-ttu-id="88c5a-124">标头</span><span class="sxs-lookup"><span data-stu-id="88c5a-124">Header</span></span>       | <span data-ttu-id="88c5a-125">值</span><span class="sxs-lookup"><span data-stu-id="88c5a-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="88c5a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="88c5a-126">Authorization</span></span>  | <span data-ttu-id="88c5a-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88c5a-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="88c5a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="88c5a-129">Request body</span></span>
<span data-ttu-id="88c5a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88c5a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88c5a-131">响应</span><span class="sxs-lookup"><span data-stu-id="88c5a-131">Response</span></span>

<span data-ttu-id="88c5a-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="88c5a-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="88c5a-134">示例</span><span class="sxs-lookup"><span data-stu-id="88c5a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88c5a-135">请求</span><span class="sxs-lookup"><span data-stu-id="88c5a-135">Request</span></span>
<span data-ttu-id="88c5a-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="88c5a-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="88c5a-137">响应</span><span class="sxs-lookup"><span data-stu-id="88c5a-137">Response</span></span>

<span data-ttu-id="88c5a-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="88c5a-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="88c5a-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="88c5a-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="88c5a-140">C#</span><span class="sxs-lookup"><span data-stu-id="88c5a-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_channel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="88c5a-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="88c5a-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_channel-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="88c5a-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="88c5a-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_channel-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/channel-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/channel-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/channel-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
