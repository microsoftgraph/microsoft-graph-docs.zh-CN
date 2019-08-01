---
title: 创建 rejectedSender
description: 将新用户或组添加到 acceptedSender 列表中。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: da2632c388f4eef805b39f135238a40dc2455e59
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014844"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="b136b-103">创建 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="b136b-103">Create rejectedSender</span></span>
<span data-ttu-id="b136b-104">将新用户或组添加到 acceptedSender 列表中。</span><span class="sxs-lookup"><span data-stu-id="b136b-104">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="b136b-p101">在请求主体的 `@odata.id` 中指定用户或组。已拒绝的发件人列表中的用户无法发布到组对话（在 POST 请求 URL 中标识）。确保未在拒绝的发件人和接受的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="b136b-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="b136b-108">权限</span><span class="sxs-lookup"><span data-stu-id="b136b-108">Permissions</span></span>
<span data-ttu-id="b136b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b136b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b136b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b136b-111">Permission type</span></span>      | <span data-ttu-id="b136b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b136b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b136b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b136b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b136b-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b136b-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b136b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b136b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b136b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b136b-116">Not supported.</span></span>    |
|<span data-ttu-id="b136b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b136b-117">Application</span></span> | <span data-ttu-id="b136b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b136b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b136b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b136b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b136b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b136b-120">Request headers</span></span>
| <span data-ttu-id="b136b-121">标头</span><span class="sxs-lookup"><span data-stu-id="b136b-121">Header</span></span>       | <span data-ttu-id="b136b-122">值</span><span class="sxs-lookup"><span data-stu-id="b136b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b136b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b136b-123">Authorization</span></span>  | <span data-ttu-id="b136b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b136b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b136b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b136b-126">Request body</span></span>
<span data-ttu-id="b136b-127">在请求正文中，提供 user 或 group 对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="b136b-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="b136b-128">响应</span><span class="sxs-lookup"><span data-stu-id="b136b-128">Response</span></span>
<span data-ttu-id="b136b-129">此方法返回 `204 No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="b136b-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="b136b-130">示例</span><span class="sxs-lookup"><span data-stu-id="b136b-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b136b-131">请求</span><span class="sxs-lookup"><span data-stu-id="b136b-131">Request</span></span>
<span data-ttu-id="b136b-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b136b-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b136b-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b136b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_rejectedsenders_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b136b-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="b136b-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-rejectedsenders-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b136b-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="b136b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-rejectedsenders-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="b136b-136">C#</span><span class="sxs-lookup"><span data-stu-id="b136b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-rejectedsenders-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b136b-137">Java</span><span class="sxs-lookup"><span data-stu-id="b136b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-rejectedsenders-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b136b-138">响应</span><span class="sxs-lookup"><span data-stu-id="b136b-138">Response</span></span>
<span data-ttu-id="b136b-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b136b-139">The following is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
