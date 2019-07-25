---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 下载早期版本
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bd813caf274755ef13102e98e02132c3fda2d13e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860864"
---
# <a name="download-contents-of-a-driveitemversion-resource-preview"></a><span data-ttu-id="3d322-102">下载 DriveItemVersion 资源的内容（预览版）</span><span class="sxs-lookup"><span data-stu-id="3d322-102">Download contents of a DriveItemVersion resource (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d322-103">检索[driveItem](../resources/driveitem.md)的特定版本的内容。</span><span class="sxs-lookup"><span data-stu-id="3d322-103">Retrieve the contents of a specific version of a [driveItem](../resources/driveitem.md).</span></span> 

><span data-ttu-id="3d322-104">**注意:** 不支持获取当前版本的内容。</span><span class="sxs-lookup"><span data-stu-id="3d322-104">**Note:** Getting the content of the current version is not supported.</span></span> <span data-ttu-id="3d322-105">而是使用[driveItem 内容终结点](driveitem-get-content.md)。</span><span class="sxs-lookup"><span data-stu-id="3d322-105">Instead, use the [driveItem content endpoint](driveitem-get-content.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3d322-106">权限</span><span class="sxs-lookup"><span data-stu-id="3d322-106">Permissions</span></span>

<span data-ttu-id="3d322-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d322-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d322-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d322-109">Permission type</span></span>      | <span data-ttu-id="3d322-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3d322-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d322-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d322-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3d322-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d322-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3d322-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d322-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d322-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d322-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3d322-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d322-115">Application</span></span> | <span data-ttu-id="3d322-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d322-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="3d322-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d322-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="3d322-118">响应</span><span class="sxs-lookup"><span data-stu-id="3d322-118">Response</span></span>

<span data-ttu-id="3d322-119">返回 `302 Found` 响应，重定向到文件字节已预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="3d322-119">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="3d322-p103">若要下载该文件的内容，应用程序将需要遵循响应中的 `Location` 标头。许多 HTTP 客户端库将自动遵循 302 重定向并立即开始下载文件。</span><span class="sxs-lookup"><span data-stu-id="3d322-p103">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="3d322-122">预先验证的下载 URL 仅在较短的一段时间 （几分钟后）内有效，不需要 `Authorization` 标头即可下载。</span><span class="sxs-lookup"><span data-stu-id="3d322-122">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="3d322-123">示例</span><span class="sxs-lookup"><span data-stu-id="3d322-123">Example</span></span>

<span data-ttu-id="3d322-124">本示例检索当前用户驱动器中的文件版本。</span><span class="sxs-lookup"><span data-stu-id="3d322-124">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="request"></a><span data-ttu-id="3d322-125">请求</span><span class="sxs-lookup"><span data-stu-id="3d322-125">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3d322-126">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3d322-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3d322-127">C#</span><span class="sxs-lookup"><span data-stu-id="3d322-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-version-contents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d322-128">Javascript</span><span class="sxs-lookup"><span data-stu-id="3d322-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-version-contents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3d322-129">目标-C</span><span class="sxs-lookup"><span data-stu-id="3d322-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-version-contents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3d322-130">Java</span><span class="sxs-lookup"><span data-stu-id="3d322-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-version-contents-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3d322-131">响应</span><span class="sxs-lookup"><span data-stu-id="3d322-131">Response</span></span>

<span data-ttu-id="3d322-132">会返回一个重定向链接，可以在其中下载版本的内容。</span><span class="sxs-lookup"><span data-stu-id="3d322-132">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Redirect
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="3d322-133">注解</span><span class="sxs-lookup"><span data-stu-id="3d322-133">Remarks</span></span>

<span data-ttu-id="3d322-134">OneDrive 不保留文件以前版本的完整元数据。</span><span class="sxs-lookup"><span data-stu-id="3d322-134">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="3d322-135">当您的应用程序检索文件的可用版本列表时, 将返回[driveItemVersion](../resources/driveitemversion.md)资源, 它提供有关特定版本的可用信息。</span><span class="sxs-lookup"><span data-stu-id="3d322-135">When your app retrieves the list of available versions for a file, a [driveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
}
-->
