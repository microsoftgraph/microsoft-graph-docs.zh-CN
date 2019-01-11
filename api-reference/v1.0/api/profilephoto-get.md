---
title: 获取照片
description: 获取指定的 profilePhoto 或其元数据（profilePhoto 属性）。
localization_priority: Priority
ms.openlocfilehash: 6b1a3e54b1145cc2fdcf8ed9e587652d4d7061c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833948"
---
# <a name="get-photo"></a><span data-ttu-id="e3288-103">获取照片</span><span class="sxs-lookup"><span data-stu-id="e3288-103">Get photo</span></span>

<span data-ttu-id="e3288-104">获取指定的 [profilePhoto](../resources/profilephoto.md) 或其元数据（profilePhoto 属性）。</span><span class="sxs-lookup"><span data-stu-id="e3288-104">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

> <span data-ttu-id="e3288-105">**注意**：在版本 1.0 中，此操作仅支持用户的工作或学校邮箱，不支持个人邮箱。</span><span class="sxs-lookup"><span data-stu-id="e3288-105">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

<span data-ttu-id="e3288-106">Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。</span><span class="sxs-lookup"><span data-stu-id="e3288-106">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="e3288-107">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="e3288-107">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="e3288-108">可以获取最大照片的元数据，也可以指定尺寸来获取相应照片尺寸的元数据。</span><span class="sxs-lookup"><span data-stu-id="e3288-108">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="e3288-109">如果请求的大小不可用，则仍然可以获取用户已上载且可供使用的较小大小。</span><span class="sxs-lookup"><span data-stu-id="e3288-109">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="e3288-110">例如，如果用户上传像素为 504x504 的照片，除 648x648 外所有尺寸的照片都可供下载。</span><span class="sxs-lookup"><span data-stu-id="e3288-110">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3288-111">权限</span><span class="sxs-lookup"><span data-stu-id="e3288-111">Permissions</span></span>

<span data-ttu-id="e3288-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3288-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3288-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3288-114">Permission type</span></span>      | <span data-ttu-id="e3288-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3288-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3288-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3288-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e3288-117">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="e3288-117">For **user** resource:</span></span><br/><span data-ttu-id="e3288-118">User.Read、User.ReadBasic.All、User.Read.All、User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3288-118">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e3288-119">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="e3288-119">For **group** resource:</span></span><br /><span data-ttu-id="e3288-120">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3288-120">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e3288-121">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="e3288-121">For **contact** resource:</span></span><br /><span data-ttu-id="e3288-122">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3288-122">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="e3288-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3288-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3288-124">不支持</span><span class="sxs-lookup"><span data-stu-id="e3288-124">Not supported</span></span> |
|<span data-ttu-id="e3288-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3288-125">Application</span></span>                        | <span data-ttu-id="e3288-126">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="e3288-126">For **user** resource:</span></span><br/><span data-ttu-id="e3288-127">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3288-127">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e3288-128">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="e3288-128">For **group** resource:</span></span><br /><span data-ttu-id="e3288-129">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3288-129">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e3288-130">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="e3288-130">For **contact** resource:</span></span><br /><span data-ttu-id="e3288-131">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3288-131">Contacts.Read, Contacts.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="e3288-132">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3288-132">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="e3288-133">获取照片</span><span class="sxs-lookup"><span data-stu-id="e3288-133">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="e3288-134">获取元数据的照片</span><span class="sxs-lookup"><span data-stu-id="e3288-134">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="e3288-135">获取特定照片大小的元数据</span><span class="sxs-lookup"><span data-stu-id="e3288-135">Get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
GET /me/contacts/{id}/photos/{size}
GET /users/{id | userPrincipalName}/contacts/{id}/photos/{size}
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photos/{size}
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="e3288-136">路径参数</span><span class="sxs-lookup"><span data-stu-id="e3288-136">Path parameters</span></span>

