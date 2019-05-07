---
title: 创建 rejectedSender
description: 将新用户或组添加到 acceptedSender 列表中。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 640a1728f498a26770827d02d10e60cf9a8bc6cb
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613727"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="70e3d-103">创建 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="70e3d-103">Create rejectedSender</span></span>
<span data-ttu-id="70e3d-104">将新用户或组添加到 acceptedSender 列表中。</span><span class="sxs-lookup"><span data-stu-id="70e3d-104">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="70e3d-p101">在请求主体的 `@odata.id` 中指定用户或组。已拒绝的发件人列表中的用户无法发布到组对话（在 POST 请求 URL 中标识）。确保未在拒绝的发件人和接受的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="70e3d-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="70e3d-108">权限</span><span class="sxs-lookup"><span data-stu-id="70e3d-108">Permissions</span></span>
<span data-ttu-id="70e3d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70e3d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70e3d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="70e3d-111">Permission type</span></span>      | <span data-ttu-id="70e3d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70e3d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70e3d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70e3d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="70e3d-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70e3d-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="70e3d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70e3d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70e3d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="70e3d-116">Not supported.</span></span>    |
|<span data-ttu-id="70e3d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="70e3d-117">Application</span></span> | <span data-ttu-id="70e3d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="70e3d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="70e3d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70e3d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="70e3d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="70e3d-120">Request headers</span></span>
| <span data-ttu-id="70e3d-121">标头</span><span class="sxs-lookup"><span data-stu-id="70e3d-121">Header</span></span>       | <span data-ttu-id="70e3d-122">值</span><span class="sxs-lookup"><span data-stu-id="70e3d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="70e3d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70e3d-123">Authorization</span></span>  | <span data-ttu-id="70e3d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="70e3d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70e3d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="70e3d-126">Request body</span></span>
<span data-ttu-id="70e3d-127">在请求正文中，提供 user 或 group 对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="70e3d-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="70e3d-128">响应</span><span class="sxs-lookup"><span data-stu-id="70e3d-128">Response</span></span>
<span data-ttu-id="70e3d-129">此方法返回 `204 No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="70e3d-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="70e3d-130">示例</span><span class="sxs-lookup"><span data-stu-id="70e3d-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="70e3d-131">请求</span><span class="sxs-lookup"><span data-stu-id="70e3d-131">Request</span></span>
<span data-ttu-id="70e3d-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="70e3d-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
#### <a name="response"></a><span data-ttu-id="70e3d-133">响应</span><span class="sxs-lookup"><span data-stu-id="70e3d-133">Response</span></span>
<span data-ttu-id="70e3d-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="70e3d-134">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="70e3d-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="70e3d-135">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70e3d-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="70e3d-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-post-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
