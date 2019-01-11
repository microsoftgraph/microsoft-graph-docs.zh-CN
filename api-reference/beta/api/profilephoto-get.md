---
title: 获取照片
description: 获取指定的 profilePhoto 或其元数据 （**profilePhoto**属性）。
localization_priority: Priority
ms.openlocfilehash: be20e243a89d258c8db2105efe0c53cbea0abebf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851735"
---
# <a name="get-photo"></a><span data-ttu-id="58436-103">获取照片</span><span class="sxs-lookup"><span data-stu-id="58436-103">Get photo</span></span>

> <span data-ttu-id="58436-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="58436-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58436-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="58436-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="58436-106">获取指定的[profilePhoto](../resources/profilephoto.md)或其元数据 （**profilePhoto**属性）。</span><span class="sxs-lookup"><span data-stu-id="58436-106">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (**profilePhoto** properties).</span></span>

<span data-ttu-id="58436-107">GET 照片操作第一次尝试从 Office 365 中检索指定的照片。</span><span class="sxs-lookup"><span data-stu-id="58436-107">A GET photo operation first attempt to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="58436-108">如果照片不是 Office 365 中可用，API 尝试从 Azure Active Directory 中检索照片。</span><span class="sxs-lookup"><span data-stu-id="58436-108">If the photo is not available in Office 365, the API attempts to retrieve the photo from Azure Active Directory.</span></span>

<span data-ttu-id="58436-109">Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。</span><span class="sxs-lookup"><span data-stu-id="58436-109">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="58436-110">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="58436-110">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="58436-111">可以获取最大照片的元数据，也可以指定尺寸来获取相应照片尺寸的元数据。</span><span class="sxs-lookup"><span data-stu-id="58436-111">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="58436-112">如果请求的大小不可用，则仍然可以获取用户已上载且可供使用的较小大小。</span><span class="sxs-lookup"><span data-stu-id="58436-112">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="58436-113">例如，如果用户上传像素为 504x504 的照片，除 648x648 外所有尺寸的照片都可供下载。</span><span class="sxs-lookup"><span data-stu-id="58436-113">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>
<span data-ttu-id="58436-114">如果在用户邮箱或 Azure Active Directory 中找不到指定尺寸，返回的是尺寸“1x1”和剩余元数据。</span><span class="sxs-lookup"><span data-stu-id="58436-114">If the specified size is not available in the user's mailbox or in Azure Active Directory, the size of '1x1' is returned with the rest of metadata.</span></span>

## <a name="permissions"></a><span data-ttu-id="58436-115">权限</span><span class="sxs-lookup"><span data-stu-id="58436-115">Permissions</span></span>
<span data-ttu-id="58436-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58436-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="58436-118">**注意：** GET 照片操作 beta 中的支持用户的工作、 学习或个人帐户。</span><span class="sxs-lookup"><span data-stu-id="58436-118">**Note:** The GET photo operation in beta supports a user's work, school, or personal accounts.</span></span> <span data-ttu-id="58436-119">获取照片元数据操作，但是，仅支持用户工作或学校帐户和不适用于个人帐户。</span><span class="sxs-lookup"><span data-stu-id="58436-119">The GET photo metadata operation, however, supports only the user's work or school accounts and not personal accounts.</span></span>

