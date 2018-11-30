---
title: 更新 profilephoto
description: 更新的签名项包括租户中的任何用户的照片用户或指定的组或联系人。 相那里
ms.openlocfilehash: 801ccd58e57cb02c1805f927dc22c9fd593cbae5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046198"
---
# <a name="update-profilephoto"></a><span data-ttu-id="c6f74-104">更新 profilephoto</span><span class="sxs-lookup"><span data-stu-id="c6f74-104">Update profilephoto</span></span>

> <span data-ttu-id="c6f74-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c6f74-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6f74-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c6f74-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c6f74-p103">更新租户中任意用户的照片，其中包括已登录用户或指定的组或联系人。由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的照片小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="c6f74-p103">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="c6f74-109">在测试版中仅使用 PUT 进行此操作。</span><span class="sxs-lookup"><span data-stu-id="c6f74-109">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="c6f74-110">**注意：** 1.0 版本中的更新照片操作仅支持用户的工作或学校邮箱，不支持个人邮箱。</span><span class="sxs-lookup"><span data-stu-id="c6f74-110">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6f74-111">权限</span><span class="sxs-lookup"><span data-stu-id="c6f74-111">Permissions</span></span>
<span data-ttu-id="c6f74-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6f74-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6f74-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6f74-114">Permission type</span></span>      | <span data-ttu-id="c6f74-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c6f74-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6f74-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6f74-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6f74-117">登录**用户**的配置文件照片：</span><span class="sxs-lookup"><span data-stu-id="c6f74-117">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="c6f74-118">User.ReadWrite User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6f74-118">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="c6f74-119">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="c6f74-119">For **group** resource:</span></span><br /><span data-ttu-id="c6f74-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6f74-120">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="c6f74-121">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="c6f74-121">For **contact** resource:</span></span><br /><span data-ttu-id="c6f74-122">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6f74-122">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="c6f74-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6f74-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6f74-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6f74-124">Not supported.</span></span> |
|<span data-ttu-id="c6f74-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6f74-125">Application</span></span>                            | <span data-ttu-id="c6f74-126">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="c6f74-126">For **user** resource:</span></span><br/><span data-ttu-id="c6f74-127">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6f74-127">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="c6f74-128">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="c6f74-128">For **group** resource:</span></span><br /><span data-ttu-id="c6f74-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6f74-129">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="c6f74-130">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="c6f74-130">For **contact** resource:</span></span><br /><span data-ttu-id="c6f74-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6f74-131">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="c6f74-p105">**注意** 要更新组织中任何用户的照片，应用必须具有 User.ReadWrite.All 应用程序权限，并以其自己的身份而不是代表用户来调用此 API。若要了解详细信息，请参阅[无需已登录用户即可访问](/graph/auth-v2-service)。</span><span class="sxs-lookup"><span data-stu-id="c6f74-p105">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="c6f74-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6f74-134">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="c6f74-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6f74-135">Request headers</span></span>
| <span data-ttu-id="c6f74-136">标头</span><span class="sxs-lookup"><span data-stu-id="c6f74-136">Header</span></span>       | <span data-ttu-id="c6f74-137">值</span><span class="sxs-lookup"><span data-stu-id="c6f74-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c6f74-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6f74-138">Authorization</span></span>  | <span data-ttu-id="c6f74-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c6f74-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c6f74-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6f74-141">Content-Type</span></span>  | <span data-ttu-id="c6f74-p107">image/jpeg。必需。</span><span class="sxs-lookup"><span data-stu-id="c6f74-p107">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c6f74-144">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6f74-144">Request body</span></span>
<span data-ttu-id="c6f74-145">在请求正文中，包括请求正文中照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="c6f74-145">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="c6f74-146">响应</span><span class="sxs-lookup"><span data-stu-id="c6f74-146">Response</span></span>

<span data-ttu-id="c6f74-147">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c6f74-147">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="c6f74-148">示例</span><span class="sxs-lookup"><span data-stu-id="c6f74-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6f74-149">请求</span><span class="sxs-lookup"><span data-stu-id="c6f74-149">Request</span></span>
<span data-ttu-id="c6f74-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6f74-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="c6f74-151">响应</span><span class="sxs-lookup"><span data-stu-id="c6f74-151">Response</span></span>
<span data-ttu-id="c6f74-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6f74-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
