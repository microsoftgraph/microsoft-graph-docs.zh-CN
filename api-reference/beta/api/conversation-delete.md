---
title: 删除对话
description: 删除对话。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7fc4c8d1d3f32cce54ae99687f23e5543be50017
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591223"
---
# <a name="delete-conversation"></a><span data-ttu-id="ad40d-103">删除对话</span><span class="sxs-lookup"><span data-stu-id="ad40d-103">Delete conversation</span></span>

<span data-ttu-id="ad40d-104">删除对话。</span><span class="sxs-lookup"><span data-stu-id="ad40d-104">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="ad40d-105">权限</span><span class="sxs-lookup"><span data-stu-id="ad40d-105">Permissions</span></span>
<span data-ttu-id="ad40d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad40d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad40d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad40d-108">Permission type</span></span>      | <span data-ttu-id="ad40d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad40d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad40d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad40d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad40d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad40d-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad40d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad40d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad40d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad40d-113">Not supported.</span></span>    |
|<span data-ttu-id="ad40d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad40d-114">Application</span></span> | <span data-ttu-id="ad40d-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad40d-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad40d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad40d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ad40d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad40d-117">Request headers</span></span>
| <span data-ttu-id="ad40d-118">标头</span><span class="sxs-lookup"><span data-stu-id="ad40d-118">Header</span></span>       | <span data-ttu-id="ad40d-119">值</span><span class="sxs-lookup"><span data-stu-id="ad40d-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ad40d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad40d-120">Authorization</span></span>  | <span data-ttu-id="ad40d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ad40d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ad40d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad40d-123">Request body</span></span>
<span data-ttu-id="ad40d-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ad40d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad40d-125">响应</span><span class="sxs-lookup"><span data-stu-id="ad40d-125">Response</span></span>

<span data-ttu-id="ad40d-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ad40d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad40d-128">示例</span><span class="sxs-lookup"><span data-stu-id="ad40d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad40d-129">请求</span><span class="sxs-lookup"><span data-stu-id="ad40d-129">Request</span></span>
<span data-ttu-id="ad40d-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ad40d-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
##### <a name="response"></a><span data-ttu-id="ad40d-131">响应</span><span class="sxs-lookup"><span data-stu-id="ad40d-131">Response</span></span>
<span data-ttu-id="ad40d-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ad40d-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ad40d-133">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ad40d-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ad40d-134">语言</span><span class="sxs-lookup"><span data-stu-id="ad40d-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_conversation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad40d-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="ad40d-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_conversation-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/conversation-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/conversation-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
