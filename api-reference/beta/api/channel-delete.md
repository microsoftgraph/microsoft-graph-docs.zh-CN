---
title: 删除频道
description: 删除频道。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 12fe7fea8eca554c956facdba942f9af4a18ea3c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864663"
---
# <a name="delete-channel"></a><span data-ttu-id="1a0c4-103">删除频道</span><span class="sxs-lookup"><span data-stu-id="1a0c4-103">Delete channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a0c4-104">删除[频道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="1a0c4-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="1a0c4-105">**请注意**：应用程序权限和此 API 存在已知问题。</span><span class="sxs-lookup"><span data-stu-id="1a0c4-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="1a0c4-106">有关详细信息，请参阅[已知问题列表](/graph/known-issues#application-permissions)。</span><span class="sxs-lookup"><span data-stu-id="1a0c4-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a0c4-107">权限</span><span class="sxs-lookup"><span data-stu-id="1a0c4-107">Permissions</span></span>
<span data-ttu-id="1a0c4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a0c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a0c4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a0c4-110">Permission type</span></span>      | <span data-ttu-id="1a0c4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a0c4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a0c4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a0c4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1a0c4-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a0c4-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1a0c4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a0c4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a0c4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a0c4-115">Not supported.</span></span>    |
|<span data-ttu-id="1a0c4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a0c4-116">Application</span></span> | <span data-ttu-id="1a0c4-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a0c4-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="1a0c4-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="1a0c4-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1a0c4-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="1a0c4-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1a0c4-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a0c4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1a0c4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a0c4-121">Request headers</span></span>
| <span data-ttu-id="1a0c4-122">标头</span><span class="sxs-lookup"><span data-stu-id="1a0c4-122">Header</span></span>       | <span data-ttu-id="1a0c4-123">值</span><span class="sxs-lookup"><span data-stu-id="1a0c4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1a0c4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a0c4-124">Authorization</span></span>  | <span data-ttu-id="1a0c4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a0c4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1a0c4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a0c4-127">Request body</span></span>
<span data-ttu-id="1a0c4-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a0c4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a0c4-129">响应</span><span class="sxs-lookup"><span data-stu-id="1a0c4-129">Response</span></span>

<span data-ttu-id="1a0c4-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1a0c4-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a0c4-132">示例</span><span class="sxs-lookup"><span data-stu-id="1a0c4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a0c4-133">请求</span><span class="sxs-lookup"><span data-stu-id="1a0c4-133">Request</span></span>
<span data-ttu-id="1a0c4-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1a0c4-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1a0c4-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1a0c4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a0c4-136">C#</span><span class="sxs-lookup"><span data-stu-id="1a0c4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a0c4-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a0c4-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a0c4-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="1a0c4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1a0c4-139">Java</span><span class="sxs-lookup"><span data-stu-id="1a0c4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1a0c4-140">响应</span><span class="sxs-lookup"><span data-stu-id="1a0c4-140">Response</span></span>

<span data-ttu-id="1a0c4-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1a0c4-141">The following is an example of the response.</span></span> 
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
