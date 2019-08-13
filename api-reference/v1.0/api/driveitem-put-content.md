---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 上传小文件
localization_priority: Priority
ms.prod: sharepoint
description: '通过简单上传 API，可以在一个 API 调用中提供新文件的内容或更新现有文件的内容。 '
doc_type: apiPageType
ms.openlocfilehash: f2918e1fddbd91fe843b4f2d02a470a90f798ec9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373411"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="ad8e0-103">上传或替换 driveItem 的内容</span><span class="sxs-lookup"><span data-stu-id="ad8e0-103">Upload or replace the contents of a DriveItem</span></span>

<span data-ttu-id="ad8e0-p101">通过简单的上载 API，你可以在单个 API 调用中提供新文件的内容，也可以更新现有文件的内容。此方法仅支持最大大小为 4 MB 的文件。</span><span class="sxs-lookup"><span data-stu-id="ad8e0-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="ad8e0-106">若要上传大文件，请参阅[通过上传会话上传大文件](driveitem-createuploadsession.md)。</span><span class="sxs-lookup"><span data-stu-id="ad8e0-106">To upload large files see [Upload large files with an upload session](driveitem-createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad8e0-107">权限</span><span class="sxs-lookup"><span data-stu-id="ad8e0-107">Permissions</span></span>

<span data-ttu-id="ad8e0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad8e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad8e0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad8e0-110">Permission type</span></span>      | <span data-ttu-id="ad8e0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad8e0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad8e0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad8e0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ad8e0-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad8e0-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad8e0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad8e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad8e0-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad8e0-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad8e0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad8e0-116">Application</span></span> | <span data-ttu-id="ad8e0-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad8e0-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="ad8e0-118">HTTP 请求（替换现有项）</span><span class="sxs-lookup"><span data-stu-id="ad8e0-118">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="ad8e0-119">HTTP 请求（上传新文件）</span><span class="sxs-lookup"><span data-stu-id="ad8e0-119">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="ad8e0-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad8e0-120">Request body</span></span>

<span data-ttu-id="ad8e0-121">请求正文的内容应该是要上载文件的二进制流。</span><span class="sxs-lookup"><span data-stu-id="ad8e0-121">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="ad8e0-122">响应</span><span class="sxs-lookup"><span data-stu-id="ad8e0-122">Response</span></span>

<span data-ttu-id="ad8e0-123">如果成功，此方法将在新创建或更新的文件的响应正文中返回 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ad8e0-123">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created or updated file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="ad8e0-124">示例（上传新文件）</span><span class="sxs-lookup"><span data-stu-id="ad8e0-124">Example (upload a new file)</span></span>

<span data-ttu-id="ad8e0-125">此示例将字符串“The contents of the file goes here.”上传到</span><span class="sxs-lookup"><span data-stu-id="ad8e0-125">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="ad8e0-126">登录用户的驱动器中 FolderA 下名为 FileB.txt 的文件中。</span><span class="sxs-lookup"><span data-stu-id="ad8e0-126">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="ad8e0-127">响应</span><span class="sxs-lookup"><span data-stu-id="ad8e0-127">Response</span></span>

<span data-ttu-id="ad8e0-128">如果成功，此方法将在响应正文中返回新建文件的 [driveItem][item-resource] 资源。</span><span class="sxs-lookup"><span data-stu-id="ad8e0-128">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="ad8e0-129">示例（更新现有文件）</span><span class="sxs-lookup"><span data-stu-id="ad8e0-129">Example (updating an existing file)</span></span>

<span data-ttu-id="ad8e0-130">此示例将文件的内容替换为已知 ID。</span><span class="sxs-lookup"><span data-stu-id="ad8e0-130">This example replaces the contents of a file with a known ID.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ad8e0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad8e0-131">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ad8e0-132">C#</span><span class="sxs-lookup"><span data-stu-id="ad8e0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upload-via-put-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad8e0-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad8e0-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upload-via-put-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ad8e0-134">响应</span><span class="sxs-lookup"><span data-stu-id="ad8e0-134">Response</span></span>

<span data-ttu-id="ad8e0-135">如果成功，此方法将在响应正文中返回新建文件的 [driveItem][item-resource] 资源。</span><span class="sxs-lookup"><span data-stu-id="ad8e0-135">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="ad8e0-136">错误响应</span><span class="sxs-lookup"><span data-stu-id="ad8e0-136">Error responses</span></span>

<span data-ttu-id="ad8e0-137">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="ad8e0-137">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation",
  "suppressions": [
  ]
} -->
