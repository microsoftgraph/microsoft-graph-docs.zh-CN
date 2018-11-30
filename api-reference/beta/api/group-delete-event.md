---
title: 删除事件
description: 删除 event 对象。
ms.openlocfilehash: 41623ad938a37ba762e843ab007f772ac8ae7504
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048095"
---
# <a name="delete-event"></a><span data-ttu-id="9680f-103">删除事件</span><span class="sxs-lookup"><span data-stu-id="9680f-103">Delete event</span></span>

> <span data-ttu-id="9680f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9680f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9680f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9680f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9680f-106">删除 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9680f-106">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9680f-107">权限</span><span class="sxs-lookup"><span data-stu-id="9680f-107">Permissions</span></span>
<span data-ttu-id="9680f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9680f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9680f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9680f-110">Permission type</span></span>      | <span data-ttu-id="9680f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9680f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9680f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9680f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9680f-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9680f-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9680f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9680f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9680f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9680f-115">Not supported.</span></span>    |
|<span data-ttu-id="9680f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9680f-116">Application</span></span> | <span data-ttu-id="9680f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9680f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9680f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9680f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9680f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9680f-119">Request headers</span></span>
| <span data-ttu-id="9680f-120">名称</span><span class="sxs-lookup"><span data-stu-id="9680f-120">Name</span></span>       | <span data-ttu-id="9680f-121">类型</span><span class="sxs-lookup"><span data-stu-id="9680f-121">Type</span></span> | <span data-ttu-id="9680f-122">说明</span><span class="sxs-lookup"><span data-stu-id="9680f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9680f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9680f-123">Authorization</span></span>  | <span data-ttu-id="9680f-124">string</span><span class="sxs-lookup"><span data-stu-id="9680f-124">string</span></span>  | <span data-ttu-id="9680f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9680f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9680f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9680f-127">Request body</span></span>
<span data-ttu-id="9680f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9680f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9680f-129">响应</span><span class="sxs-lookup"><span data-stu-id="9680f-129">Response</span></span>
<span data-ttu-id="9680f-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9680f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9680f-132">示例</span><span class="sxs-lookup"><span data-stu-id="9680f-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9680f-133">请求</span><span class="sxs-lookup"><span data-stu-id="9680f-133">Request</span></span>
<span data-ttu-id="9680f-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9680f-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="9680f-135">响应</span><span class="sxs-lookup"><span data-stu-id="9680f-135">Response</span></span>
<span data-ttu-id="9680f-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9680f-136">The following is an example of the response.</span></span> 
><span data-ttu-id="9680f-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9680f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->