|<span data-ttu-id="58436-120">权限类型</span><span class="sxs-lookup"><span data-stu-id="58436-120">Permission type</span></span>      | <span data-ttu-id="58436-121">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="58436-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58436-122">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58436-122">Delegated (work or school account)</span></span> | <span data-ttu-id="58436-123">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="58436-123">For **user** resource:</span></span><br/><span data-ttu-id="58436-124">User.Read、User.ReadBasic.All、User.Read.All、User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58436-124">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="58436-125">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="58436-125">For **group** resource:</span></span><br /><span data-ttu-id="58436-126">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58436-126">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="58436-127">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="58436-127">For **contact** resource:</span></span><br /><span data-ttu-id="58436-128">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58436-128">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="58436-129">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58436-129">Delegated (personal Microsoft account)</span></span>  <br /> <span data-ttu-id="58436-130">**注意**： 元数据操作不受支持。</span><span class="sxs-lookup"><span data-stu-id="58436-130">**Note**: Metadata operation is not supported.</span></span> | <span data-ttu-id="58436-131">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="58436-131">For **user** resource:</span></span><br/><span data-ttu-id="58436-132">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58436-132">User.Read, User.ReadWrite</span></span><br /><br /><span data-ttu-id="58436-133">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="58436-133">For **contact** resource:</span></span><br /><span data-ttu-id="58436-134">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58436-134">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="58436-135">应用程序</span><span class="sxs-lookup"><span data-stu-id="58436-135">Application</span></span>                        | <span data-ttu-id="58436-136">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="58436-136">For **user** resource:</span></span><br/><span data-ttu-id="58436-137">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58436-137">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="58436-138">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="58436-138">For **group** resource:</span></span><br /><span data-ttu-id="58436-139">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58436-139">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="58436-140">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="58436-140">For **contact** resource:</span></span><br /><span data-ttu-id="58436-141">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58436-141">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="58436-142">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58436-142">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="58436-143">获取照片</span><span class="sxs-lookup"><span data-stu-id="58436-143">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="58436-144">获取元数据的照片</span><span class="sxs-lookup"><span data-stu-id="58436-144">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="58436-145">获取特定照片大小的元数据</span><span class="sxs-lookup"><span data-stu-id="58436-145">Get the metadata for a specific photo size</span></span>
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

## <a name="path-parameters"></a><span data-ttu-id="58436-146">路径参数</span><span class="sxs-lookup"><span data-stu-id="58436-146">Path parameters</span></span>

