---
title: 删除对话线程
description: 删除 thread 对象。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 24e779b528391e82f452f7bbe3153e39a3975b93
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946754"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="96752-103">删除对话线程</span><span class="sxs-lookup"><span data-stu-id="96752-103">Delete conversation thread</span></span>
<span data-ttu-id="96752-104">删除 [thread](../resources/conversationthread.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="96752-104">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="96752-105">权限</span><span class="sxs-lookup"><span data-stu-id="96752-105">Permissions</span></span>
<span data-ttu-id="96752-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96752-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96752-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="96752-108">Permission type</span></span>      | <span data-ttu-id="96752-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96752-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96752-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96752-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96752-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96752-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="96752-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96752-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96752-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="96752-113">Not supported.</span></span>    |
|<span data-ttu-id="96752-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="96752-114">Application</span></span> | <span data-ttu-id="96752-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="96752-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96752-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96752-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="96752-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="96752-117">Request headers</span></span>
| <span data-ttu-id="96752-118">名称</span><span class="sxs-lookup"><span data-stu-id="96752-118">Name</span></span>       | <span data-ttu-id="96752-119">类型</span><span class="sxs-lookup"><span data-stu-id="96752-119">Type</span></span> | <span data-ttu-id="96752-120">说明</span><span class="sxs-lookup"><span data-stu-id="96752-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="96752-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="96752-121">Authorization</span></span>  | <span data-ttu-id="96752-122">string</span><span class="sxs-lookup"><span data-stu-id="96752-122">string</span></span>  | <span data-ttu-id="96752-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96752-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96752-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="96752-125">Request body</span></span>
<span data-ttu-id="96752-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96752-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96752-127">响应</span><span class="sxs-lookup"><span data-stu-id="96752-127">Response</span></span>
<span data-ttu-id="96752-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="96752-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96752-130">示例</span><span class="sxs-lookup"><span data-stu-id="96752-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="96752-131">请求</span><span class="sxs-lookup"><span data-stu-id="96752-131">Request</span></span>
<span data-ttu-id="96752-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="96752-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="96752-133">响应</span><span class="sxs-lookup"><span data-stu-id="96752-133">Response</span></span>
<span data-ttu-id="96752-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="96752-134">The following is an example of the response.</span></span> 
><span data-ttu-id="96752-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="96752-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
