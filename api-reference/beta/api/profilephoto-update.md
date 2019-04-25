---
title: 更新 profilephoto
description: 更新租户中任意用户的照片，其中包括已登录用户或指定的组或联系人。 由于存在
localization_priority: Normal
ms.openlocfilehash: f8191716471cba565b27ef316b5b13e3b32ecaff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546477"
---
# <a name="update-profilephoto"></a><span data-ttu-id="4057b-104">更新 profilephoto</span><span class="sxs-lookup"><span data-stu-id="4057b-104">Update profilephoto</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4057b-p102">更新租户中任意用户的照片，其中包括已登录用户或指定的组或联系人。由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的照片小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="4057b-p102">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="4057b-107">在测试版中仅使用 PUT 进行此操作。</span><span class="sxs-lookup"><span data-stu-id="4057b-107">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="4057b-108">**注意：** 1.0 版本中的更新照片操作仅支持用户的工作或学校邮箱，不支持个人邮箱。</span><span class="sxs-lookup"><span data-stu-id="4057b-108">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="4057b-109">权限</span><span class="sxs-lookup"><span data-stu-id="4057b-109">Permissions</span></span>
<span data-ttu-id="4057b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4057b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4057b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4057b-112">Permission type</span></span>      | <span data-ttu-id="4057b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4057b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4057b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4057b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4057b-115">已登录**用户**的个人资料照片:</span><span class="sxs-lookup"><span data-stu-id="4057b-115">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="4057b-116">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="4057b-116">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4057b-117">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="4057b-117">For **group** resource:</span></span><br /><span data-ttu-id="4057b-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4057b-118">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4057b-119">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="4057b-119">For **contact** resource:</span></span><br /><span data-ttu-id="4057b-120">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4057b-120">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="4057b-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4057b-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4057b-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="4057b-122">Not supported.</span></span> |
|<span data-ttu-id="4057b-123">Application</span><span class="sxs-lookup"><span data-stu-id="4057b-123">Application</span></span>                            | <span data-ttu-id="4057b-124">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="4057b-124">For **user** resource:</span></span><br/><span data-ttu-id="4057b-125">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4057b-125">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4057b-126">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="4057b-126">For **group** resource:</span></span><br /><span data-ttu-id="4057b-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4057b-127">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4057b-128">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="4057b-128">For **contact** resource:</span></span><br /><span data-ttu-id="4057b-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4057b-129">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="4057b-130">**注释**若要更新组织中任何用户的照片, 应用必须具有用户的 ReadWrite。所有应用程序权限, 并在其自己的标识下调用此 API, 而不代表用户。</span><span class="sxs-lookup"><span data-stu-id="4057b-130">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="4057b-131">若要了解详细信息, 请参阅[获取 access 而无需登录用户](/graph/auth-v2-service)。</span><span class="sxs-lookup"><span data-stu-id="4057b-131">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="4057b-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4057b-132">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="4057b-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="4057b-133">Request headers</span></span>
| <span data-ttu-id="4057b-134">标头</span><span class="sxs-lookup"><span data-stu-id="4057b-134">Header</span></span>       | <span data-ttu-id="4057b-135">值</span><span class="sxs-lookup"><span data-stu-id="4057b-135">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4057b-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="4057b-136">Authorization</span></span>  | <span data-ttu-id="4057b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4057b-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4057b-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4057b-139">Content-Type</span></span>  | <span data-ttu-id="4057b-p106">image/jpeg。必需。</span><span class="sxs-lookup"><span data-stu-id="4057b-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4057b-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="4057b-142">Request body</span></span>
<span data-ttu-id="4057b-143">在请求正文中，包括请求正文中照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="4057b-143">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="4057b-144">响应</span><span class="sxs-lookup"><span data-stu-id="4057b-144">Response</span></span>

<span data-ttu-id="4057b-145">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4057b-145">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="4057b-146">示例</span><span class="sxs-lookup"><span data-stu-id="4057b-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4057b-147">请求</span><span class="sxs-lookup"><span data-stu-id="4057b-147">Request</span></span>
<span data-ttu-id="4057b-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4057b-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="4057b-149">响应</span><span class="sxs-lookup"><span data-stu-id="4057b-149">Response</span></span>
<span data-ttu-id="4057b-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4057b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/profilephoto-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
