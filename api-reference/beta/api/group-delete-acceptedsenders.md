---
title: 删除 acceptedSender
description: '从 acceptedSenders 列表中删除用户或组。 '
author: dkershaw10
ms.openlocfilehash: 7028f2f63e340c9f5c3f300f6e3724a05f87d288
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313907"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="4b015-103">删除 acceptedSender</span><span class="sxs-lookup"><span data-stu-id="4b015-103">Remove acceptedSender</span></span>

> <span data-ttu-id="4b015-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4b015-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b015-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4b015-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b015-106">从 acceptedSenders 列表中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="4b015-106">Remove a user or group from the acceptedSenders list.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4b015-107">权限</span><span class="sxs-lookup"><span data-stu-id="4b015-107">Permissions</span></span>
<span data-ttu-id="4b015-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b015-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b015-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b015-110">Permission type</span></span>                        | <span data-ttu-id="4b015-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b015-111">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="4b015-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b015-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b015-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b015-113">Group.ReadWrite.All</span></span>    |
| <span data-ttu-id="4b015-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b015-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b015-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b015-115">Not supported.</span></span>|
| <span data-ttu-id="4b015-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b015-116">Application</span></span>                            | <span data-ttu-id="4b015-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b015-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b015-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b015-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id=<id>
```

## <a name="request-headers"></a><span data-ttu-id="4b015-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b015-119">Request headers</span></span>
| <span data-ttu-id="4b015-120">标头</span><span class="sxs-lookup"><span data-stu-id="4b015-120">Header</span></span>         | <span data-ttu-id="4b015-121">值</span><span class="sxs-lookup"><span data-stu-id="4b015-121">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="4b015-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b015-122">Authorization</span></span>  | <span data-ttu-id="4b015-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b015-p103">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="4b015-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b015-125">Request body</span></span>
<span data-ttu-id="4b015-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b015-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b015-127">响应</span><span class="sxs-lookup"><span data-stu-id="4b015-127">Response</span></span>
<span data-ttu-id="4b015-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4b015-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b015-130">示例</span><span class="sxs-lookup"><span data-stu-id="4b015-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4b015-131">请求</span><span class="sxs-lookup"><span data-stu-id="4b015-131">Request</span></span>
<span data-ttu-id="4b015-132">下面展示了几个示例请求。</span><span class="sxs-lookup"><span data-stu-id="4b015-132">The following are a couple of examples of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}

DELETE https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="4b015-133">响应</span><span class="sxs-lookup"><span data-stu-id="4b015-133">Response</span></span>
<span data-ttu-id="4b015-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4b015-134">The following is an example of the response.</span></span> 

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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->