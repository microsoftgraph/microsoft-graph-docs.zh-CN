---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 上传小文件
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1b6ec254dd56de3b678aa0c6a3d5c95a8f149837
ms.sourcegitcommit: b198efc2391a12a840e4f1b8c42c18a55b06037f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2019
ms.locfileid: "35820703"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="24551-102">上传或替换 DriveItem 的内容</span><span class="sxs-lookup"><span data-stu-id="24551-102">Upload or replace the contents of a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24551-p101">通过简单的上载 API，你可以在单个 API 调用中提供新文件的内容，也可以更新现有文件的内容。此方法仅支持最大大小为 4 MB 的文件。</span><span class="sxs-lookup"><span data-stu-id="24551-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="24551-105">若要上传大文件，请参阅[通过上传会话上传大文件](driveitem-createuploadsession.md)。</span><span class="sxs-lookup"><span data-stu-id="24551-105">To upload large files see [Upload large files with an upload session](driveitem-createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="24551-106">权限</span><span class="sxs-lookup"><span data-stu-id="24551-106">Permissions</span></span>

<span data-ttu-id="24551-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24551-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24551-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="24551-109">Permission type</span></span>      | <span data-ttu-id="24551-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24551-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24551-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24551-111">Delegated (work or school account)</span></span> | <span data-ttu-id="24551-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24551-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="24551-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24551-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24551-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24551-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="24551-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="24551-115">Application</span></span> | <span data-ttu-id="24551-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24551-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="24551-117">HTTP 请求（替换现有项）</span><span class="sxs-lookup"><span data-stu-id="24551-117">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="24551-118">HTTP 请求（上传新文件）</span><span class="sxs-lookup"><span data-stu-id="24551-118">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="24551-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="24551-119">Request body</span></span>

<span data-ttu-id="24551-120">请求正文的内容应该是要上载文件的二进制流。</span><span class="sxs-lookup"><span data-stu-id="24551-120">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="24551-121">响应</span><span class="sxs-lookup"><span data-stu-id="24551-121">Response</span></span>

<span data-ttu-id="24551-122">如果成功，此方法将在新创建或更新的文件的响应正文中返回 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="24551-122">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created or updated file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="24551-123">示例（上传新文件）</span><span class="sxs-lookup"><span data-stu-id="24551-123">Example (upload a new file)</span></span>

<span data-ttu-id="24551-124">此示例将字符串“The contents of the file goes here.”上传到</span><span class="sxs-lookup"><span data-stu-id="24551-124">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="24551-125">登录用户的驱动器中 FolderA 下名为 FileB.txt 的文件中。</span><span class="sxs-lookup"><span data-stu-id="24551-125">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="24551-126">响应</span><span class="sxs-lookup"><span data-stu-id="24551-126">Response</span></span>

<span data-ttu-id="24551-127">如果成功, 此方法在响应正文中返回新创建或更新的文件的[driveItem][item-resource]资源。</span><span class="sxs-lookup"><span data-stu-id="24551-127">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created or updated file.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="24551-128">示例（更新现有文件）</span><span class="sxs-lookup"><span data-stu-id="24551-128">Example (updating an existing file)</span></span>

<span data-ttu-id="24551-129">此示例将文件的内容替换为已知 ID。</span><span class="sxs-lookup"><span data-stu-id="24551-129">This example replaces the contents of a file with a known ID.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="24551-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="24551-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="24551-131">C#</span><span class="sxs-lookup"><span data-stu-id="24551-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upload-via-put-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24551-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="24551-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upload-via-put-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="24551-133">响应</span><span class="sxs-lookup"><span data-stu-id="24551-133">Response</span></span>

<span data-ttu-id="24551-134">如果成功，此方法将在响应正文中返回新建文件的 [driveItem][item-resource] 资源。</span><span class="sxs-lookup"><span data-stu-id="24551-134">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="error-responses"></a><span data-ttu-id="24551-135">错误响应</span><span class="sxs-lookup"><span data-stu-id="24551-135">Error responses</span></span>

<span data-ttu-id="24551-136">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="24551-136">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation",
  "suppressions": [
  ]
}
-->
