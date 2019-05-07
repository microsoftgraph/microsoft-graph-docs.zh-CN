---
title: 删除对话
description: 删除 conversation 对象。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 03a33f834083766c081fc99a696bcb2cf4c1c651
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614832"
---
# <a name="delete-conversation"></a><span data-ttu-id="14725-103">删除对话</span><span class="sxs-lookup"><span data-stu-id="14725-103">Delete conversation</span></span>
<span data-ttu-id="14725-104">删除 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14725-104">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="14725-105">权限</span><span class="sxs-lookup"><span data-stu-id="14725-105">Permissions</span></span>
<span data-ttu-id="14725-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14725-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14725-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="14725-108">Permission type</span></span>      | <span data-ttu-id="14725-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14725-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14725-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14725-110">Delegated (work or school account)</span></span> | <span data-ttu-id="14725-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14725-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="14725-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14725-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14725-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="14725-113">Not supported.</span></span>    |
|<span data-ttu-id="14725-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="14725-114">Application</span></span> | <span data-ttu-id="14725-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="14725-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="14725-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14725-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="14725-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="14725-117">Request headers</span></span>
| <span data-ttu-id="14725-118">名称</span><span class="sxs-lookup"><span data-stu-id="14725-118">Name</span></span>       | <span data-ttu-id="14725-119">类型</span><span class="sxs-lookup"><span data-stu-id="14725-119">Type</span></span> | <span data-ttu-id="14725-120">说明</span><span class="sxs-lookup"><span data-stu-id="14725-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="14725-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="14725-121">Authorization</span></span>  | <span data-ttu-id="14725-122">string</span><span class="sxs-lookup"><span data-stu-id="14725-122">string</span></span>  | <span data-ttu-id="14725-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14725-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14725-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="14725-125">Request body</span></span>
<span data-ttu-id="14725-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="14725-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14725-127">响应</span><span class="sxs-lookup"><span data-stu-id="14725-127">Response</span></span>
<span data-ttu-id="14725-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="14725-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14725-130">示例</span><span class="sxs-lookup"><span data-stu-id="14725-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="14725-131">请求</span><span class="sxs-lookup"><span data-stu-id="14725-131">Request</span></span>
<span data-ttu-id="14725-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="14725-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="14725-133">响应</span><span class="sxs-lookup"><span data-stu-id="14725-133">Response</span></span>
<span data-ttu-id="14725-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="14725-134">The following is an example of the response.</span></span> 
><span data-ttu-id="14725-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="14725-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="14725-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="14725-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="14725-138">语言</span><span class="sxs-lookup"><span data-stu-id="14725-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_group_conversation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="14725-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="14725-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_group_conversation-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/group-delete-conversation.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-delete-conversation.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
