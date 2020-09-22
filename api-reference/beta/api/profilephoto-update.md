---
title: 更新 profilephoto
description: 更新租户中任意用户的照片，其中包括已登录用户或指定的组或联系人。 自此处起
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: 675b1cb4116ec59b65442c683fe07f67a8045379
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087997"
---
# <a name="update-profilephoto"></a><span data-ttu-id="070d9-104">更新 profilephoto</span><span class="sxs-lookup"><span data-stu-id="070d9-104">Update profilephoto</span></span>

<span data-ttu-id="070d9-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="070d9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="070d9-p102">更新租户中任何用户的照片，包括已登录用户或指定的组或联系人。由于目前每个 REST 请求的总大小限制为8MB，因此您可以添加的照片的大小限制为 8 MB 以下。</span><span class="sxs-lookup"><span data-stu-id="070d9-p102">Update the photo for any user in the tenant, including the signed-in user or the specified group or contact. Because there is currently a limit of 8MB on the total size of each REST request, the size of the photo you can add is limited to under 8MB.</span></span>

<span data-ttu-id="070d9-108">仅在此操作中使用 PUT。</span><span class="sxs-lookup"><span data-stu-id="070d9-108">Only use PUT for this operation.</span></span>

> <span data-ttu-id="070d9-109">**注意**：更新 **用户** 照片时，此操作将先尝试更新 Microsoft 365 中的照片。</span><span class="sxs-lookup"><span data-stu-id="070d9-109">**Note**:  When updating the **user** photo, this operation first attempts to update the photo in Microsoft 365.</span></span> <span data-ttu-id="070d9-110">如果此操作失败 (由于用户没有邮箱) ，此 API 将尝试更新 Azure Active Directory 中的照片。</span><span class="sxs-lookup"><span data-stu-id="070d9-110">If that fails (due to the user not having a mailbox), this API will attempt to update the photo in Azure Active Directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="070d9-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="070d9-111">Permissions</span></span>
<span data-ttu-id="070d9-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="070d9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="070d9-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="070d9-114">Permission type</span></span>      | <span data-ttu-id="070d9-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="070d9-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="070d9-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="070d9-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="070d9-117">已登录 **用户**的个人资料照片：</span><span class="sxs-lookup"><span data-stu-id="070d9-117">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="070d9-118">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="070d9-118">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="070d9-119">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="070d9-119">For **group** resource:</span></span><br /><span data-ttu-id="070d9-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="070d9-120">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="070d9-121">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="070d9-121">For **contact** resource:</span></span><br /><span data-ttu-id="070d9-122">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="070d9-122">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="070d9-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="070d9-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="070d9-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="070d9-124">Not supported.</span></span> |
|<span data-ttu-id="070d9-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="070d9-125">Application</span></span>                            | <span data-ttu-id="070d9-126">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="070d9-126">For **user** resource:</span></span><br/><span data-ttu-id="070d9-127">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="070d9-127">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="070d9-128">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="070d9-128">For **group** resource:</span></span><br /><span data-ttu-id="070d9-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="070d9-129">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="070d9-130">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="070d9-130">For **contact** resource:</span></span><br /><span data-ttu-id="070d9-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="070d9-131">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="070d9-132">**注意** 若要更新组织中任何用户的照片，应用必须具有 User.ReadWrite.All 应用程序权限，并以其自己的身份而不是代表用户来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="070d9-132">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="070d9-133">若要了解详细信息，请参阅[在没有已登录用户的情况下进行访问](/graph/auth-v2-service)。</span><span class="sxs-lookup"><span data-stu-id="070d9-133">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span> <span data-ttu-id="070d9-134">更新已登录用户的照片只需要用户的 ReadWrite 权限。</span><span class="sxs-lookup"><span data-stu-id="070d9-134">Updating the photo of the signed-in user only requires User.ReadWrite permission.</span></span>

> <span data-ttu-id="070d9-135">**注意：** 当前有一个[已知问题](/graph/known-issues#groups)，即使用应用程序权限访问组照片。</span><span class="sxs-lookup"><span data-stu-id="070d9-135">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="070d9-136">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="070d9-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```

<span data-ttu-id="070d9-137">若要更新团队的照片：</span><span class="sxs-lookup"><span data-stu-id="070d9-137">To update the photo for a team:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PUT /groups/{teamId}/photo/$value`
```

## <a name="request-headers"></a><span data-ttu-id="070d9-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="070d9-138">Request headers</span></span>
| <span data-ttu-id="070d9-139">标头</span><span class="sxs-lookup"><span data-stu-id="070d9-139">Header</span></span>       | <span data-ttu-id="070d9-140">值</span><span class="sxs-lookup"><span data-stu-id="070d9-140">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="070d9-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="070d9-141">Authorization</span></span>  | <span data-ttu-id="070d9-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="070d9-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="070d9-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="070d9-144">Content-Type</span></span>  | <span data-ttu-id="070d9-p107">image/jpeg。必需。</span><span class="sxs-lookup"><span data-stu-id="070d9-p107">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="070d9-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="070d9-147">Request body</span></span>
<span data-ttu-id="070d9-148">在请求正文中，包括请求正文中照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="070d9-148">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="070d9-149">响应</span><span class="sxs-lookup"><span data-stu-id="070d9-149">Response</span></span>

<span data-ttu-id="070d9-150">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="070d9-150">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="070d9-151">示例</span><span class="sxs-lookup"><span data-stu-id="070d9-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="070d9-152">请求</span><span class="sxs-lookup"><span data-stu-id="070d9-152">Request</span></span>
<span data-ttu-id="070d9-153">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="070d9-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="070d9-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="070d9-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="c"></a>[<span data-ttu-id="070d9-155">C#</span><span class="sxs-lookup"><span data-stu-id="070d9-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="070d9-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="070d9-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="070d9-157">响应</span><span class="sxs-lookup"><span data-stu-id="070d9-157">Response</span></span>
<span data-ttu-id="070d9-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="070d9-158">The following is an example of the response.</span></span> 

><span data-ttu-id="070d9-159">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="070d9-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


