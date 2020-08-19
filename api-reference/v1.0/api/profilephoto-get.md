---
title: 获取照片
description: 获取指定的 profilePhoto 或其元数据（profilePhoto 属性）。
localization_priority: Priority
author: kevinbellinger
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 7e3731d225ec86ba0a4789401394fa062085d992
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807057"
---
# <a name="get-photo"></a><span data-ttu-id="a42d2-103">获取照片</span><span class="sxs-lookup"><span data-stu-id="a42d2-103">Get photo</span></span>

<span data-ttu-id="a42d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a42d2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a42d2-105">获取指定的 [profilePhoto](../resources/profilephoto.md) 或其元数据（profilePhoto 属性）。</span><span class="sxs-lookup"><span data-stu-id="a42d2-105">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

> <span data-ttu-id="a42d2-106">**注意**：在版本 1.0 中，此操作仅支持用户的工作或学校邮箱，不支持个人邮箱。</span><span class="sxs-lookup"><span data-stu-id="a42d2-106">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

<span data-ttu-id="a42d2-107">Microsoft 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。</span><span class="sxs-lookup"><span data-stu-id="a42d2-107">The supported sizes of HD photos on Microsoft 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="a42d2-108">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="a42d2-108">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="a42d2-109">可以获取最大照片的元数据，也可以指定尺寸来获取相应照片尺寸的元数据。</span><span class="sxs-lookup"><span data-stu-id="a42d2-109">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="a42d2-110">如果请求的大小不可用，则仍然可以获取用户已上载且可供使用的较小大小。</span><span class="sxs-lookup"><span data-stu-id="a42d2-110">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="a42d2-111">例如，如果用户上传像素为 504x504 的照片，除 648x648 外的所有尺寸的照片都可供下载。</span><span class="sxs-lookup"><span data-stu-id="a42d2-111">For example, if the user uploads a photo that is 504x504 pixels, all but the 648x648 size of photo will be available for download.</span></span>

## <a name="permissions"></a><span data-ttu-id="a42d2-112">权限</span><span class="sxs-lookup"><span data-stu-id="a42d2-112">Permissions</span></span>

<span data-ttu-id="a42d2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a42d2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a42d2-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="a42d2-115">Permission type</span></span>      | <span data-ttu-id="a42d2-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a42d2-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a42d2-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a42d2-117">Delegated (work or school account)</span></span> | <span data-ttu-id="a42d2-118">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="a42d2-118">For **user** resource:</span></span><br/><span data-ttu-id="a42d2-119">User.Read、User.ReadBasic.All、User.Read.All、User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a42d2-119">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="a42d2-120">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="a42d2-120">For **group** resource:</span></span><br /><span data-ttu-id="a42d2-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a42d2-121">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="a42d2-122">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="a42d2-122">For **contact** resource:</span></span><br /><span data-ttu-id="a42d2-123">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a42d2-123">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="a42d2-124">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a42d2-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a42d2-125">不支持</span><span class="sxs-lookup"><span data-stu-id="a42d2-125">Not supported</span></span> |
|<span data-ttu-id="a42d2-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="a42d2-126">Application</span></span>                        | <span data-ttu-id="a42d2-127">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="a42d2-127">For **user** resource:</span></span><br/><span data-ttu-id="a42d2-128">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a42d2-128">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="a42d2-129">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="a42d2-129">For **group** resource:</span></span><br /><span data-ttu-id="a42d2-130">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a42d2-130">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="a42d2-131">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="a42d2-131">For **contact** resource:</span></span><br /><span data-ttu-id="a42d2-132">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a42d2-132">Contacts.Read, Contacts.ReadWrite</span></span> |

