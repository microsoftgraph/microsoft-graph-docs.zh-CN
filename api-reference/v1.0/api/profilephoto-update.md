---
title: 更新 profilephoto
description: 更新已登录 **用户**、指定 **组** 或 **联系人** 的照片。 自此处起
localization_priority: Priority
author: kevinbellinger
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 8797b12d070b582a551486ac25678c4f1794adf5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048664"
---
# <a name="update-profilephoto"></a><span data-ttu-id="c0331-104">更新 profilephoto</span><span class="sxs-lookup"><span data-stu-id="c0331-104">Update profilephoto</span></span>

<span data-ttu-id="c0331-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0331-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0331-p102">更新登录 **用户**、指定 **组** 或 **联系人** 的照片。由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的照片小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="c0331-p102">Update the photo for the signed-in **user**, or the specified **group** or **contact**. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="c0331-108">可以在版本 1.0 中使用 PATCH 或 PUT 执行此操作。</span><span class="sxs-lookup"><span data-stu-id="c0331-108">You can use either PATCH or PUT for this operation in version 1.0.</span></span>

> <span data-ttu-id="c0331-109">**注意**：1.0 版本中的操作仅支持用户的工作或学校邮箱，不支持个人邮箱。</span><span class="sxs-lookup"><span data-stu-id="c0331-109">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0331-110">权限</span><span class="sxs-lookup"><span data-stu-id="c0331-110">Permissions</span></span>
<span data-ttu-id="c0331-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0331-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

- <span data-ttu-id="c0331-113">已登录 **用户** 的个人资料照片 - User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0331-113">Profile photo of the signed-in **user** - User.ReadWrite, User.ReadWrite.All</span></span>
- <span data-ttu-id="c0331-114">**组** 的个人资料照片 - Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0331-114">Profile photo of a **group** - Group.ReadWrite.All</span></span>
- <span data-ttu-id="c0331-115">**联系人** 的照片 - Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0331-115">Photo of a **contact** - Contacts.ReadWrite</span></span>

> <span data-ttu-id="c0331-116">**注意** 若要更新组织中任何用户的照片，应用必须具有 User.ReadWrite.All 应用程序权限，并以其自己的身份而不是代表用户来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="c0331-116">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="c0331-117">若要了解详细信息，请参阅[在没有已登录用户的情况下进行访问](/graph/auth-v2-service)。</span><span class="sxs-lookup"><span data-stu-id="c0331-117">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

> <span data-ttu-id="c0331-118">**注意：** 当前有一个 [已知问题](/graph/known-issues#groups)，即使用应用程序权限访问组照片。</span><span class="sxs-lookup"><span data-stu-id="c0331-118">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="c0331-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0331-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/photo/$value
PATCH /users/{id | userPrincipalName}/photo/$value
PATCH /groups/{id}/photo/$value
PATCH /me/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PATCH /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value

PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a><span data-ttu-id="c0331-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0331-120">Request headers</span></span>
| <span data-ttu-id="c0331-121">标头</span><span class="sxs-lookup"><span data-stu-id="c0331-121">Header</span></span>       | <span data-ttu-id="c0331-122">值</span><span class="sxs-lookup"><span data-stu-id="c0331-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c0331-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0331-123">Authorization</span></span>  | <span data-ttu-id="c0331-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0331-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c0331-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0331-126">Content-Type</span></span>  | <span data-ttu-id="c0331-p106">image/jpeg。必需。</span><span class="sxs-lookup"><span data-stu-id="c0331-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0331-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0331-129">Request body</span></span>
<span data-ttu-id="c0331-130">在请求正文中，包括请求正文中照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="c0331-130">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="c0331-131">响应</span><span class="sxs-lookup"><span data-stu-id="c0331-131">Response</span></span>

<span data-ttu-id="c0331-132">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c0331-132">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="c0331-133">示例</span><span class="sxs-lookup"><span data-stu-id="c0331-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0331-134">请求</span><span class="sxs-lookup"><span data-stu-id="c0331-134">Request</span></span>
<span data-ttu-id="c0331-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0331-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0331-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0331-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="c"></a>[<span data-ttu-id="c0331-137">C#</span><span class="sxs-lookup"><span data-stu-id="c0331-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0331-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0331-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0331-139">Java</span><span class="sxs-lookup"><span data-stu-id="c0331-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-profilephoto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0331-140">响应</span><span class="sxs-lookup"><span data-stu-id="c0331-140">Response</span></span>
<span data-ttu-id="c0331-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c0331-141">Here is an example of the response.</span></span> <span data-ttu-id="c0331-142">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c0331-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

