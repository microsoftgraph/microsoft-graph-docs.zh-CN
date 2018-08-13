# <a name="get-photo"></a><span data-ttu-id="1da69-101">获取照片</span><span class="sxs-lookup"><span data-stu-id="1da69-101">Get photo</span></span>

<span data-ttu-id="1da69-102">获取指定的 [profilePhoto](../resources/profilephoto.md) 或其元数据（profilePhoto 属性）。</span><span class="sxs-lookup"><span data-stu-id="1da69-102">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

> <span data-ttu-id="1da69-103">**注意**：在版本 1.0 中，此操作仅支持用户的工作或学校邮箱，不支持个人邮箱。</span><span class="sxs-lookup"><span data-stu-id="1da69-103">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

<span data-ttu-id="1da69-104">Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。</span><span class="sxs-lookup"><span data-stu-id="1da69-104">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="1da69-105">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="1da69-105">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="1da69-106">可以获取最大照片的元数据，也可以指定尺寸来获取相应照片尺寸的元数据。</span><span class="sxs-lookup"><span data-stu-id="1da69-106">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="1da69-107">如果请求的大小不可用，则仍然可以获取用户已上载且可供使用的较小大小。</span><span class="sxs-lookup"><span data-stu-id="1da69-107">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="1da69-108">例如，如果用户上传像素为 504x504 的照片，除 648x648 外所有尺寸的照片都可供下载。</span><span class="sxs-lookup"><span data-stu-id="1da69-108">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>

## <a name="permissions"></a><span data-ttu-id="1da69-109">权限</span><span class="sxs-lookup"><span data-stu-id="1da69-109">Permissions</span></span>

<span data-ttu-id="1da69-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1da69-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1da69-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="1da69-112">Permission type</span></span>      | <span data-ttu-id="1da69-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1da69-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1da69-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1da69-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1da69-115">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="1da69-115">For **user** resource:</span></span><br/><span data-ttu-id="1da69-116">User.Read、User.ReadBasic.All、User.Read.All、User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1da69-116">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="1da69-117">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="1da69-117">For **group** resource:</span></span><br /><span data-ttu-id="1da69-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1da69-118">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="1da69-119">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="1da69-119">For **contact** resource:</span></span><br /><span data-ttu-id="1da69-120">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1da69-120">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="1da69-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1da69-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1da69-122">不支持</span><span class="sxs-lookup"><span data-stu-id="1da69-122">Not supported</span></span> |
|<span data-ttu-id="1da69-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="1da69-123">Application</span></span>                        | <span data-ttu-id="1da69-124">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="1da69-124">For **user** resource:</span></span><br/><span data-ttu-id="1da69-125">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1da69-125">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="1da69-126">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="1da69-126">For **group** resource:</span></span><br /><span data-ttu-id="1da69-127">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1da69-127">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="1da69-128">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="1da69-128">For **contact** resource:</span></span><br /><span data-ttu-id="1da69-129">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1da69-129">Contacts.Read, Contacts.ReadWrite</span></span> |


## <a name="http-request-to-get-the-photo"></a><span data-ttu-id="1da69-130">获取照片的 HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1da69-130">HTTP request to get the photo</span></span>
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
## <a name="http-request-to-get-the-metadata-of-the-photo"></a><span data-ttu-id="1da69-131">获取照片元数据的 HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1da69-131">HTTP request to get the metadata of the photo</span></span>
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

## <a name="http-request-to-get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="1da69-132">获取指定照片尺寸的元数据的 HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1da69-132">HTTP request to get the metadata for a specific photo size</span></span>
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

## <a name="parameters"></a><span data-ttu-id="1da69-133">参数</span><span class="sxs-lookup"><span data-stu-id="1da69-133">Parameters</span></span>

