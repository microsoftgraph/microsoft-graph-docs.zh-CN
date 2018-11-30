---
title: 更新 profilephoto
description: 更新已登录的**用户**，或指定的**组**或**联系人**的照片。 相那里
ms.openlocfilehash: cf20ae6f59f0d912b8bd08a9be42591bb6f97127
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008071"
---
# <a name="update-profilephoto"></a><span data-ttu-id="c777c-104">更新 profilephoto</span><span class="sxs-lookup"><span data-stu-id="c777c-104">Update profilephoto</span></span>

<span data-ttu-id="c777c-p102">更新登录 **用户**、指定**组**或**联系人**的照片。由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的照片小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="c777c-p102">Update the photo for the signed-in **user**, or the specified **group** or **contact**. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="c777c-107">可以在版本 1.0 中使用 PATCH 或 PUT 执行此操作。</span><span class="sxs-lookup"><span data-stu-id="c777c-107">You can use either PATCH or PUT for this operation in version 1.0.</span></span>

> <span data-ttu-id="c777c-108">**注意**：1.0 版本中的操作仅支持用户的工作或学校邮箱，不支持个人邮箱。</span><span class="sxs-lookup"><span data-stu-id="c777c-108">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="c777c-109">权限</span><span class="sxs-lookup"><span data-stu-id="c777c-109">Permissions</span></span>
<span data-ttu-id="c777c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c777c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

- <span data-ttu-id="c777c-112">已登录**用户**的个人资料照片 - User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c777c-112">Profile photo of the signed-in **user** - User.ReadWrite, User.ReadWrite.All</span></span>
- <span data-ttu-id="c777c-113">**组**的个人资料照片 - Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c777c-113">Profile photo of a **group** - Group.ReadWrite.All</span></span>
- <span data-ttu-id="c777c-114">**联系人**的照片 - Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c777c-114">Photo of a **contact** - Contacts.ReadWrite</span></span>

> <span data-ttu-id="c777c-p104">**注意** 要更新组织中任何用户的照片，应用必须具有 User.ReadWrite.All 应用程序权限，并以其自己的身份而不是代表用户来调用此 API。若要了解详细信息，请参阅[无需已登录用户即可访问](/graph/auth-v2-service)。</span><span class="sxs-lookup"><span data-stu-id="c777c-p104">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="c777c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c777c-117">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="c777c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c777c-118">Request headers</span></span>
| <span data-ttu-id="c777c-119">标头</span><span class="sxs-lookup"><span data-stu-id="c777c-119">Header</span></span>       | <span data-ttu-id="c777c-120">值</span><span class="sxs-lookup"><span data-stu-id="c777c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c777c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c777c-121">Authorization</span></span>  | <span data-ttu-id="c777c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c777c-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c777c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c777c-124">Content-Type</span></span>  | <span data-ttu-id="c777c-p106">image/jpeg。必需。</span><span class="sxs-lookup"><span data-stu-id="c777c-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c777c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c777c-127">Request body</span></span>
<span data-ttu-id="c777c-128">在请求正文中，包括请求正文中照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="c777c-128">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="c777c-129">响应</span><span class="sxs-lookup"><span data-stu-id="c777c-129">Response</span></span>

<span data-ttu-id="c777c-130">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c777c-130">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="c777c-131">示例</span><span class="sxs-lookup"><span data-stu-id="c777c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c777c-132">请求</span><span class="sxs-lookup"><span data-stu-id="c777c-132">Request</span></span>
<span data-ttu-id="c777c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c777c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="c777c-134">响应</span><span class="sxs-lookup"><span data-stu-id="c777c-134">Response</span></span>
<span data-ttu-id="c777c-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c777c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
