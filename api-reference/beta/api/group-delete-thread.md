---
title: 删除对话线程
description: 删除 thread 对象。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f4da21812bf7fb77f1c377b8d26e6857302447c0
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681800"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="bfdfe-103">删除对话线程</span><span class="sxs-lookup"><span data-stu-id="bfdfe-103">Delete conversation thread</span></span>

<span data-ttu-id="bfdfe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfdfe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfdfe-105">删除 [thread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bfdfe-105">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfdfe-106">权限</span><span class="sxs-lookup"><span data-stu-id="bfdfe-106">Permissions</span></span>
<span data-ttu-id="bfdfe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bfdfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfdfe-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfdfe-109">Permission type</span></span>      | <span data-ttu-id="bfdfe-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bfdfe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfdfe-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfdfe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bfdfe-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfdfe-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bfdfe-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfdfe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfdfe-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfdfe-114">Not supported.</span></span>    |
|<span data-ttu-id="bfdfe-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfdfe-115">Application</span></span> | <span data-ttu-id="bfdfe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfdfe-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfdfe-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfdfe-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bfdfe-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfdfe-118">Request headers</span></span>
| <span data-ttu-id="bfdfe-119">名称</span><span class="sxs-lookup"><span data-stu-id="bfdfe-119">Name</span></span>       | <span data-ttu-id="bfdfe-120">类型</span><span class="sxs-lookup"><span data-stu-id="bfdfe-120">Type</span></span> | <span data-ttu-id="bfdfe-121">说明</span><span class="sxs-lookup"><span data-stu-id="bfdfe-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bfdfe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfdfe-122">Authorization</span></span>  | <span data-ttu-id="bfdfe-123">string</span><span class="sxs-lookup"><span data-stu-id="bfdfe-123">string</span></span>  | <span data-ttu-id="bfdfe-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bfdfe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfdfe-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfdfe-126">Request body</span></span>
<span data-ttu-id="bfdfe-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bfdfe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfdfe-128">响应</span><span class="sxs-lookup"><span data-stu-id="bfdfe-128">Response</span></span>
<span data-ttu-id="bfdfe-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bfdfe-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfdfe-131">示例</span><span class="sxs-lookup"><span data-stu-id="bfdfe-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bfdfe-132">请求</span><span class="sxs-lookup"><span data-stu-id="bfdfe-132">Request</span></span>
<span data-ttu-id="bfdfe-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bfdfe-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bfdfe-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfdfe-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```
# <a name="c"></a>[<span data-ttu-id="bfdfe-135">C#</span><span class="sxs-lookup"><span data-stu-id="bfdfe-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-thread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfdfe-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfdfe-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfdfe-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfdfe-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-thread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bfdfe-138">Java</span><span class="sxs-lookup"><span data-stu-id="bfdfe-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-thread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bfdfe-139">响应</span><span class="sxs-lookup"><span data-stu-id="bfdfe-139">Response</span></span>
<span data-ttu-id="bfdfe-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bfdfe-140">The following is an example of the response.</span></span> 
><span data-ttu-id="bfdfe-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bfdfe-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Delete conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


