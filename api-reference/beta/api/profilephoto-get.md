---
title: 获取照片
description: 获取指定的 profilePhoto 或其元数据（**profilePhoto** 属性）。
localization_priority: Priority
ms.openlocfilehash: 422b9cb39b7af6527341070cbe35f3bfb59d504d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337165"
---
# <a name="get-photo"></a><span data-ttu-id="2cb02-103">获取照片</span><span class="sxs-lookup"><span data-stu-id="2cb02-103">Get photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cb02-104">获取指定的 [profilePhoto](../resources/profilephoto.md) 或其元数据（**profilePhoto** 属性）。</span><span class="sxs-lookup"><span data-stu-id="2cb02-104">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (**profilePhoto** properties).</span></span>

<span data-ttu-id="2cb02-105">获取照片方法首先尝试从 Office 365 检索指定的照片。</span><span class="sxs-lookup"><span data-stu-id="2cb02-105">A GET photo method first attempts to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="2cb02-106">如果 Office 365 中没有此照片，则 API 尝试从 Azure Active Directory 检索该照片。</span><span class="sxs-lookup"><span data-stu-id="2cb02-106">If the photo is not available in Office 365, the API attempts to retrieve the photo from Azure Active Directory.</span></span>

<span data-ttu-id="2cb02-107">Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。</span><span class="sxs-lookup"><span data-stu-id="2cb02-107">The supported sizes of HD photos in Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="2cb02-108">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="2cb02-108">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="2cb02-109">可以获取最大照片的元数据，也可以指定尺寸来获取相应照片尺寸的元数据。</span><span class="sxs-lookup"><span data-stu-id="2cb02-109">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="2cb02-110">如果请求的大小不可用，则仍然可以获取用户已上载且可供使用的较小大小。</span><span class="sxs-lookup"><span data-stu-id="2cb02-110">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="2cb02-111">例如，如果用户上传像素为 504x504 的照片，除 648x648 外所有尺寸的照片都可供下载。</span><span class="sxs-lookup"><span data-stu-id="2cb02-111">For example, if the user uploads a photo that is 504x504 pixels, all but the 648x648 size of the photo will be available for download.</span></span>
<span data-ttu-id="2cb02-112">如果在用户邮箱或 Azure Active Directory 中找不到指定尺寸，则返回的是尺寸 1x1 和剩余元数据。</span><span class="sxs-lookup"><span data-stu-id="2cb02-112">If the specified size is not available in the user's mailbox or in Azure Active Directory, the size 1x1 is returned with the rest of the  metadata.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cb02-113">权限</span><span class="sxs-lookup"><span data-stu-id="2cb02-113">Permissions</span></span>
<span data-ttu-id="2cb02-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2cb02-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="2cb02-116">**注意：** beta 版中的获取照片方法支持用户的工作、学校或个人帐户。</span><span class="sxs-lookup"><span data-stu-id="2cb02-116">**Note:** The GET photo method in beta supports a user's work, school, or personal accounts.</span></span> <span data-ttu-id="2cb02-117">但是获取照片元数据方法仅支持用户的工作或学校帐户，不支持个人帐户。</span><span class="sxs-lookup"><span data-stu-id="2cb02-117">The GET photo metadata method, however, supports only the user's work or school accounts and not personal accounts.</span></span>

