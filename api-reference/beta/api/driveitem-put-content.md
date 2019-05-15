---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 上传小文件
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 28c3076c351755cf65ae1cbd83a6cc2c36c1544b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33960884"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="97457-102">上传或替换 DriveItem 的内容</span><span class="sxs-lookup"><span data-stu-id="97457-102">Upload or replace the contents of a DriveItem</span></span>

<span data-ttu-id="97457-p101">通过简单的上载 API，你可以在单个 API 调用中提供新文件的内容，也可以更新现有文件的内容。此方法仅支持最大大小为 4 MB 的文件。</span><span class="sxs-lookup"><span data-stu-id="97457-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="97457-105">若要上传大文件，请参阅[通过上传会话上传大文件](driveitem-createuploadsession.md)。</span><span class="sxs-lookup"><span data-stu-id="97457-105">To upload large files see [Upload large files with an upload session](driveitem-createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="97457-106">权限</span><span class="sxs-lookup"><span data-stu-id="97457-106">Permissions</span></span>

<span data-ttu-id="97457-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97457-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97457-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="97457-109">Permission type</span></span>      | <span data-ttu-id="97457-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97457-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97457-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97457-111">Delegated (work or school account)</span></span> | <span data-ttu-id="97457-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97457-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="97457-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97457-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97457-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97457-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="97457-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="97457-115">Application</span></span> | <span data-ttu-id="97457-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97457-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="97457-117">HTTP 请求（替换现有项）</span><span class="sxs-lookup"><span data-stu-id="97457-117">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="97457-118">HTTP 请求（上传新文件）</span><span class="sxs-lookup"><span data-stu-id="97457-118">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="97457-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="97457-119">Request body</span></span>

<span data-ttu-id="97457-120">请求正文的内容应该是要上载文件的二进制流。</span><span class="sxs-lookup"><span data-stu-id="97457-120">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="97457-121">响应</span><span class="sxs-lookup"><span data-stu-id="97457-121">Response</span></span>

<span data-ttu-id="97457-122">如果成功，此方法将在新创建或更新的文件的响应正文中返回 [driveItem](../resources/driveitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="97457-122">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created or updated file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="97457-123">示例（上传新文件）</span><span class="sxs-lookup"><span data-stu-id="97457-123">Example (upload a new file)</span></span>

<span data-ttu-id="97457-124">此示例将字符串“The contents of the file goes here.”上传到</span><span class="sxs-lookup"><span data-stu-id="97457-124">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="97457-125">登录用户的驱动器中 FolderA 下名为 FileB.txt 的文件中。</span><span class="sxs-lookup"><span data-stu-id="97457-125">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="97457-126">响应</span><span class="sxs-lookup"><span data-stu-id="97457-126">Response</span></span>

<span data-ttu-id="97457-127">如果成功，此方法将在响应正文中返回新建文件的 [driveItem][item-resource] 资源。</span><span class="sxs-lookup"><span data-stu-id="97457-127">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="97457-128">示例（更新现有文件）</span><span class="sxs-lookup"><span data-stu-id="97457-128">Example (updating an existing file)</span></span>

<span data-ttu-id="97457-129">此示例将文件的内容替换为已知 ID。</span><span class="sxs-lookup"><span data-stu-id="97457-129">This example replaces the contents of a file with a known ID.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="97457-130">响应</span><span class="sxs-lookup"><span data-stu-id="97457-130">Response</span></span>

<span data-ttu-id="97457-131">如果成功，此方法将在响应正文中返回新建文件的 [driveItem][item-resource] 资源。</span><span class="sxs-lookup"><span data-stu-id="97457-131">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="97457-132">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="97457-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="97457-133">C#</span><span class="sxs-lookup"><span data-stu-id="97457-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/upload-via-put-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97457-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="97457-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/upload-via-put-id-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="error-responses"></a><span data-ttu-id="97457-135">错误响应</span><span class="sxs-lookup"><span data-stu-id="97457-135">Error responses</span></span>

<span data-ttu-id="97457-136">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="97457-136">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-put-content.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-put-content.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
