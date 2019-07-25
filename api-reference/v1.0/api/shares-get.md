---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 访问共享项目
localization_priority: Normal
ms.openlocfilehash: 887567bc780c65b88989d8df79fdaec0f7b4c676
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891634"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="c05bc-102">访问共享 DriveItem</span><span class="sxs-lookup"><span data-stu-id="c05bc-102">Accessing shared DriveItems</span></span>

<span data-ttu-id="c05bc-103">通过使用 **shareId** 或共享 URL 访问共享 [DriveItem](../resources/driveitem.md) 或共享项目集合。</span><span class="sxs-lookup"><span data-stu-id="c05bc-103">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="c05bc-104">要与此 API 一起使用共享 URL，应用需要[将此 URL 转换为共享令牌](#encoding-sharing-urls)。</span><span class="sxs-lookup"><span data-stu-id="c05bc-104">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="c05bc-105">权限</span><span class="sxs-lookup"><span data-stu-id="c05bc-105">Permissions</span></span>

<span data-ttu-id="c05bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c05bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c05bc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c05bc-108">Permission type</span></span>      | <span data-ttu-id="c05bc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c05bc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c05bc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c05bc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c05bc-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c05bc-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c05bc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c05bc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c05bc-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c05bc-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c05bc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c05bc-114">Application</span></span> | <span data-ttu-id="c05bc-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c05bc-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c05bc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c05bc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="c05bc-117">路径参数</span><span class="sxs-lookup"><span data-stu-id="c05bc-117">Path parameters</span></span>

| <span data-ttu-id="c05bc-118">参数名称</span><span class="sxs-lookup"><span data-stu-id="c05bc-118">Parameter Name</span></span>                 | <span data-ttu-id="c05bc-119">值</span><span class="sxs-lookup"><span data-stu-id="c05bc-119">Value</span></span>    | <span data-ttu-id="c05bc-120">说明</span><span class="sxs-lookup"><span data-stu-id="c05bc-120">Description</span></span>                                                                         |
|:-------------------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="c05bc-121">**shareIdOrEncodedSharingUrl**</span><span class="sxs-lookup"><span data-stu-id="c05bc-121">**shareIdOrEncodedSharingUrl**</span></span> | `string` | <span data-ttu-id="c05bc-122">必需。</span><span class="sxs-lookup"><span data-stu-id="c05bc-122">Required.</span></span> <span data-ttu-id="c05bc-123">API 返回的共享令牌或正确编码的共享 URL。</span><span class="sxs-lookup"><span data-stu-id="c05bc-123">A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="c05bc-124">编码共享 URL</span><span class="sxs-lookup"><span data-stu-id="c05bc-124">Encoding sharing URLs</span></span>

<span data-ttu-id="c05bc-125">若要编码共享 URL，请使用以下逻辑：</span><span class="sxs-lookup"><span data-stu-id="c05bc-125">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="c05bc-126">首先，使用 base64 编码 URL。</span><span class="sxs-lookup"><span data-stu-id="c05bc-126">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="c05bc-127">删除值末尾的 [](https://en.wikipedia.org/wiki/Base64) 字符，将 `=` 替换成 `/`，将 `_` 替换成 `+`，从而将 base64 编码结果转换成`-`。</span><span class="sxs-lookup"><span data-stu-id="c05bc-127">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="c05bc-128">将 `u!` 追加到字符串的开头。</span><span class="sxs-lookup"><span data-stu-id="c05bc-128">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="c05bc-129">例如，若要对 URL 进行 C# 编码，请使用以下代码：</span><span class="sxs-lookup"><span data-stu-id="c05bc-129">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="optional-request-headers"></a><span data-ttu-id="c05bc-130">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="c05bc-130">Optional request headers</span></span>

| <span data-ttu-id="c05bc-131">名称</span><span class="sxs-lookup"><span data-stu-id="c05bc-131">Name</span></span>       | <span data-ttu-id="c05bc-132">类型</span><span class="sxs-lookup"><span data-stu-id="c05bc-132">Type</span></span>   | <span data-ttu-id="c05bc-133">说明</span><span class="sxs-lookup"><span data-stu-id="c05bc-133">Description</span></span>                                                    |
|:-----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="c05bc-134">**Prefer**</span><span class="sxs-lookup"><span data-stu-id="c05bc-134">**Prefer**</span></span> | <span data-ttu-id="c05bc-135">字符串</span><span class="sxs-lookup"><span data-stu-id="c05bc-135">string</span></span> | <span data-ttu-id="c05bc-136">可选。</span><span class="sxs-lookup"><span data-stu-id="c05bc-136">Optional.</span></span> <span data-ttu-id="c05bc-137">将设置为以下记录`prefer`的值之一。</span><span class="sxs-lookup"><span data-stu-id="c05bc-137">Set to one of the `prefer` values documented below.</span></span>  |

### <a name="prefer-header-values"></a><span data-ttu-id="c05bc-138">首选标头值</span><span class="sxs-lookup"><span data-stu-id="c05bc-138">Prefer header values</span></span>

| <span data-ttu-id="c05bc-139">名称</span><span class="sxs-lookup"><span data-stu-id="c05bc-139">Name</span></span>                          | <span data-ttu-id="c05bc-140">说明</span><span class="sxs-lookup"><span data-stu-id="c05bc-140">Description</span></span>                                                                                             |
|:------------------------------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c05bc-141">redeemSharingLink</span><span class="sxs-lookup"><span data-stu-id="c05bc-141">redeemSharingLink</span></span>             | <span data-ttu-id="c05bc-142">如果**shareIdOrEncodedSharingUrl**是共享链接, 则向呼叫者授予对项目的持久访问权限</span><span class="sxs-lookup"><span data-stu-id="c05bc-142">If the **shareIdOrEncodedSharingUrl** is a sharing link, grant the caller durable access to the item</span></span>    |
| <span data-ttu-id="c05bc-143">redeemSharingLinkIfNecessary</span><span class="sxs-lookup"><span data-stu-id="c05bc-143">redeemSharingLinkIfNecessary</span></span>  | <span data-ttu-id="c05bc-144">与 redeemSharingLink 相同, 但仅保证在此请求的持续时间内授予访问权限</span><span class="sxs-lookup"><span data-stu-id="c05bc-144">Same as redeemSharingLink, but access is only guaranteed to be granted for the duration of this request</span></span> |

<span data-ttu-id="c05bc-145">应将 redeemSharingLink 视为与调用者导航到共享链接的调用者导航到浏览器 (接受共享手势), 而 redeemSharingLinkIfNecessary 的目的是专门用于查看链接的metadata.</span><span class="sxs-lookup"><span data-stu-id="c05bc-145">redeemSharingLink should be considered equivalent to the caller navigating to the sharing link the browser (accepting the sharing gesture), whereas redeemSharingLinkIfNecessary is intended for scenarios where the intention is simply to peek at the link's metadata.</span></span>

## <a name="response"></a><span data-ttu-id="c05bc-146">响应</span><span class="sxs-lookup"><span data-stu-id="c05bc-146">Response</span></span>

<span data-ttu-id="c05bc-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [sharedDriveItem](../resources/shareddriveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="c05bc-147">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c05bc-148">示例</span><span class="sxs-lookup"><span data-stu-id="c05bc-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="c05bc-149">请求</span><span class="sxs-lookup"><span data-stu-id="c05bc-149">Request</span></span>

<span data-ttu-id="c05bc-150">下面是一个请求检索共享项目的示例：</span><span class="sxs-lookup"><span data-stu-id="c05bc-150">Here is an example of the request to retrieve a shared item:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c05bc-151">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c05bc-151">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c05bc-152">C#</span><span class="sxs-lookup"><span data-stu-id="c05bc-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c05bc-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="c05bc-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c05bc-154">目标-C</span><span class="sxs-lookup"><span data-stu-id="c05bc-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c05bc-155">Java</span><span class="sxs-lookup"><span data-stu-id="c05bc-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shared-root-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c05bc-156">响应</span><span class="sxs-lookup"><span data-stu-id="c05bc-156">Response</span></span>

<span data-ttu-id="c05bc-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c05bc-157">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.sharedDriveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "B64397C8-07AE-43E4-920E-32BFB4331A5B",
  "name": "contoso project.docx",
  "owner": {
    "user": {
      "id": "98E88F1C-F8DC-47CC-A406-C090248B30E5",
      "displayName": "Ryan Gregg"
    }
  }
}
```

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="c05bc-158">直接访问共享项目</span><span class="sxs-lookup"><span data-stu-id="c05bc-158">Access the shared item directly</span></span>

<span data-ttu-id="c05bc-p104">虽然 [**SharedDriveItem**](../resources/shareddriveitem.md) 包含一些有用的信息，但大多数应用程序都需要直接访问共享 [DriveItem](../resources/driveitem.md)。**SharedDriveItem** 资源包括**根**和**项目**关系，这些关系可以访问共享项目范围内的内容。</span><span class="sxs-lookup"><span data-stu-id="c05bc-p104">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="c05bc-161">示例（单个文件）</span><span class="sxs-lookup"><span data-stu-id="c05bc-161">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="c05bc-162">请求</span><span class="sxs-lookup"><span data-stu-id="c05bc-162">Request</span></span>

<span data-ttu-id="c05bc-163">通过请求 **driveItem** 关系，将返回共享的 **DriveItem**。</span><span class="sxs-lookup"><span data-stu-id="c05bc-163">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c05bc-164">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c05bc-164">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c05bc-165">C#</span><span class="sxs-lookup"><span data-stu-id="c05bc-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c05bc-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="c05bc-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c05bc-167">目标-C</span><span class="sxs-lookup"><span data-stu-id="c05bc-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c05bc-168">Java</span><span class="sxs-lookup"><span data-stu-id="c05bc-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shared-driveitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c05bc-169">响应</span><span class="sxs-lookup"><span data-stu-id="c05bc-169">Response</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

## <a name="example-shared-folder"></a><span data-ttu-id="c05bc-170">示例（共享文件夹）</span><span class="sxs-lookup"><span data-stu-id="c05bc-170">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="c05bc-171">请求</span><span class="sxs-lookup"><span data-stu-id="c05bc-171">Request</span></span>

<span data-ttu-id="c05bc-172">通过请求 **driveItem** 关系并展开**子**集合，将同时返回共享的 **DriveItem** 以及共享文件夹内的文件。</span><span class="sxs-lookup"><span data-stu-id="c05bc-172">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c05bc-173">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c05bc-173">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c05bc-174">C#</span><span class="sxs-lookup"><span data-stu-id="c05bc-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-expand-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c05bc-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="c05bc-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-expand-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c05bc-176">目标-C</span><span class="sxs-lookup"><span data-stu-id="c05bc-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-expand-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c05bc-177">Java</span><span class="sxs-lookup"><span data-stu-id="c05bc-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shared-driveitem-expand-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c05bc-178">响应</span><span class="sxs-lookup"><span data-stu-id="c05bc-178">Response</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {},
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <a name="error-responses"></a><span data-ttu-id="c05bc-179">错误响应</span><span class="sxs-lookup"><span data-stu-id="c05bc-179">Error Responses</span></span>

<span data-ttu-id="c05bc-180">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="c05bc-180">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="remarks"></a><span data-ttu-id="c05bc-181">注解</span><span class="sxs-lookup"><span data-stu-id="c05bc-181">Remarks</span></span>

* <span data-ttu-id="c05bc-182">对于 OneDrive for Business 和 SharePoint，共享 API 始终要求进行身份验证，无法用于在没有用户上下文的情况下访问匿名共享内容。</span><span class="sxs-lookup"><span data-stu-id="c05bc-182">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link",
  "suppressions": [
  ]
} -->