|<span data-ttu-id="2cb02-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="2cb02-118">Permission type</span></span>      | <span data-ttu-id="2cb02-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2cb02-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cb02-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2cb02-120">Delegated (work or school account)</span></span> | <span data-ttu-id="2cb02-121">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="2cb02-121">For **user** resource:</span></span><br/><span data-ttu-id="2cb02-122">User.Read、User.ReadBasic.All、User.Read.All、User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cb02-122">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="2cb02-123">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="2cb02-123">For **group** resource:</span></span><br /><span data-ttu-id="2cb02-124">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cb02-124">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="2cb02-125">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="2cb02-125">For **contact** resource:</span></span><br /><span data-ttu-id="2cb02-126">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2cb02-126">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="2cb02-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2cb02-127">Delegated (personal Microsoft account)</span></span>  <br /> <span data-ttu-id="2cb02-128">**注意**：不支持元数据操作。</span><span class="sxs-lookup"><span data-stu-id="2cb02-128">**Note**: Metadata operation is not supported.</span></span> | <span data-ttu-id="2cb02-129">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="2cb02-129">For **user** resource:</span></span><br/><span data-ttu-id="2cb02-130">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2cb02-130">User.Read, User.ReadWrite</span></span><br /><br /><span data-ttu-id="2cb02-131">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="2cb02-131">For **contact** resource:</span></span><br /><span data-ttu-id="2cb02-132">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2cb02-132">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="2cb02-133">Application</span><span class="sxs-lookup"><span data-stu-id="2cb02-133">Application</span></span>                        | <span data-ttu-id="2cb02-134">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="2cb02-134">For **user** resource:</span></span><br/><span data-ttu-id="2cb02-135">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cb02-135">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="2cb02-136">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="2cb02-136">For **group** resource:</span></span><br /><span data-ttu-id="2cb02-137">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cb02-137">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="2cb02-138">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="2cb02-138">For **contact** resource:</span></span><br /><span data-ttu-id="2cb02-139">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2cb02-139">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2cb02-140">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2cb02-140">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="2cb02-141">获取照片</span><span class="sxs-lookup"><span data-stu-id="2cb02-141">Get the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo/$value
GET /users/{id | userPrincipalName}/photo/$value
GET /groups/{id}/photo/$value
GET /me/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contacts/{id}/photo/$value
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="2cb02-142">获取照片的元数据</span><span class="sxs-lookup"><span data-stu-id="2cb02-142">Get the metadata of the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="2cb02-143">获取指定照片尺寸的元数据</span><span class="sxs-lookup"><span data-stu-id="2cb02-143">Get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="2cb02-144">路径参数</span><span class="sxs-lookup"><span data-stu-id="2cb02-144">Path parameters</span></span>

|<span data-ttu-id="2cb02-145">**参数**</span><span class="sxs-lookup"><span data-stu-id="2cb02-145">**Parameter**</span></span>|<span data-ttu-id="2cb02-146">**类型**</span><span class="sxs-lookup"><span data-stu-id="2cb02-146">**Type**</span></span>|<span data-ttu-id="2cb02-147">**说明**</span><span class="sxs-lookup"><span data-stu-id="2cb02-147">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2cb02-148">size</span><span class="sxs-lookup"><span data-stu-id="2cb02-148">size</span></span>  |<span data-ttu-id="2cb02-149">String</span><span class="sxs-lookup"><span data-stu-id="2cb02-149">String</span></span>  | <span data-ttu-id="2cb02-150">照片尺寸。</span><span class="sxs-lookup"><span data-stu-id="2cb02-150">A photo size.</span></span> <span data-ttu-id="2cb02-151">Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。</span><span class="sxs-lookup"><span data-stu-id="2cb02-151">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="2cb02-152">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="2cb02-152">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="2cb02-153">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2cb02-153">Optional query parameters</span></span>
<span data-ttu-id="2cb02-154">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2cb02-154">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2cb02-155">请求标头</span><span class="sxs-lookup"><span data-stu-id="2cb02-155">Request headers</span></span>
| <span data-ttu-id="2cb02-156">名称</span><span class="sxs-lookup"><span data-stu-id="2cb02-156">Name</span></span>       | <span data-ttu-id="2cb02-157">类型</span><span class="sxs-lookup"><span data-stu-id="2cb02-157">Type</span></span> | <span data-ttu-id="2cb02-158">说明</span><span class="sxs-lookup"><span data-stu-id="2cb02-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2cb02-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cb02-159">Authorization</span></span>  | <span data-ttu-id="2cb02-160">string</span><span class="sxs-lookup"><span data-stu-id="2cb02-160">string</span></span>  | <span data-ttu-id="2cb02-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2cb02-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2cb02-163">请求正文</span><span class="sxs-lookup"><span data-stu-id="2cb02-163">Request body</span></span>
<span data-ttu-id="2cb02-164">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2cb02-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cb02-165">响应</span><span class="sxs-lookup"><span data-stu-id="2cb02-165">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="2cb02-166">获取照片的响应</span><span class="sxs-lookup"><span data-stu-id="2cb02-166">Response for getting the photo</span></span>
<span data-ttu-id="2cb02-p108">如果成功，此方法返回 `200 OK` 响应代码和所请求照片的二进制数据。如果照片不存在，此操作返回 `404 Not Found`。</span><span class="sxs-lookup"><span data-stu-id="2cb02-p108">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="2cb02-169">获取照片元数据的响应</span><span class="sxs-lookup"><span data-stu-id="2cb02-169">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="2cb02-170">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilephoto.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2cb02-170">If successful, this method returns a `200 OK` response code and a [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2cb02-171">示例</span><span class="sxs-lookup"><span data-stu-id="2cb02-171">Examples</span></span>

