---
title: 删除对话
description: 删除 conversation 对象。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 8eda987cb30d4ffbdda32bf9df750c58f3b77f37
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859057"
---
# <a name="delete-conversation"></a><span data-ttu-id="297f7-103">删除对话</span><span class="sxs-lookup"><span data-stu-id="297f7-103">Delete conversation</span></span>

> <span data-ttu-id="297f7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="297f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="297f7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="297f7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="297f7-106">删除 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="297f7-106">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="297f7-107">权限</span><span class="sxs-lookup"><span data-stu-id="297f7-107">Permissions</span></span>
<span data-ttu-id="297f7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="297f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="297f7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="297f7-110">Permission type</span></span>      | <span data-ttu-id="297f7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="297f7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="297f7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="297f7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="297f7-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="297f7-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="297f7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="297f7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="297f7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="297f7-115">Not supported.</span></span>    |
|<span data-ttu-id="297f7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="297f7-116">Application</span></span> | <span data-ttu-id="297f7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="297f7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="297f7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="297f7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="297f7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="297f7-119">Request headers</span></span>
| <span data-ttu-id="297f7-120">名称</span><span class="sxs-lookup"><span data-stu-id="297f7-120">Name</span></span>       | <span data-ttu-id="297f7-121">类型</span><span class="sxs-lookup"><span data-stu-id="297f7-121">Type</span></span> | <span data-ttu-id="297f7-122">说明</span><span class="sxs-lookup"><span data-stu-id="297f7-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="297f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="297f7-123">Authorization</span></span>  | <span data-ttu-id="297f7-124">string</span><span class="sxs-lookup"><span data-stu-id="297f7-124">string</span></span>  | <span data-ttu-id="297f7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="297f7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="297f7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="297f7-127">Request body</span></span>
<span data-ttu-id="297f7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="297f7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="297f7-129">响应</span><span class="sxs-lookup"><span data-stu-id="297f7-129">Response</span></span>
<span data-ttu-id="297f7-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="297f7-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="297f7-132">示例</span><span class="sxs-lookup"><span data-stu-id="297f7-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="297f7-133">请求</span><span class="sxs-lookup"><span data-stu-id="297f7-133">Request</span></span>
<span data-ttu-id="297f7-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="297f7-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="297f7-135">响应</span><span class="sxs-lookup"><span data-stu-id="297f7-135">Response</span></span>
<span data-ttu-id="297f7-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="297f7-136">The following is an example of the response.</span></span> 
><span data-ttu-id="297f7-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="297f7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
