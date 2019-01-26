---
title: 获取照片
description: 获取指定的 profilePhoto 或其元数据（**profilePhoto** 属性）。
localization_priority: Priority
ms.openlocfilehash: 759c0ff3ac2585f43ea38963e10b001250702c56
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509628"
---
# <a name="get-photo"></a><span data-ttu-id="dbe94-103">获取照片</span><span class="sxs-lookup"><span data-stu-id="dbe94-103">Get photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbe94-104">获取指定的 [profilePhoto](../resources/profilephoto.md) 或其元数据（**profilePhoto** 属性）。</span><span class="sxs-lookup"><span data-stu-id="dbe94-104">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (**profilePhoto** properties).</span></span>

<span data-ttu-id="dbe94-105">获取照片操作首先会尝试从 Office 365 检索指定的照片。</span><span class="sxs-lookup"><span data-stu-id="dbe94-105">A GET photo operation first attempt to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="dbe94-106">如果 Office 365 中没有此照片，则 API 会尝试从 Azure Active Directory 检索该照片。</span><span class="sxs-lookup"><span data-stu-id="dbe94-106">If the photo is not available in Office 365, the API attempts to retrieve the photo from Azure Active Directory.</span></span>

<span data-ttu-id="dbe94-107">Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。</span><span class="sxs-lookup"><span data-stu-id="dbe94-107">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="dbe94-108">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="dbe94-108">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="dbe94-109">可以获取最大照片的元数据，也可以指定尺寸来获取相应照片尺寸的元数据。</span><span class="sxs-lookup"><span data-stu-id="dbe94-109">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="dbe94-110">如果请求的大小不可用，则仍然可以获取用户已上载且可供使用的较小大小。</span><span class="sxs-lookup"><span data-stu-id="dbe94-110">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="dbe94-111">例如，如果用户上传像素为 504x504 的照片，除 648x648 外所有尺寸的照片都可供下载。</span><span class="sxs-lookup"><span data-stu-id="dbe94-111">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>
<span data-ttu-id="dbe94-112">如果在用户邮箱或 Azure Active Directory 中找不到指定尺寸，返回的是尺寸“1x1”和剩余元数据。</span><span class="sxs-lookup"><span data-stu-id="dbe94-112">If the specified size is not available in the user's mailbox or in Azure Active Directory, the size of '1x1' is returned with the rest of metadata.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbe94-113">权限</span><span class="sxs-lookup"><span data-stu-id="dbe94-113">Permissions</span></span>
<span data-ttu-id="dbe94-p104">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dbe94-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="dbe94-116">**注意：** 测试版中的获取照片操作支持用户的工作、学校或个人帐户。</span><span class="sxs-lookup"><span data-stu-id="dbe94-116">**Note:** The GET photo operation in beta supports a user's work, school, or personal accounts.</span></span> <span data-ttu-id="dbe94-117">但是获取照片元数据操作仅支持用户的工作或学校帐户，不支持个人帐户。</span><span class="sxs-lookup"><span data-stu-id="dbe94-117">The GET photo metadata operation, however, supports only the user's work or school accounts and not personal accounts.</span></span>

