---
title: 下载 DriveItemVersion 资源的内容
description: 检索某个特定版本的 DriveItem 的内容。
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 3b30987686c91ff6ab4ac35e352f79f7b4e60951
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006897"
---
# <a name="download-contents-of-a-driveitemversion-resource"></a><span data-ttu-id="ef90b-103">下载 DriveItemVersion 资源的内容</span><span class="sxs-lookup"><span data-stu-id="ef90b-103">Download contents of a DriveItemVersion resource</span></span>

<span data-ttu-id="ef90b-104">检索某个特定版本的 [DriveItem](../resources/driveitem.md) 的内容。</span><span class="sxs-lookup"><span data-stu-id="ef90b-104">Retrieve the contents of a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ef90b-105">权限</span><span class="sxs-lookup"><span data-stu-id="ef90b-105">Permissions</span></span>

<span data-ttu-id="ef90b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef90b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef90b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef90b-108">Permission type</span></span>      | <span data-ttu-id="ef90b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ef90b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef90b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef90b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ef90b-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef90b-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef90b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef90b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef90b-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef90b-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef90b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef90b-114">Application</span></span> | <span data-ttu-id="ef90b-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef90b-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="ef90b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef90b-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="ef90b-117">响应</span><span class="sxs-lookup"><span data-stu-id="ef90b-117">Response</span></span>

<span data-ttu-id="ef90b-118">返回 `302 Found` 响应，重定向到文件字节已预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="ef90b-118">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="ef90b-p102">若要下载该文件的内容，应用程序将需要遵循响应中的 `Location` 标头。许多 HTTP 客户端库将自动遵循 302 重定向并立即开始下载文件。</span><span class="sxs-lookup"><span data-stu-id="ef90b-p102">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="ef90b-121">预先验证的下载 URL 仅在较短的一段时间 （几分钟后）内有效，不需要 `Authorization` 标头即可下载。</span><span class="sxs-lookup"><span data-stu-id="ef90b-121">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="ef90b-122">示例</span><span class="sxs-lookup"><span data-stu-id="ef90b-122">Example</span></span>

<span data-ttu-id="ef90b-123">本示例检索当前用户驱动器中的文件版本。</span><span class="sxs-lookup"><span data-stu-id="ef90b-123">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="ef90b-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef90b-124">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ef90b-125">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ef90b-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ef90b-126">C#</span><span class="sxs-lookup"><span data-stu-id="ef90b-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-version-contents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef90b-127">Javascript</span><span class="sxs-lookup"><span data-stu-id="ef90b-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-version-contents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ef90b-128">目标-C</span><span class="sxs-lookup"><span data-stu-id="ef90b-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-version-contents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ef90b-129">Java</span><span class="sxs-lookup"><span data-stu-id="ef90b-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-version-contents-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ef90b-130">响应</span><span class="sxs-lookup"><span data-stu-id="ef90b-130">Response</span></span>

<span data-ttu-id="ef90b-131">会返回一个重定向链接，可以在其中下载版本的内容。</span><span class="sxs-lookup"><span data-stu-id="ef90b-131">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Found
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="ef90b-132">注解</span><span class="sxs-lookup"><span data-stu-id="ef90b-132">Remarks</span></span>

<span data-ttu-id="ef90b-133">OneDrive 不保留文件以前版本的完整元数据。</span><span class="sxs-lookup"><span data-stu-id="ef90b-133">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="ef90b-134">当应用程序检索文件的可用版本列表时，将返回 [DriveItemVersion](../resources/driveitemversion.md) 资源，它提供有关特定版本的可用信息。</span><span class="sxs-lookup"><span data-stu-id="ef90b-134">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
} -->