> <span data-ttu-id="a42d2-133">**注意：** 当前有一个[已知问题](/graph/known-issues#groups)，即使用应用程序权限访问组照片。</span><span class="sxs-lookup"><span data-stu-id="a42d2-133">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="a42d2-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a42d2-134">HTTP request</span></span>

### <a name="get-the-photo"></a><span data-ttu-id="a42d2-135">获取照片</span><span class="sxs-lookup"><span data-stu-id="a42d2-135">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="a42d2-136">获取照片的元数据</span><span class="sxs-lookup"><span data-stu-id="a42d2-136">Get the metadata of the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo
GET /me/photos
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="a42d2-137">获取指定照片尺寸的元数据</span><span class="sxs-lookup"><span data-stu-id="a42d2-137">Get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="a42d2-138">路径参数</span><span class="sxs-lookup"><span data-stu-id="a42d2-138">Path parameters</span></span>

|<span data-ttu-id="a42d2-139">参数</span><span class="sxs-lookup"><span data-stu-id="a42d2-139">Parameter</span></span>|<span data-ttu-id="a42d2-140">类型</span><span class="sxs-lookup"><span data-stu-id="a42d2-140">Type</span></span>|<span data-ttu-id="a42d2-141">说明</span><span class="sxs-lookup"><span data-stu-id="a42d2-141">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a42d2-142">size</span><span class="sxs-lookup"><span data-stu-id="a42d2-142">size</span></span>  |<span data-ttu-id="a42d2-143">String</span><span class="sxs-lookup"><span data-stu-id="a42d2-143">String</span></span>  | <span data-ttu-id="a42d2-144">照片尺寸。</span><span class="sxs-lookup"><span data-stu-id="a42d2-144">A photo size.</span></span> <span data-ttu-id="a42d2-145">Microsoft 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。</span><span class="sxs-lookup"><span data-stu-id="a42d2-145">The supported sizes of HD photos on Microsoft 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="a42d2-146">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="a42d2-146">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="a42d2-147">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a42d2-147">Optional query parameters</span></span>
<span data-ttu-id="a42d2-148">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a42d2-148">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a42d2-149">请求标头</span><span class="sxs-lookup"><span data-stu-id="a42d2-149">Request headers</span></span>
| <span data-ttu-id="a42d2-150">名称</span><span class="sxs-lookup"><span data-stu-id="a42d2-150">Name</span></span>       | <span data-ttu-id="a42d2-151">类型</span><span class="sxs-lookup"><span data-stu-id="a42d2-151">Type</span></span> | <span data-ttu-id="a42d2-152">说明</span><span class="sxs-lookup"><span data-stu-id="a42d2-152">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a42d2-153">Authorization</span><span class="sxs-lookup"><span data-stu-id="a42d2-153">Authorization</span></span>  | <span data-ttu-id="a42d2-154">string</span><span class="sxs-lookup"><span data-stu-id="a42d2-154">string</span></span>  | <span data-ttu-id="a42d2-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a42d2-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a42d2-157">请求正文</span><span class="sxs-lookup"><span data-stu-id="a42d2-157">Request body</span></span>
<span data-ttu-id="a42d2-158">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a42d2-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a42d2-159">响应</span><span class="sxs-lookup"><span data-stu-id="a42d2-159">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="a42d2-160">获取照片的响应</span><span class="sxs-lookup"><span data-stu-id="a42d2-160">Response for getting the photo</span></span>
<span data-ttu-id="a42d2-p106">如果成功，此方法返回 `200 OK` 响应代码和所请求照片的二进制数据。如果照片不存在，此操作返回 `404 Not Found`。</span><span class="sxs-lookup"><span data-stu-id="a42d2-p106">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="a42d2-163">获取照片元数据的响应</span><span class="sxs-lookup"><span data-stu-id="a42d2-163">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="a42d2-164">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilephoto.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a42d2-164">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="a42d2-165">示例</span><span class="sxs-lookup"><span data-stu-id="a42d2-165">Examples</span></span>

### <a name="example-1-get-the-photo-for-the-signed-in-user-in-the-largest-available-size"></a><span data-ttu-id="a42d2-166">示例 1：为已登录用户获取最大可用大小的照片</span><span class="sxs-lookup"><span data-stu-id="a42d2-166">Example 1: Get the photo for the signed-in user in the largest available size</span></span>
##### <a name="request"></a><span data-ttu-id="a42d2-167">请求</span><span class="sxs-lookup"><span data-stu-id="a42d2-167">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response"></a><span data-ttu-id="a42d2-168">响应</span><span class="sxs-lookup"><span data-stu-id="a42d2-168">Response</span></span>
<span data-ttu-id="a42d2-169">包含所请求照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="a42d2-169">Contains the binary data of the requested photo.</span></span> <span data-ttu-id="a42d2-170">HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="a42d2-170">The HTTP response code is 200.</span></span>

### <a name="example-2-get-the-48x48-photo-for-the-signed-in-use"></a><span data-ttu-id="a42d2-171">示例 2：为已登录用户获取 48x48 的照片</span><span class="sxs-lookup"><span data-stu-id="a42d2-171">Example 2: Get the 48x48 photo for the signed-in use</span></span>
##### <a name="request"></a><span data-ttu-id="a42d2-172">请求</span><span class="sxs-lookup"><span data-stu-id="a42d2-172">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="a42d2-173">响应</span><span class="sxs-lookup"><span data-stu-id="a42d2-173">Response</span></span>
<span data-ttu-id="a42d2-174">包含所请求的 48x48 照片的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="a42d2-174">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="a42d2-175">HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="a42d2-175">The HTTP response code is 200.</span></span>

### <a name="example-3-get-the-metadata-of-the-user-photo-of-the-signed-in-user"></a><span data-ttu-id="a42d2-176">示例 3：获取已登录用户的用户照片的元数据</span><span class="sxs-lookup"><span data-stu-id="a42d2-176">Example 3: Get the metadata of the user photo of the signed-in user</span></span>
##### <a name="request"></a><span data-ttu-id="a42d2-177">请求</span><span class="sxs-lookup"><span data-stu-id="a42d2-177">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response"></a><span data-ttu-id="a42d2-178">响应</span><span class="sxs-lookup"><span data-stu-id="a42d2-178">Response</span></span>

<span data-ttu-id="a42d2-179">以下响应数据显示照片的元数据。</span><span class="sxs-lookup"><span data-stu-id="a42d2-179">The following response data shows the photo metadata.</span></span>

><span data-ttu-id="a42d2-180">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a42d2-180">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

<span data-ttu-id="a42d2-181">以下响应数据显示还没有为用户上传照片时的响应内容。</span><span class="sxs-lookup"><span data-stu-id="a42d2-181">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user.</span></span>

><span data-ttu-id="a42d2-182">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a42d2-182">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="a42d2-183">使用所请求照片的二进制数据</span><span class="sxs-lookup"><span data-stu-id="a42d2-183">Using the binary data of the requested photo</span></span>

<span data-ttu-id="a42d2-184">使用 `/photo/$value` 终结点来获取个人资料照片的二进制数据时，需要将数据转换为 Base64 字符串，以便将其添加为电子邮件附件。</span><span class="sxs-lookup"><span data-stu-id="a42d2-184">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="a42d2-185">以下是 JavaScript 中的一个示例，介绍如何创建一个数组，并将其作为 [Outlook 邮件](user-post-messages.md)的 `Attachments` 参数值传递。</span><span class="sxs-lookup"><span data-stu-id="a42d2-185">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="a42d2-186">有关此示例的实现，请参阅[用于 Node.js 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/nodejs-connect-rest-sample)。</span><span class="sxs-lookup"><span data-stu-id="a42d2-186">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="a42d2-187">如果想要在网页上显示图像，可以通过图像创建内存中对象，然后使该对象成为图像元素源。</span><span class="sxs-lookup"><span data-stu-id="a42d2-187">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="a42d2-188">以下示例演示了如何在 JavaScript 中执行此操作。</span><span class="sxs-lookup"><span data-stu-id="a42d2-188">Here is an example in JavaScript of this operation.</span></span>

    const url = window.URL || window.webkitURL;
    const blobUrl = url.createObjectURL(image.data);
    document.getElementById(imageElement).setAttribute("src", blobUrl);

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
