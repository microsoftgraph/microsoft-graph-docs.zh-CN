---
title: 删除频道
description: 删除频道。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b6a2e1f8c0eef45e227affdf0d73417ee90992b8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003880"
---
# <a name="delete-channel"></a><span data-ttu-id="73dee-103">删除频道</span><span class="sxs-lookup"><span data-stu-id="73dee-103">Delete channel</span></span>



<span data-ttu-id="73dee-104">删除[频道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="73dee-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="73dee-105">**请注意**：应用程序权限和此 API 存在已知问题。</span><span class="sxs-lookup"><span data-stu-id="73dee-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="73dee-106">有关详细信息，请参阅[已知问题列表](/graph/known-issues#application-permissions)。</span><span class="sxs-lookup"><span data-stu-id="73dee-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

> <span data-ttu-id="73dee-107">**注意**: 已删除频道中的数据将继续存储几周, 以允许团队所有者恢复已删除的频道。</span><span class="sxs-lookup"><span data-stu-id="73dee-107">**Note**: The data in deleted channels will continue to be stored for several weeks to allow team owner to recovery deleted channel.</span></span> <span data-ttu-id="73dee-108">在这段时间内, 可能不会创建具有相同 displayName 的新通道。</span><span class="sxs-lookup"><span data-stu-id="73dee-108">During that time, a new channel with the same displayName may not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="73dee-109">权限</span><span class="sxs-lookup"><span data-stu-id="73dee-109">Permissions</span></span>
<span data-ttu-id="73dee-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73dee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73dee-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="73dee-112">Permission type</span></span>      | <span data-ttu-id="73dee-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73dee-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73dee-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73dee-114">Delegated (work or school account)</span></span> | <span data-ttu-id="73dee-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73dee-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="73dee-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73dee-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73dee-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="73dee-117">Not supported.</span></span>    |
|<span data-ttu-id="73dee-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="73dee-118">Application</span></span> | <span data-ttu-id="73dee-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73dee-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="73dee-120">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="73dee-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="73dee-121">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="73dee-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="73dee-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73dee-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="73dee-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="73dee-123">Request headers</span></span>
| <span data-ttu-id="73dee-124">标头</span><span class="sxs-lookup"><span data-stu-id="73dee-124">Header</span></span>       | <span data-ttu-id="73dee-125">值</span><span class="sxs-lookup"><span data-stu-id="73dee-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73dee-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="73dee-126">Authorization</span></span>  | <span data-ttu-id="73dee-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73dee-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="73dee-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="73dee-129">Request body</span></span>
<span data-ttu-id="73dee-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73dee-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73dee-131">响应</span><span class="sxs-lookup"><span data-stu-id="73dee-131">Response</span></span>

<span data-ttu-id="73dee-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="73dee-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="73dee-134">示例</span><span class="sxs-lookup"><span data-stu-id="73dee-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73dee-135">请求</span><span class="sxs-lookup"><span data-stu-id="73dee-135">Request</span></span>
<span data-ttu-id="73dee-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="73dee-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="73dee-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="73dee-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73dee-138">C#</span><span class="sxs-lookup"><span data-stu-id="73dee-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73dee-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="73dee-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73dee-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="73dee-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="73dee-141">Java</span><span class="sxs-lookup"><span data-stu-id="73dee-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="73dee-142">响应</span><span class="sxs-lookup"><span data-stu-id="73dee-142">Response</span></span>

<span data-ttu-id="73dee-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="73dee-143">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