|<span data-ttu-id="dbe94-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="dbe94-118">Permission type</span></span>      | <span data-ttu-id="dbe94-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dbe94-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbe94-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbe94-120">Delegated (work or school account)</span></span> | <span data-ttu-id="dbe94-121">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="dbe94-121">For **user** resource:</span></span><br/><span data-ttu-id="dbe94-122">User.Read、User.ReadBasic.All、User.Read.All、User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbe94-122">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="dbe94-123">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="dbe94-123">For **group** resource:</span></span><br /><span data-ttu-id="dbe94-124">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbe94-124">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="dbe94-125">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="dbe94-125">For **contact** resource:</span></span><br /><span data-ttu-id="dbe94-126">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbe94-126">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="dbe94-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbe94-127">Delegated (personal Microsoft account)</span></span>  <br /> <span data-ttu-id="dbe94-128">**注意**：不支持元数据操作。</span><span class="sxs-lookup"><span data-stu-id="dbe94-128">**Note**: Metadata operation is not supported.</span></span> | <span data-ttu-id="dbe94-129">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="dbe94-129">For **user** resource:</span></span><br/><span data-ttu-id="dbe94-130">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbe94-130">User.Read, User.ReadWrite</span></span><br /><br /><span data-ttu-id="dbe94-131">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="dbe94-131">For **contact** resource:</span></span><br /><span data-ttu-id="dbe94-132">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbe94-132">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="dbe94-133">Application</span><span class="sxs-lookup"><span data-stu-id="dbe94-133">Application</span></span>                        | <span data-ttu-id="dbe94-134">对于 **user** 资源：</span><span class="sxs-lookup"><span data-stu-id="dbe94-134">For **user** resource:</span></span><br/><span data-ttu-id="dbe94-135">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbe94-135">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="dbe94-136">对于 **group** 资源：</span><span class="sxs-lookup"><span data-stu-id="dbe94-136">For **group** resource:</span></span><br /><span data-ttu-id="dbe94-137">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbe94-137">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="dbe94-138">对于 **contact** 资源：</span><span class="sxs-lookup"><span data-stu-id="dbe94-138">For **contact** resource:</span></span><br /><span data-ttu-id="dbe94-139">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbe94-139">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbe94-140">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dbe94-140">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="dbe94-141">获取照片</span><span class="sxs-lookup"><span data-stu-id="dbe94-141">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="dbe94-142">获取照片的元数据</span><span class="sxs-lookup"><span data-stu-id="dbe94-142">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="dbe94-143">获取指定照片尺寸的元数据</span><span class="sxs-lookup"><span data-stu-id="dbe94-143">Get the metadata for a specific photo size</span></span>
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

## <a name="path-parameters"></a><span data-ttu-id="dbe94-144">路径参数</span><span class="sxs-lookup"><span data-stu-id="dbe94-144">Path parameters</span></span>