|<span data-ttu-id="58436-147">**参数**</span><span class="sxs-lookup"><span data-stu-id="58436-147">**Parameter**</span></span>|<span data-ttu-id="58436-148">**类型**</span><span class="sxs-lookup"><span data-stu-id="58436-148">**Type**</span></span>|<span data-ttu-id="58436-149">**说明**</span><span class="sxs-lookup"><span data-stu-id="58436-149">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="58436-150">size</span><span class="sxs-lookup"><span data-stu-id="58436-150">size</span></span>  |<span data-ttu-id="58436-151">String</span><span class="sxs-lookup"><span data-stu-id="58436-151">String</span></span>  | <span data-ttu-id="58436-152">照片尺寸。</span><span class="sxs-lookup"><span data-stu-id="58436-152">A photo size.</span></span> <span data-ttu-id="58436-153">Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。</span><span class="sxs-lookup"><span data-stu-id="58436-153">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="58436-154">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="58436-154">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="58436-155">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="58436-155">Optional query parameters</span></span>
<span data-ttu-id="58436-156">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="58436-156">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58436-157">请求标头</span><span class="sxs-lookup"><span data-stu-id="58436-157">Request headers</span></span>
| <span data-ttu-id="58436-158">名称</span><span class="sxs-lookup"><span data-stu-id="58436-158">Name</span></span>       | <span data-ttu-id="58436-159">类型</span><span class="sxs-lookup"><span data-stu-id="58436-159">Type</span></span> | <span data-ttu-id="58436-160">说明</span><span class="sxs-lookup"><span data-stu-id="58436-160">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="58436-161">Authorization</span><span class="sxs-lookup"><span data-stu-id="58436-161">Authorization</span></span>  | <span data-ttu-id="58436-162">string</span><span class="sxs-lookup"><span data-stu-id="58436-162">string</span></span>  | <span data-ttu-id="58436-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="58436-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58436-165">请求正文</span><span class="sxs-lookup"><span data-stu-id="58436-165">Request body</span></span>
<span data-ttu-id="58436-166">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="58436-166">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58436-167">响应</span><span class="sxs-lookup"><span data-stu-id="58436-167">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="58436-168">获取照片的响应</span><span class="sxs-lookup"><span data-stu-id="58436-168">Response for getting the photo</span></span>
<span data-ttu-id="58436-p109">如果成功，此方法返回 `200 OK` 响应代码和所请求照片的二进制数据。如果照片不存在，此操作返回 `404 Not Found`。</span><span class="sxs-lookup"><span data-stu-id="58436-p109">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="58436-171">获取照片元数据的响应</span><span class="sxs-lookup"><span data-stu-id="58436-171">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="58436-172">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilephoto.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58436-172">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58436-173">示例</span><span class="sxs-lookup"><span data-stu-id="58436-173">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="58436-174">请求 1</span><span class="sxs-lookup"><span data-stu-id="58436-174">Request 1</span></span>
<span data-ttu-id="58436-175">此请求为已登录用户获取最大可用大小的照片。</span><span class="sxs-lookup"><span data-stu-id="58436-175">This request gets the photo for the signed-in user, in the largest available size.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response-1"></a><span data-ttu-id="58436-176">响应 1</span><span class="sxs-lookup"><span data-stu-id="58436-176">Response 1</span></span>
<span data-ttu-id="58436-p110">包含所请求照片的二进制数据。HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="58436-p110">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="58436-179">请求 2</span><span class="sxs-lookup"><span data-stu-id="58436-179">Request 2</span></span>
<span data-ttu-id="58436-180">此请求获取已登录用户的 48x48 照片。</span><span class="sxs-lookup"><span data-stu-id="58436-180">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="58436-181">响应 2</span><span class="sxs-lookup"><span data-stu-id="58436-181">Response 2</span></span>
<span data-ttu-id="58436-p111">包含所请求的 48x48 照片的二进制数据。HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="58436-p111">Contains the binary data of the requested 48x48 photo. The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="58436-184">请求 3</span><span class="sxs-lookup"><span data-stu-id="58436-184">Request 3</span></span>
<span data-ttu-id="58436-185">此请求获取已登录用户的用户照片的元数据。</span><span class="sxs-lookup"><span data-stu-id="58436-185">This request gets the metadata of the user photo of the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="58436-186">响应 3</span><span class="sxs-lookup"><span data-stu-id="58436-186">Response 3</span></span>
<span data-ttu-id="58436-p112">以下响应数据显示照片的元数据。注意：为了简单起见，可能会将此处所示的响应对象截断。</span><span class="sxs-lookup"><span data-stu-id="58436-p112">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="58436-p113">以下响应数据显示还没有为用户上载照片时的响应内容。注意：为了简单起见，可能会将此处所示的响应对象截断。</span><span class="sxs-lookup"><span data-stu-id="58436-p113">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="58436-191">使用所请求照片的二进制数据</span><span class="sxs-lookup"><span data-stu-id="58436-191">Using the binary data of the requested photo</span></span>

<span data-ttu-id="58436-192">使用 `/photo/$value` 终结点来获取个人资料照片的二进制数据时，需要将数据转换为 Base64 字符串，以便将其添加为电子邮件附件。</span><span class="sxs-lookup"><span data-stu-id="58436-192">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="58436-193">以下是 JavaScript 中的一个示例，介绍如何创建一个数组，并将其作为 [Outlook 邮件](user-post-messages.md)的 `Attachments` 参数值传递。</span><span class="sxs-lookup"><span data-stu-id="58436-193">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="58436-194">有关此示例的实现，请参阅[用于 Node.js 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/nodejs-connect-rest-sample)。</span><span class="sxs-lookup"><span data-stu-id="58436-194">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="58436-195">如果想要在网页上显示图像，可以通过图像创建内存中对象，然后使该对象成为图像元素源。</span><span class="sxs-lookup"><span data-stu-id="58436-195">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="58436-196">以下示例演示了如何在 JavaScript 中执行此操作。</span><span class="sxs-lookup"><span data-stu-id="58436-196">Here is an example in JavaScript of this operation.</span></span>

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