### <a name="example-1-get-the-photo-of-the-signed-in-user-in-the-largest-available-size"></a><span data-ttu-id="2cb02-172">示例 1：为已登录用户获取最大可用大小的照片</span><span class="sxs-lookup"><span data-stu-id="2cb02-172">Example 1: Get the photo of the signed-in user in the largest available size</span></span>

##### <a name="request"></a><span data-ttu-id="2cb02-173">请求</span><span class="sxs-lookup"><span data-stu-id="2cb02-173">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="2cb02-174">响应</span><span class="sxs-lookup"><span data-stu-id="2cb02-174">Response</span></span>
<span data-ttu-id="2cb02-175">包含所请求照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="2cb02-175">Contains the binary data of the requested photo.</span></span> <span data-ttu-id="2cb02-176">HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="2cb02-176">The HTTP response code is 200.</span></span>

### <a name="example-2-get-the-48x48-photo-for-the-signed-in-user"></a><span data-ttu-id="2cb02-177">示例 2：获取已登录用户的 48x48 照片</span><span class="sxs-lookup"><span data-stu-id="2cb02-177">Example 2: Get the 48x48 photo for the signed-in user</span></span>

##### <a name="request"></a><span data-ttu-id="2cb02-178">请求</span><span class="sxs-lookup"><span data-stu-id="2cb02-178">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="2cb02-179">响应</span><span class="sxs-lookup"><span data-stu-id="2cb02-179">Response</span></span>
<span data-ttu-id="2cb02-180">包含所请求的 48x48 照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="2cb02-180">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="2cb02-181">HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="2cb02-181">The HTTP response code is 200.</span></span>

### <a name="example-3-get-the-metadata-of-the-user-photo-of-the-signed-in-user"></a><span data-ttu-id="2cb02-182">示例 3：获取已登录用户的用户照片的元数据</span><span class="sxs-lookup"><span data-stu-id="2cb02-182">Example 3: Get the metadata of the user photo of the signed-in user</span></span>

##### <a name="request"></a><span data-ttu-id="2cb02-183">请求</span><span class="sxs-lookup"><span data-stu-id="2cb02-183">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response"></a><span data-ttu-id="2cb02-184">响应</span><span class="sxs-lookup"><span data-stu-id="2cb02-184">Response</span></span>
<span data-ttu-id="2cb02-185">以下响应数据显示照片的元数据。</span><span class="sxs-lookup"><span data-stu-id="2cb02-185">The following response data shows the photo metadata.</span></span> 

><span data-ttu-id="2cb02-186">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2cb02-186">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

<span data-ttu-id="2cb02-187">以下响应数据显示还没有为用户上传照片时的响应内容。</span><span class="sxs-lookup"><span data-stu-id="2cb02-187">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user.</span></span> 

><span data-ttu-id="2cb02-188">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2cb02-188">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="2cb02-189">使用所请求照片的二进制数据</span><span class="sxs-lookup"><span data-stu-id="2cb02-189">Using the binary data of the requested photo</span></span>

<span data-ttu-id="2cb02-190">使用 `/photo/$value` 终结点来获取个人资料照片的二进制数据时，需要将数据转换为 Base64 字符串，以便将其添加为电子邮件附件。</span><span class="sxs-lookup"><span data-stu-id="2cb02-190">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="2cb02-191">以下 JavaScript 示例介绍如何创建一个数组，并将其作为 [Outlook 邮件](user-post-messages.md)的 `Attachments` 参数值传递。</span><span class="sxs-lookup"><span data-stu-id="2cb02-191">The following JavaScript example shows how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="2cb02-192">有关此示例的实现，请参阅[用于 Node.js 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/nodejs-connect-rest-sample)。</span><span class="sxs-lookup"><span data-stu-id="2cb02-192">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="2cb02-193">如果想要在网页上显示图像，可以通过图像创建内存中对象，然后使该对象成为图像元素源。</span><span class="sxs-lookup"><span data-stu-id="2cb02-193">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="2cb02-194">以下示例演示了如何在 JavaScript 中执行此操作。</span><span class="sxs-lookup"><span data-stu-id="2cb02-194">Here is an example in JavaScript of this operation.</span></span>

    const url = window.URL || window.webkitURL;
    const blobUrl = url.createObjectURL(image.data);
    document.getElementById(imageElement).setAttribute("src", blobUrl);

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
