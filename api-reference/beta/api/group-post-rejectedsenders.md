---
title: 创建 rejectedSender
description: 将新用户或组添加到 acceptedSender 列表中。
author: dkershaw10
ms.openlocfilehash: 08156823a8a7e7ad6075afee49ff979c3955e70a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350076"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="42415-103">创建 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="42415-103">Create rejectedSender</span></span>

> <span data-ttu-id="42415-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="42415-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42415-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="42415-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42415-106">将新用户或组添加到 acceptedSender 列表中。</span><span class="sxs-lookup"><span data-stu-id="42415-106">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="42415-p102">在请求主体的 `@odata.id` 中指定用户或组。已拒绝的发件人列表中的用户无法发布到组对话（在 POST 请求 URL 中标识）。确保未在拒绝的发件人和接受的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="42415-p102">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="42415-110">权限</span><span class="sxs-lookup"><span data-stu-id="42415-110">Permissions</span></span>
<span data-ttu-id="42415-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42415-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42415-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="42415-113">Permission type</span></span>      | <span data-ttu-id="42415-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42415-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42415-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42415-115">Delegated (work or school account)</span></span> | <span data-ttu-id="42415-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42415-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="42415-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42415-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42415-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="42415-118">Not supported.</span></span>    |
|<span data-ttu-id="42415-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="42415-119">Application</span></span> | <span data-ttu-id="42415-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="42415-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42415-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42415-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="42415-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="42415-122">Request headers</span></span>
| <span data-ttu-id="42415-123">标头</span><span class="sxs-lookup"><span data-stu-id="42415-123">Header</span></span>       | <span data-ttu-id="42415-124">值</span><span class="sxs-lookup"><span data-stu-id="42415-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="42415-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="42415-125">Authorization</span></span>  | <span data-ttu-id="42415-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="42415-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="42415-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="42415-128">Request body</span></span>
<span data-ttu-id="42415-129">在请求正文中，提供 user 或 group 对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="42415-129">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="42415-130">响应</span><span class="sxs-lookup"><span data-stu-id="42415-130">Response</span></span>
<span data-ttu-id="42415-131">此方法返回 `204 No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="42415-131">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="42415-132">示例</span><span class="sxs-lookup"><span data-stu-id="42415-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="42415-133">请求</span><span class="sxs-lookup"><span data-stu-id="42415-133">Request</span></span>
<span data-ttu-id="42415-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="42415-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rejectedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```

#### <a name="response"></a><span data-ttu-id="42415-135">响应</span><span class="sxs-lookup"><span data-stu-id="42415-135">Response</span></span>
<span data-ttu-id="42415-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="42415-136">The following is an example of the response.</span></span>
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
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