|<span data-ttu-id="dbe94-145">**参数**</span><span class="sxs-lookup"><span data-stu-id="dbe94-145">**Parameter**</span></span>|<span data-ttu-id="dbe94-146">**类型**</span><span class="sxs-lookup"><span data-stu-id="dbe94-146">**Type**</span></span>|<span data-ttu-id="dbe94-147">**说明**</span><span class="sxs-lookup"><span data-stu-id="dbe94-147">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="dbe94-148">size</span><span class="sxs-lookup"><span data-stu-id="dbe94-148">size</span></span>  |<span data-ttu-id="dbe94-149">String</span><span class="sxs-lookup"><span data-stu-id="dbe94-149">String</span></span>  | <span data-ttu-id="dbe94-150">照片尺寸。</span><span class="sxs-lookup"><span data-stu-id="dbe94-150">A photo size.</span></span> <span data-ttu-id="dbe94-151">Office 365 支持以下高清照片尺寸：48x48、64x64、96x96、120x120、240x240、360x360、432x432、504x504 和 648x648。</span><span class="sxs-lookup"><span data-stu-id="dbe94-151">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="dbe94-152">如果照片存储在 Azure Active Directory 中，可以采用任何尺寸。</span><span class="sxs-lookup"><span data-stu-id="dbe94-152">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="dbe94-153">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dbe94-153">Optional query parameters</span></span>
<span data-ttu-id="dbe94-154">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dbe94-154">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dbe94-155">请求标头</span><span class="sxs-lookup"><span data-stu-id="dbe94-155">Request headers</span></span>
| <span data-ttu-id="dbe94-156">名称</span><span class="sxs-lookup"><span data-stu-id="dbe94-156">Name</span></span>       | <span data-ttu-id="dbe94-157">类型</span><span class="sxs-lookup"><span data-stu-id="dbe94-157">Type</span></span> | <span data-ttu-id="dbe94-158">说明</span><span class="sxs-lookup"><span data-stu-id="dbe94-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dbe94-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbe94-159">Authorization</span></span>  | <span data-ttu-id="dbe94-160">string</span><span class="sxs-lookup"><span data-stu-id="dbe94-160">string</span></span>  | <span data-ttu-id="dbe94-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dbe94-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbe94-163">请求正文</span><span class="sxs-lookup"><span data-stu-id="dbe94-163">Request body</span></span>
<span data-ttu-id="dbe94-164">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dbe94-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbe94-165">响应</span><span class="sxs-lookup"><span data-stu-id="dbe94-165">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="dbe94-166">获取照片的响应</span><span class="sxs-lookup"><span data-stu-id="dbe94-166">Response for getting the photo</span></span>
<span data-ttu-id="dbe94-p108">如果成功，此方法返回 `200 OK` 响应代码和所请求照片的二进制数据。如果照片不存在，此操作返回 `404 Not Found`。</span><span class="sxs-lookup"><span data-stu-id="dbe94-p108">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="dbe94-169">获取照片元数据的响应</span><span class="sxs-lookup"><span data-stu-id="dbe94-169">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="dbe94-170">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [profilePhoto](../resources/profilephoto.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dbe94-170">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbe94-171">示例</span><span class="sxs-lookup"><span data-stu-id="dbe94-171">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="dbe94-172">请求 1</span><span class="sxs-lookup"><span data-stu-id="dbe94-172">Request 1</span></span>
<span data-ttu-id="dbe94-173">此请求为已登录用户获取最大可用大小的照片。</span><span class="sxs-lookup"><span data-stu-id="dbe94-173">This request gets the photo for the signed-in user, in the largest available size.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response-1"></a><span data-ttu-id="dbe94-174">响应 1</span><span class="sxs-lookup"><span data-stu-id="dbe94-174">Response 1</span></span>
<span data-ttu-id="dbe94-p109">包含所请求照片的二进制数据。HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="dbe94-p109">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="dbe94-177">请求 2</span><span class="sxs-lookup"><span data-stu-id="dbe94-177">Request 2</span></span>
<span data-ttu-id="dbe94-178">此请求获取已登录用户的 48x48 照片。</span><span class="sxs-lookup"><span data-stu-id="dbe94-178">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="dbe94-179">响应 2</span><span class="sxs-lookup"><span data-stu-id="dbe94-179">Response 2</span></span>
<span data-ttu-id="dbe94-p110">包含所请求的 48x48 照片的二进制数据。HTTP 响应代码为 200。</span><span class="sxs-lookup"><span data-stu-id="dbe94-p110">Contains the binary data of the requested 48x48 photo. The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="dbe94-182">请求 3</span><span class="sxs-lookup"><span data-stu-id="dbe94-182">Request 3</span></span>
<span data-ttu-id="dbe94-183">此请求获取已登录用户的用户照片的元数据。</span><span class="sxs-lookup"><span data-stu-id="dbe94-183">This request gets the metadata of the user photo of the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="dbe94-184">响应 3</span><span class="sxs-lookup"><span data-stu-id="dbe94-184">Response 3</span></span>
<span data-ttu-id="dbe94-p111">以下响应数据显示照片的元数据。注意：为了简单起见，可能会将此处所示的响应对象截断。</span><span class="sxs-lookup"><span data-stu-id="dbe94-p111">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="dbe94-p112">以下响应数据显示还没有为用户上载照片时的响应内容。注意：为了简单起见，可能会将此处所示的响应对象截断。</span><span class="sxs-lookup"><span data-stu-id="dbe94-p112">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="dbe94-189">使用所请求照片的二进制数据</span><span class="sxs-lookup"><span data-stu-id="dbe94-189">Using the binary data of the requested photo</span></span>

<span data-ttu-id="dbe94-190">使用 `/photo/$value` 终结点来获取个人资料照片的二进制数据时，需要将数据转换为 Base64 字符串，以便将其添加为电子邮件附件。</span><span class="sxs-lookup"><span data-stu-id="dbe94-190">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="dbe94-191">以下是 JavaScript 中的一个示例，介绍如何创建一个数组，并将其作为 [Outlook 邮件](user-post-messages.md)的 `Attachments` 参数值传递。</span><span class="sxs-lookup"><span data-stu-id="dbe94-191">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="dbe94-192">有关此示例的实现，请参阅[用于 Node.js 的 Microsoft Graph Connect 示例](https://github.com/microsoftgraph/nodejs-connect-rest-sample)。</span><span class="sxs-lookup"><span data-stu-id="dbe94-192">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="dbe94-193">如果想要在网页上显示图像，可以通过图像创建内存中对象，然后使该对象成为图像元素源。</span><span class="sxs-lookup"><span data-stu-id="dbe94-193">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="dbe94-194">以下示例演示了如何在 JavaScript 中执行此操作。</span><span class="sxs-lookup"><span data-stu-id="dbe94-194">Here is an example in JavaScript of this operation.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/profilephoto-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
