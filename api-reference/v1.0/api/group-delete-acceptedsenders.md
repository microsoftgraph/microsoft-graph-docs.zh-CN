---
title: 删除 acceptedSender
description: '从接受的发件人列表中删除用户或组。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c2e098e88d4f855c5736f2e176b234f50a4e71b3
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614652"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="7fa8c-103">删除 acceptedSender</span><span class="sxs-lookup"><span data-stu-id="7fa8c-103">Remove acceptedSender</span></span>
<span data-ttu-id="7fa8c-104">从接受的发件人列表中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="7fa8c-104">Remove a user or group from the accepted-senders list.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7fa8c-105">权限</span><span class="sxs-lookup"><span data-stu-id="7fa8c-105">Permissions</span></span>
<span data-ttu-id="7fa8c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7fa8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7fa8c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7fa8c-108">Permission type</span></span>                        | <span data-ttu-id="7fa8c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7fa8c-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="7fa8c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7fa8c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7fa8c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fa8c-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="7fa8c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7fa8c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fa8c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fa8c-113">Not supported.</span></span> |
| <span data-ttu-id="7fa8c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7fa8c-114">Application</span></span>                            | <span data-ttu-id="7fa8c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fa8c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fa8c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7fa8c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
DELETE /groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/groups/{other-group-id}
```

## <a name="request-headers"></a><span data-ttu-id="7fa8c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7fa8c-117">Request headers</span></span>
| <span data-ttu-id="7fa8c-118">标头</span><span class="sxs-lookup"><span data-stu-id="7fa8c-118">Header</span></span>         | <span data-ttu-id="7fa8c-119">值</span><span class="sxs-lookup"><span data-stu-id="7fa8c-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="7fa8c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fa8c-120">Authorization</span></span>  | <span data-ttu-id="7fa8c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7fa8c-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="7fa8c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="7fa8c-123">Request body</span></span>
<span data-ttu-id="7fa8c-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7fa8c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fa8c-125">响应</span><span class="sxs-lookup"><span data-stu-id="7fa8c-125">Response</span></span>
<span data-ttu-id="7fa8c-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7fa8c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fa8c-128">示例</span><span class="sxs-lookup"><span data-stu-id="7fa8c-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7fa8c-129">请求</span><span class="sxs-lookup"><span data-stu-id="7fa8c-129">Request</span></span>
<span data-ttu-id="7fa8c-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7fa8c-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="7fa8c-131">响应</span><span class="sxs-lookup"><span data-stu-id="7fa8c-131">Response</span></span>
<span data-ttu-id="7fa8c-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7fa8c-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7fa8c-133">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7fa8c-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7fa8c-134">语言</span><span class="sxs-lookup"><span data-stu-id="7fa8c-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7fa8c-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="7fa8c-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-delete-acceptedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-delete-acceptedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