|<span data-ttu-id="e3288-137">参数</span><span class="sxs-lookup"><span data-stu-id="e3288-137">Parameter</span></span>|<span data-ttu-id="e3288-138">类型</span><span class="sxs-lookup"><span data-stu-id="e3288-138">Type</span></span>|<span data-ttu-id="e3288-139">说明</span><span class="sxs-lookup"><span data-stu-id="e3288-139">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e3288-140">size</span><span class="sxs-lookup"><span data-stu-id="e3288-140">size</span></span>  |<span data-ttu-id="e3288-141">String</span><span class="sxs-lookup"><span data-stu-id="e3288-141">String</span></span>  | <span data-ttu-id="e3288-142">照片尺寸。</span><span class="sxs-lookup"><span data-stu-id="e3288-142">A photo size.</span></span> <span data-ttu-id="e3288-143">Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。</span><span class="sxs-lookup"><span data-stu-id="e3288-143">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="e3288-144">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="e3288-144">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="e3288-145">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e3288-145">Optional query parameters</span></span>
<span data-ttu-id="e3288-146">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e3288-146">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3288-147">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3288-147">Request headers</span></span>
| <span data-ttu-id="e3288-148">名称</span><span class="sxs-lookup"><span data-stu-id="e3288-148">Name</span></span>       | <span data-ttu-id="e3288-149">类型</span><span class="sxs-lookup"><span data-stu-id="e3288-149">Type</span></span> | <span data-ttu-id="e3288-150">说明</span><span class="sxs-lookup"><span data-stu-id="e3288-150">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e3288-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3288-151">Authorization</span></span>  | <span data-ttu-id="e3288-152">string</span><span class="sxs-lookup"><span data-stu-id="e3288-152">string</span></span>  | <span data-ttu-id="e3288-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3288-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3288-155">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3288-155">Request body</span></span>
<span data-ttu-id="e3288-156">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e3288-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3288-157">响应</span><span class="sxs-lookup"><span data-stu-id="e3288-157">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="e3288-158">获取照片的响应</span><span class="sxs-lookup"><span data-stu-id="e3288-158">Response for getting the photo</span></span>
<span data-ttu-id="e3288-p106">如果成功，此方法返回 `200 OK` 响应代码和所请求照片的二进制数据。如果照片不存在，此操作返回 `404 Not Found`。</span><span class="sxs-lookup"><span data-stu-id="e3288-p106">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="e3288-161">获取照片元数据的响应</span><span class="sxs-lookup"><span data-stu-id="e3288-161">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="e3288-162">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilephoto.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e3288-162">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e3288-163">示例</span><span class="sxs-lookup"><span data-stu-id="e3288-163">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e3288-164">请求 1</span><span class="sxs-lookup"><span data-stu-id="e3288-164">Request 1</span></span>
<span data-ttu-id="e3288-165">此请求为已登录用户获取最大可用大小的照片。</span><span class="sxs-lookup"><span data-stu-id="e3288-165">This request gets the photo for the signed-in user, in the largest available size.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a><span data-ttu-id="e3288-166">响应 1</span><span class="sxs-lookup"><span data-stu-id="e3288-166">Response 1</span></span>
<span data-ttu-id="e3288-p107">包含所请求照片的二进制数据。HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="e3288-p107">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="e3288-169">请求 2</span><span class="sxs-lookup"><span data-stu-id="e3288-169">Request 2</span></span>
<span data-ttu-id="e3288-170">此请求获取已登录用户的 48x48 照片。</span><span class="sxs-lookup"><span data-stu-id="e3288-170">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="e3288-171">响应 2</span><span class="sxs-lookup"><span data-stu-id="e3288-171">Response 2</span></span>
<span data-ttu-id="e3288-p108">包含所请求的 48x48 照片的二进制数据。HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="e3288-p108">Contains the binary data of the requested 48x48 photo. The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="e3288-174">请求 3</span><span class="sxs-lookup"><span data-stu-id="e3288-174">Request 3</span></span>
<span data-ttu-id="e3288-175">此请求获取已登录用户的用户照片的元数据。</span><span class="sxs-lookup"><span data-stu-id="e3288-175">This request gets the metadata of the user photo of the signed-in user.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="e3288-176">响应 3</span><span class="sxs-lookup"><span data-stu-id="e3288-176">Response 3</span></span>

<span data-ttu-id="e3288-p109">以下响应数据显示照片的元数据。注意：为了简单起见，可能会将此处所示的响应对象截断。</span><span class="sxs-lookup"><span data-stu-id="e3288-p109">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>
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

<span data-ttu-id="e3288-p110">以下响应数据显示还没有为用户上载照片时的响应内容。注意：为了简单起见，可能会将此处所示的响应对象截断。</span><span class="sxs-lookup"><span data-stu-id="e3288-p110">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="e3288-181">使用所请求照片的二进制数据</span><span class="sxs-lookup"><span data-stu-id="e3288-181">Using the binary data of the requested photo</span></span>

<span data-ttu-id="e3288-182">使用 `/photo/$value` 终结点来获取个人资料照片的二进制数据时，需要将数据转换为 Base64 字符串，以便将其添加为电子邮件附件。</span><span class="sxs-lookup"><span data-stu-id="e3288-182">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="e3288-183">以下是 JavaScript 中的一个示例，介绍如何创建一个数组，并将其作为 [Outlook 邮件](user-post-messages.md)的 `Attachments` 参数值传递。</span><span class="sxs-lookup"><span data-stu-id="e3288-183">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="e3288-184">有关此示例的实现，请参阅[用于 Node.js 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/nodejs-connect-rest-sample)。</span><span class="sxs-lookup"><span data-stu-id="e3288-184">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="e3288-185">如果想要在网页上显示图像，可以通过图像创建内存中对象，然后使该对象成为图像元素源。</span><span class="sxs-lookup"><span data-stu-id="e3288-185">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="e3288-186">以下示例演示了如何在 JavaScript 中执行此操作。</span><span class="sxs-lookup"><span data-stu-id="e3288-186">Here is an example in JavaScript of this operation.</span></span>

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
