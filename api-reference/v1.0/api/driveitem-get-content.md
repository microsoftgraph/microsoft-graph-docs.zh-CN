---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 下载文件
localization_priority: Priority
ms.prod: sharepoint
description: 下载 DriveItem 的主要流（文件）的内容。 只能下载具有 file 属性的 driveItem。
doc_type: apiPageType
ms.openlocfilehash: 97ea17f8cfe6ac8230d91cc6e4ac6995b3512e90
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015486"
---
# <a name="download-the-contents-of-a-driveitem"></a><span data-ttu-id="580e5-104">下载 DriveItem 的内容</span><span class="sxs-lookup"><span data-stu-id="580e5-104">Download the contents of a DriveItem</span></span>

<span data-ttu-id="580e5-105">下载 DriveItem 的主要流（文件）的内容。</span><span class="sxs-lookup"><span data-stu-id="580e5-105">Download the contents of the primary stream (file) of a DriveItem.</span></span> <span data-ttu-id="580e5-106">只能下载具有 **file** 属性的 driveItem。</span><span class="sxs-lookup"><span data-stu-id="580e5-106">Only driveItems with the **file** property can be downloaded.</span></span>

## <a name="permissions"></a><span data-ttu-id="580e5-107">权限</span><span class="sxs-lookup"><span data-stu-id="580e5-107">Permissions</span></span>

<span data-ttu-id="580e5-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="580e5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="580e5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="580e5-110">Permission type</span></span>      | <span data-ttu-id="580e5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="580e5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="580e5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="580e5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="580e5-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="580e5-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="580e5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="580e5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="580e5-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="580e5-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="580e5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="580e5-116">Application</span></span> | <span data-ttu-id="580e5-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="580e5-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="580e5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="580e5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/content
GET /groups/{group-id}/drive/items/{item-id}/content
GET /me/drive/root:/{item-path}:/content
GET /me/drive/items/{item-id}/content
GET /sites/{siteId}/drive/items/{item-id}/content
GET /users/{userId}/drive/items/{item-id}/content
```

## <a name="optional-request-headers"></a><span data-ttu-id="580e5-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="580e5-119">Optional request headers</span></span>

| <span data-ttu-id="580e5-120">名称</span><span class="sxs-lookup"><span data-stu-id="580e5-120">Name</span></span>          | <span data-ttu-id="580e5-121">值</span><span class="sxs-lookup"><span data-stu-id="580e5-121">Value</span></span>  | <span data-ttu-id="580e5-122">说明</span><span class="sxs-lookup"><span data-stu-id="580e5-122">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="580e5-123">if-none-match</span><span class="sxs-lookup"><span data-stu-id="580e5-123">if-none-match</span></span> | <span data-ttu-id="580e5-124">String</span><span class="sxs-lookup"><span data-stu-id="580e5-124">String</span></span> | <span data-ttu-id="580e5-125">如果包含此请求标头，且提供的 eTag（或 cTag）与文件中的当前标记不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="580e5-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="580e5-126">示例</span><span class="sxs-lookup"><span data-stu-id="580e5-126">Example</span></span>

<span data-ttu-id="580e5-127">下面是下载整个文件的示例。</span><span class="sxs-lookup"><span data-stu-id="580e5-127">Here is an example to download a complete file.</span></span>



# <a name="httptabhttp"></a>[<span data-ttu-id="580e5-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="580e5-128">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "download-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="580e5-129">C#</span><span class="sxs-lookup"><span data-stu-id="580e5-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/download-item-content-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="580e5-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="580e5-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/download-item-content-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="580e5-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="580e5-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/download-item-content-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="580e5-132">Java</span><span class="sxs-lookup"><span data-stu-id="580e5-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/download-item-content-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="580e5-133">响应</span><span class="sxs-lookup"><span data-stu-id="580e5-133">Response</span></span>

<span data-ttu-id="580e5-p104">返回 `302 Found` 响应，该响应重定向到文件的预先身份验证的下载 URL。这是可通过 DriveItem 上的 `@microsoft.graph.downloadUrl` 属性获得的同一个 URL。</span><span class="sxs-lookup"><span data-stu-id="580e5-p104">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the file. This is the same URL available through the `@microsoft.graph.downloadUrl` property on the DriveItem.</span></span>

<span data-ttu-id="580e5-136">应用必须遵循响应中的 `Location` 头，才能下载文件内容。</span><span class="sxs-lookup"><span data-stu-id="580e5-136">To download the contents of the file your application will need to follow the `Location` header in the response.</span></span>
<span data-ttu-id="580e5-137">许多 HTTP 客户端库将自动遵循 302 重定向并立即开始下载文件。</span><span class="sxs-lookup"><span data-stu-id="580e5-137">Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immediately.</span></span>

<span data-ttu-id="580e5-138">预先身份验证的下载 URL 仅在较短的一段时间 （几分钟后）内有效，不需要 `Authorization` 标头即可下载。</span><span class="sxs-lookup"><span data-stu-id="580e5-138">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

## <a name="partial-range-downloads"></a><span data-ttu-id="580e5-139">部分范围下载</span><span class="sxs-lookup"><span data-stu-id="580e5-139">Partial range downloads</span></span>

<span data-ttu-id="580e5-p106">若要从文件中下载部分范围的字节，应用程序可以使用 [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt) 中指定的 `Range` 标头。请注意，必须将 `Range` 标头附加到实际 `@microsoft.graph.downloadUrl` URL，而不是 `/content` 的请求。</span><span class="sxs-lookup"><span data-stu-id="580e5-p106">To download a partial range of bytes from the file, your app can use the `Range` header as specified in [RFC 2616](https://www.ietf.org/rfc/rfc2616.txt). Note that you must append the `Range` header to the actual `@microsoft.graph.downloadUrl` URL and not to the request for `/content`.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "download-item-partial", "scopes": "files.read" } -->

```http
GET https://b0mpua-by3301.files.1drv.com/y23vmag
Range: bytes=0-1023
```

<span data-ttu-id="580e5-p107">此方法将返回 `HTTP 206 Partial Content` 响应和文件中字节的请求区域。如果无法生成此范围，可能会忽略 Range 标头，并会返回包含文件完整内容的 `HTTP 200` 响应。</span><span class="sxs-lookup"><span data-stu-id="580e5-p107">This will return an `HTTP 206 Partial Content` response with the request range of bytes from the file. If the range cannot be generated the Range header may be ignored and an `HTTP 200` response would be returned with the full contents of the file.</span></span>

<!-- { "blockType": "response", "name": "download-item-partial", "@odata.type": "stream" } -->

```http
HTTP/1.1 206 Partial Content
Content-Range: bytes 0-1023/2048
Content-Type: application/octet-stream

<first 1024 bytes of file>
```

### <a name="error-responses"></a><span data-ttu-id="580e5-144">错误响应</span><span class="sxs-lookup"><span data-stu-id="580e5-144">Error responses</span></span>

<span data-ttu-id="580e5-145">请参阅[错误响应][error-response]，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="580e5-145">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Download the contents of a DriveItem.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Items/Download",
  "suppressions": [
  ]
} -->
