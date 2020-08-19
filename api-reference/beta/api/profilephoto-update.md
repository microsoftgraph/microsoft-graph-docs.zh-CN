---
title: 更新 profilephoto
description: 更新租户中任意用户的照片，其中包括已登录用户或指定的组或联系人。 自此处起
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: 72c30f03b51e186321acf6b89790c0fbd1352f06
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807981"
---
# <a name="update-profilephoto"></a><span data-ttu-id="85c29-104">更新 profilephoto</span><span class="sxs-lookup"><span data-stu-id="85c29-104">Update profilephoto</span></span>

<span data-ttu-id="85c29-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85c29-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85c29-p102">更新租户中任何用户的照片，包括登录用户或指定的组或联系人。由于目前每个 REST 请求的总大小限制为8MB，这会限制您可以添加到8MB 下的照片的大小。</span><span class="sxs-lookup"><span data-stu-id="85c29-p102">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact. Since there is currently a limit of 8MB on the total size of each REST request, this limits the size of the photo you can add to under 8MB.</span></span>

<span data-ttu-id="85c29-108">在测试版中仅使用 PUT 进行此操作。</span><span class="sxs-lookup"><span data-stu-id="85c29-108">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="85c29-109">**注意**：更新 **用户** 照片时，此操作将先尝试更新 Microsoft 365 中的照片。</span><span class="sxs-lookup"><span data-stu-id="85c29-109">**Note**:  When updating the **user** photo, this operation first attempts to update the photo in Microsoft 365.</span></span> <span data-ttu-id="85c29-110">如果此操作失败 (由于用户没有邮箱) ，此 API 将尝试更新 Azure Active Directory 中的照片。</span><span class="sxs-lookup"><span data-stu-id="85c29-110">If that fails (due to the user not having a mailbox), this API will attempt to update the photo in Azure Active Directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="85c29-111">权限</span><span class="sxs-lookup"><span data-stu-id="85c29-111">Permissions</span></span>
<span data-ttu-id="85c29-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85c29-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85c29-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="85c29-114">Permission type</span></span>      | <span data-ttu-id="85c29-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="85c29-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85c29-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85c29-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="85c29-117">已登录 **用户**的个人资料照片：</span><span class="sxs-lookup"><span data-stu-id="85c29-117">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="85c29-118">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="85c29-118">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="85c29-119">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="85c29-119">For **group** resource:</span></span><br /><span data-ttu-id="85c29-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85c29-120">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="85c29-121">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="85c29-121">For **contact** resource:</span></span><br /><span data-ttu-id="85c29-122">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85c29-122">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="85c29-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85c29-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85c29-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="85c29-124">Not supported.</span></span> |
|<span data-ttu-id="85c29-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="85c29-125">Application</span></span>                            | <span data-ttu-id="85c29-126">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="85c29-126">For **user** resource:</span></span><br/><span data-ttu-id="85c29-127">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85c29-127">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="85c29-128">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="85c29-128">For **group** resource:</span></span><br /><span data-ttu-id="85c29-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85c29-129">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="85c29-130">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="85c29-130">For **contact** resource:</span></span><br /><span data-ttu-id="85c29-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85c29-131">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="85c29-132">**注意** 若要更新组织中任何用户的照片，应用必须具有 User.ReadWrite.All 应用程序权限，并以其自己的身份而不是代表用户来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="85c29-132">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="85c29-133">若要了解详细信息，请参阅[在没有已登录用户的情况下进行访问](/graph/auth-v2-service)。</span><span class="sxs-lookup"><span data-stu-id="85c29-133">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span> <span data-ttu-id="85c29-134">更新已登录用户的照片只需要用户的 ReadWrite 权限。</span><span class="sxs-lookup"><span data-stu-id="85c29-134">Updating the photo of the signed-in user only requires User.ReadWrite permission.</span></span>

> <span data-ttu-id="85c29-135">**注意：** 当前有一个[已知问题](/graph/known-issues#groups)，即使用应用程序权限访问组照片。</span><span class="sxs-lookup"><span data-stu-id="85c29-135">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="85c29-136">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85c29-136">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="85c29-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="85c29-137">Request headers</span></span>
| <span data-ttu-id="85c29-138">标头</span><span class="sxs-lookup"><span data-stu-id="85c29-138">Header</span></span>       | <span data-ttu-id="85c29-139">值</span><span class="sxs-lookup"><span data-stu-id="85c29-139">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="85c29-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="85c29-140">Authorization</span></span>  | <span data-ttu-id="85c29-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="85c29-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="85c29-143">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85c29-143">Content-Type</span></span>  | <span data-ttu-id="85c29-p107">image/jpeg。必需。</span><span class="sxs-lookup"><span data-stu-id="85c29-p107">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="85c29-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="85c29-146">Request body</span></span>
<span data-ttu-id="85c29-147">在请求正文中，包括请求正文中照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="85c29-147">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="85c29-148">响应</span><span class="sxs-lookup"><span data-stu-id="85c29-148">Response</span></span>

<span data-ttu-id="85c29-149">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="85c29-149">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="85c29-150">示例</span><span class="sxs-lookup"><span data-stu-id="85c29-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85c29-151">请求</span><span class="sxs-lookup"><span data-stu-id="85c29-151">Request</span></span>
<span data-ttu-id="85c29-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="85c29-152">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85c29-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="85c29-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="c"></a>[<span data-ttu-id="85c29-154">C#</span><span class="sxs-lookup"><span data-stu-id="85c29-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85c29-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85c29-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="85c29-156">响应</span><span class="sxs-lookup"><span data-stu-id="85c29-156">Response</span></span>
<span data-ttu-id="85c29-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="85c29-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
