---
title: 删除对话线程
description: 删除 thread 对象。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f4e40763a1221575fbe45e8294aad0d2e0bdf764
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935785"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="4b0d1-103">删除对话线程</span><span class="sxs-lookup"><span data-stu-id="4b0d1-103">Delete conversation thread</span></span>

> <span data-ttu-id="4b0d1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4b0d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b0d1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4b0d1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b0d1-106">删除 [thread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4b0d1-106">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b0d1-107">权限</span><span class="sxs-lookup"><span data-stu-id="4b0d1-107">Permissions</span></span>
<span data-ttu-id="4b0d1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b0d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b0d1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b0d1-110">Permission type</span></span>      | <span data-ttu-id="4b0d1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b0d1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b0d1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b0d1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4b0d1-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b0d1-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b0d1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b0d1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b0d1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b0d1-115">Not supported.</span></span>    |
|<span data-ttu-id="4b0d1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b0d1-116">Application</span></span> | <span data-ttu-id="4b0d1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b0d1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b0d1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b0d1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4b0d1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b0d1-119">Request headers</span></span>
| <span data-ttu-id="4b0d1-120">名称</span><span class="sxs-lookup"><span data-stu-id="4b0d1-120">Name</span></span>       | <span data-ttu-id="4b0d1-121">类型</span><span class="sxs-lookup"><span data-stu-id="4b0d1-121">Type</span></span> | <span data-ttu-id="4b0d1-122">说明</span><span class="sxs-lookup"><span data-stu-id="4b0d1-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4b0d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b0d1-123">Authorization</span></span>  | <span data-ttu-id="4b0d1-124">string</span><span class="sxs-lookup"><span data-stu-id="4b0d1-124">string</span></span>  | <span data-ttu-id="4b0d1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b0d1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b0d1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b0d1-127">Request body</span></span>
<span data-ttu-id="4b0d1-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b0d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b0d1-129">响应</span><span class="sxs-lookup"><span data-stu-id="4b0d1-129">Response</span></span>
<span data-ttu-id="4b0d1-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4b0d1-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b0d1-132">示例</span><span class="sxs-lookup"><span data-stu-id="4b0d1-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4b0d1-133">请求</span><span class="sxs-lookup"><span data-stu-id="4b0d1-133">Request</span></span>
<span data-ttu-id="4b0d1-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4b0d1-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="4b0d1-135">响应</span><span class="sxs-lookup"><span data-stu-id="4b0d1-135">Response</span></span>
<span data-ttu-id="4b0d1-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4b0d1-136">The following is an example of the response.</span></span> 
><span data-ttu-id="4b0d1-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4b0d1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