|<span data-ttu-id="1da69-134">**参数**</span><span class="sxs-lookup"><span data-stu-id="1da69-134">**Parameter**</span></span>|<span data-ttu-id="1da69-135">**类型**</span><span class="sxs-lookup"><span data-stu-id="1da69-135">**Type**</span></span>|<span data-ttu-id="1da69-136">**说明**</span><span class="sxs-lookup"><span data-stu-id="1da69-136">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1da69-137">_URL 参数_</span><span class="sxs-lookup"><span data-stu-id="1da69-137">_URL parameters_</span></span>|
|<span data-ttu-id="1da69-138">size</span><span class="sxs-lookup"><span data-stu-id="1da69-138">size</span></span>  |<span data-ttu-id="1da69-139">String</span><span class="sxs-lookup"><span data-stu-id="1da69-139">String</span></span>  | <span data-ttu-id="1da69-140">照片尺寸。</span><span class="sxs-lookup"><span data-stu-id="1da69-140">A photo size.</span></span> <span data-ttu-id="1da69-141">Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、</span><span class="sxs-lookup"><span data-stu-id="1da69-141">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240',</span></span> 
<span data-ttu-id="1da69-142">360x360、432x432、504x504 和 648x648。</span><span class="sxs-lookup"><span data-stu-id="1da69-142">'360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="1da69-143">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="1da69-143">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="1da69-144">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1da69-144">Optional query parameters</span></span>
<span data-ttu-id="1da69-145">此方法支持 [OData 查询参数](http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1da69-145">This method supports the [OData Query Parameters](http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1da69-146">请求标头</span><span class="sxs-lookup"><span data-stu-id="1da69-146">Request headers</span></span>
| <span data-ttu-id="1da69-147">名称</span><span class="sxs-lookup"><span data-stu-id="1da69-147">Name</span></span>       | <span data-ttu-id="1da69-148">类型</span><span class="sxs-lookup"><span data-stu-id="1da69-148">Type</span></span> | <span data-ttu-id="1da69-149">说明</span><span class="sxs-lookup"><span data-stu-id="1da69-149">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1da69-150">Authorization</span><span class="sxs-lookup"><span data-stu-id="1da69-150">Authorization</span></span>  | <span data-ttu-id="1da69-151">string</span><span class="sxs-lookup"><span data-stu-id="1da69-151">string</span></span>  | <span data-ttu-id="1da69-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1da69-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1da69-154">请求正文</span><span class="sxs-lookup"><span data-stu-id="1da69-154">Request body</span></span>
<span data-ttu-id="1da69-155">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1da69-155">Do not supply a request body for this method.</span></span>
## <a name="response-for-getting-the-photo"></a><span data-ttu-id="1da69-156">获取照片的响应</span><span class="sxs-lookup"><span data-stu-id="1da69-156">Response for getting the photo</span></span>
<span data-ttu-id="1da69-p107">如果成功，此方法返回 `200 OK` 响应代码和所请求照片的二进制数据。如果照片不存在，此操作返回 `404 Not Found`。</span><span class="sxs-lookup"><span data-stu-id="1da69-p107">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
## <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="1da69-159">获取照片元数据的响应</span><span class="sxs-lookup"><span data-stu-id="1da69-159">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="1da69-160">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilePhoto.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1da69-160">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilePhoto.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1da69-161">示例</span><span class="sxs-lookup"><span data-stu-id="1da69-161">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="1da69-162">请求 1</span><span class="sxs-lookup"><span data-stu-id="1da69-162">Request 1</span></span>
<span data-ttu-id="1da69-163">此请求为已登录用户获取最大可用大小的照片。</span><span class="sxs-lookup"><span data-stu-id="1da69-163">This request gets the photo for the signed-in user, in the largest available size.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a><span data-ttu-id="1da69-164">响应 1</span><span class="sxs-lookup"><span data-stu-id="1da69-164">Response 1</span></span>
<span data-ttu-id="1da69-p108">包含所请求照片的二进制数据。HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="1da69-p108">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="1da69-167">请求 2</span><span class="sxs-lookup"><span data-stu-id="1da69-167">Request 2</span></span>
<span data-ttu-id="1da69-168">此请求获取已登录用户的 48x48 照片。</span><span class="sxs-lookup"><span data-stu-id="1da69-168">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="1da69-169">响应 2</span><span class="sxs-lookup"><span data-stu-id="1da69-169">Response 2</span></span>
<span data-ttu-id="1da69-p109">包含所请求的 48x48 照片的二进制数据。HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="1da69-p109">Contains the binary data of the requested 48x48 photo. The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="1da69-172">请求 3</span><span class="sxs-lookup"><span data-stu-id="1da69-172">Request 3</span></span>
<span data-ttu-id="1da69-173">此请求获取已登录用户的用户照片的元数据。</span><span class="sxs-lookup"><span data-stu-id="1da69-173">This request gets the metadata of the user photo of the signed-in user.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="1da69-174">响应 3</span><span class="sxs-lookup"><span data-stu-id="1da69-174">Response 3</span></span>

<span data-ttu-id="1da69-p110">以下响应数据显示照片的元数据。注意：为了简单起见，可能会将此处所示的响应对象截断。</span><span class="sxs-lookup"><span data-stu-id="1da69-p110">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>
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

<span data-ttu-id="1da69-p111">以下响应数据显示还没有为用户上载照片时的响应内容。注意：为了简单起见，可能会将此处所示的响应对象截断。</span><span class="sxs-lookup"><span data-stu-id="1da69-p111">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="1da69-179">使用所请求照片的二进制数据</span><span class="sxs-lookup"><span data-stu-id="1da69-179">Using the binary data of the requested photo</span></span>

<span data-ttu-id="1da69-180">使用 `/photo/$value` 终结点来获取个人资料照片的二进制数据时，需要将数据转换为 Base64 字符串，以便将其添加为电子邮件附件。</span><span class="sxs-lookup"><span data-stu-id="1da69-180">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="1da69-181">以下是 JavaScript 中的一个示例，介绍如何创建一个数组，并将其作为 [Outlook 邮件](user_post_messages.md)的 `Attachments` 参数值传递。</span><span class="sxs-lookup"><span data-stu-id="1da69-181">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user_post_messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="1da69-182">有关此示例的实现，请参阅[用于 Node.js 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/nodejs-connect-rest-sample)。</span><span class="sxs-lookup"><span data-stu-id="1da69-182">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="1da69-183">如果想要在网页上显示图像，可以通过图像创建内存中对象，然后使该对象成为图像元素源。</span><span class="sxs-lookup"><span data-stu-id="1da69-183">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="1da69-184">以下示例演示了如何在 JavaScript 中执行此操作。</span><span class="sxs-lookup"><span data-stu-id="1da69-184">Here is an example in JavaScript of this operation.</span></span>

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
