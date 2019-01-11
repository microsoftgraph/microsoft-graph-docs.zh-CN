---
title: 删除 acceptedSender
description: 向 acceptedSender 列表中添加新用户或组。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: d450d7441429f6e40477570609a9b9689ebc0a28
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843461"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="7aa4e-103">删除 acceptedSender</span><span class="sxs-lookup"><span data-stu-id="7aa4e-103">Create acceptedSender</span></span>

> <span data-ttu-id="7aa4e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7aa4e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7aa4e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7aa4e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7aa4e-106">向 acceptedSender 列表中添加新用户或组。</span><span class="sxs-lookup"><span data-stu-id="7aa4e-106">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="7aa4e-p102">在请求主体的 `@odata.id` 中指定用户或组。已接受的发件人列表中的用户可以发布到组对话。确保未在接受的发件人和拒绝的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="7aa4e-p102">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="7aa4e-110">权限</span><span class="sxs-lookup"><span data-stu-id="7aa4e-110">Permissions</span></span>
<span data-ttu-id="7aa4e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7aa4e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aa4e-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="7aa4e-113">Permission type</span></span>      | <span data-ttu-id="7aa4e-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7aa4e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7aa4e-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7aa4e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7aa4e-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa4e-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7aa4e-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7aa4e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aa4e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7aa4e-118">Not supported.</span></span>    |
|<span data-ttu-id="7aa4e-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="7aa4e-119">Application</span></span> | <span data-ttu-id="7aa4e-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="7aa4e-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aa4e-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7aa4e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7aa4e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7aa4e-122">Request headers</span></span>
| <span data-ttu-id="7aa4e-123">标头</span><span class="sxs-lookup"><span data-stu-id="7aa4e-123">Header</span></span>       | <span data-ttu-id="7aa4e-124">值</span><span class="sxs-lookup"><span data-stu-id="7aa4e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7aa4e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aa4e-125">Authorization</span></span>  | <span data-ttu-id="7aa4e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7aa4e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7aa4e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7aa4e-128">Request body</span></span>
<span data-ttu-id="7aa4e-129">在请求正文中，提供 user 或 group 对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="7aa4e-129">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="7aa4e-130">响应</span><span class="sxs-lookup"><span data-stu-id="7aa4e-130">Response</span></span>
<span data-ttu-id="7aa4e-131">此方法返回 `204 No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="7aa4e-131">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aa4e-132">示例</span><span class="sxs-lookup"><span data-stu-id="7aa4e-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7aa4e-133">请求</span><span class="sxs-lookup"><span data-stu-id="7aa4e-133">Request</span></span>
<span data-ttu-id="7aa4e-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7aa4e-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_acceptedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```

#### <a name="response"></a><span data-ttu-id="7aa4e-135">响应</span><span class="sxs-lookup"><span data-stu-id="7aa4e-135">Response</span></span>
<span data-ttu-id="7aa4e-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7aa4e-136">The following is an example of the response.</span></span>
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
