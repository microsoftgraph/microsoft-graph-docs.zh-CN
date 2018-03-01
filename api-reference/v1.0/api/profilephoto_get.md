# <a name="get-photo"></a><span data-ttu-id="53ceb-101">获取照片</span><span class="sxs-lookup"><span data-stu-id="53ceb-101">Get photo</span></span>

<span data-ttu-id="53ceb-102">获取指定的 [profilePhoto](../resources/profilephoto.md) 或其元数据（profilePhoto 属性）。</span><span class="sxs-lookup"><span data-stu-id="53ceb-102">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

<span data-ttu-id="53ceb-103">GET 操作查找用户邮箱在 Exchange Online 上的指定照片。</span><span class="sxs-lookup"><span data-stu-id="53ceb-103">A GET operation looks for the specified photo in the user's mailbox on Exchange Online.</span></span>

> <span data-ttu-id="53ceb-104">**注意**：1.0 版本中的操作仅支持用户的工作或学校邮箱，不支持个人邮箱。</span><span class="sxs-lookup"><span data-stu-id="53ceb-104">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="53ceb-105">权限</span><span class="sxs-lookup"><span data-stu-id="53ceb-105">Permissions</span></span>
<span data-ttu-id="53ceb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="53ceb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

*   <span data-ttu-id="53ceb-108">租户中任意用户的个人资料照片，包括已登录用户 - User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53ceb-108">Profile photo of any user in the tenant including the signed-in user - User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>
*   <span data-ttu-id="53ceb-109">特别是已登录用户的个人资料照片 - User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53ceb-109">Profile photo of specifically the signed-in user - User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>
* <span data-ttu-id="53ceb-110">**组**的个人资料照片 - Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53ceb-110">Profile photo of a **group** - Group.Read.All, Group.ReadWrite.All</span></span>
* <span data-ttu-id="53ceb-111">**联系人**的照片 - Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53ceb-111">Photo of a **contact** - Contacts.Read, Contacts.ReadWrite</span></span>

## <a name="http-request-to-get-the-photo"></a><span data-ttu-id="53ceb-112">获取照片的 HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53ceb-112">HTTP request to get the photo</span></span>
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
## <a name="http-request-to-get-the-metadata-of-the-photo"></a><span data-ttu-id="53ceb-113">获取照片元数据的 HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53ceb-113">HTTP request to get the metadata of the photo</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="53ceb-114">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="53ceb-114">Optional query parameters</span></span>
<span data-ttu-id="53ceb-115">此方法支持 [OData 查询参数](http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="53ceb-115">This method supports the [OData Query Parameters](http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53ceb-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="53ceb-116">Request headers</span></span>
| <span data-ttu-id="53ceb-117">名称</span><span class="sxs-lookup"><span data-stu-id="53ceb-117">Name</span></span>       | <span data-ttu-id="53ceb-118">类型</span><span class="sxs-lookup"><span data-stu-id="53ceb-118">Type</span></span> | <span data-ttu-id="53ceb-119">说明</span><span class="sxs-lookup"><span data-stu-id="53ceb-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="53ceb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="53ceb-120">Authorization</span></span>  | <span data-ttu-id="53ceb-121">string</span><span class="sxs-lookup"><span data-stu-id="53ceb-121">string</span></span>  | <span data-ttu-id="53ceb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53ceb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53ceb-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="53ceb-124">Request body</span></span>
<span data-ttu-id="53ceb-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53ceb-125">Do not supply a request body for this method.</span></span>
## <a name="response-for-getting-the-photo"></a><span data-ttu-id="53ceb-126">获取照片的响应</span><span class="sxs-lookup"><span data-stu-id="53ceb-126">Response for getting the photo</span></span>
<span data-ttu-id="53ceb-p103">如果成功，此方法返回 `200 OK` 响应代码和所请求照片的二进制数据。如果照片不存在，此操作返回 `404 Not Found`。</span><span class="sxs-lookup"><span data-stu-id="53ceb-p103">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
## <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="53ceb-129">获取照片元数据的响应</span><span class="sxs-lookup"><span data-stu-id="53ceb-129">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="53ceb-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilePhoto.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53ceb-130">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilePhoto.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="53ceb-131">示例</span><span class="sxs-lookup"><span data-stu-id="53ceb-131">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="53ceb-132">请求 1</span><span class="sxs-lookup"><span data-stu-id="53ceb-132">Request 1</span></span>
<span data-ttu-id="53ceb-133">此请求为已登录用户获取最大可用大小的照片。</span><span class="sxs-lookup"><span data-stu-id="53ceb-133">This request gets the photo for the signed-in user, in the largest available size.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a><span data-ttu-id="53ceb-134">响应 1</span><span class="sxs-lookup"><span data-stu-id="53ceb-134">Response 1</span></span>
<span data-ttu-id="53ceb-p104">包含所请求照片的二进制数据。HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="53ceb-p104">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="53ceb-137">请求 2</span><span class="sxs-lookup"><span data-stu-id="53ceb-137">Request 2</span></span>
<span data-ttu-id="53ceb-138">此请求获取已登录用户的用户照片的元数据。</span><span class="sxs-lookup"><span data-stu-id="53ceb-138">This request gets the metadata of the user photo of the signed-in user.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-2"></a><span data-ttu-id="53ceb-139">响应 2</span><span class="sxs-lookup"><span data-stu-id="53ceb-139">Response 2</span></span>

<span data-ttu-id="53ceb-p105">以下响应数据显示照片的元数据。注意：为了简单起见，可能会将此处所示的响应对象截断。</span><span class="sxs-lookup"><span data-stu-id="53ceb-p105">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>
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

<span data-ttu-id="53ceb-p106">以下响应数据显示还没有为用户上载照片时的响应内容。注意：为了简单起见，可能会将此处所示的响应对象截断。</span><span class="sxs-lookup"><span data-stu-id="53ceb-p106">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="53ceb-144">使用所请求照片的二进制数据</span><span class="sxs-lookup"><span data-stu-id="53ceb-144">Using the binary data of the requested photo</span></span>

<span data-ttu-id="53ceb-145">使用 `/photo/$value` 终结点来获取个人资料照片的二进制数据时，需要将数据转换为 Base64 字符串，以便将其添加为电子邮件附件。</span><span class="sxs-lookup"><span data-stu-id="53ceb-145">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="53ceb-146">以下是 JavaScript 中的一个示例，介绍如何创建一个数组，并将其作为 [Outlook 邮件](user_post_messages.md)的 `Attachments` 参数值传递。</span><span class="sxs-lookup"><span data-stu-id="53ceb-146">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user_post_messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="53ceb-147">有关此示例的实现，请参阅[用于 Node.js 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/nodejs-connect-rest-sample)。</span><span class="sxs-lookup"><span data-stu-id="53ceb-147">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="53ceb-148">如果想要在网页上显示图像，可以通过图像创建内存中对象，然后使该对象成为图像元素源。</span><span class="sxs-lookup"><span data-stu-id="53ceb-148">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="53ceb-149">以下示例演示了如何在 JavaScript 中执行此操作。</span><span class="sxs-lookup"><span data-stu-id="53ceb-149">Here is an example in JavaScript of this operation.</span></span>

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
