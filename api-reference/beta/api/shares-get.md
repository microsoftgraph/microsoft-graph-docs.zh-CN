---
author: JeremyKelley
description: 通过使用 shareId 或共享 URL 访问共享 DriveItem 或共享项目集合。
ms.date: 09/10/2017
title: 访问共享项目
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 0cdb265ea8064e1bd13f0c131735911b010f312e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453308"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="d958d-103">访问共享 DriveItem</span><span class="sxs-lookup"><span data-stu-id="d958d-103">Accessing shared DriveItems</span></span>

<span data-ttu-id="d958d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d958d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d958d-105">通过使用 **shareId** 或共享 URL 访问共享 [DriveItem](../resources/driveitem.md) 或共享项目集合。</span><span class="sxs-lookup"><span data-stu-id="d958d-105">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="d958d-106">要与此 API 一起使用共享 URL，应用需要[将此 URL 转换为共享令牌](#encoding-sharing-urls)。</span><span class="sxs-lookup"><span data-stu-id="d958d-106">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="d958d-107">权限</span><span class="sxs-lookup"><span data-stu-id="d958d-107">Permissions</span></span>

<span data-ttu-id="d958d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d958d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d958d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d958d-110">Permission type</span></span>      | <span data-ttu-id="d958d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d958d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d958d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d958d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d958d-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d958d-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d958d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d958d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d958d-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d958d-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d958d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d958d-116">Application</span></span> | <span data-ttu-id="d958d-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d958d-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d958d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d958d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="d958d-119">路径参数</span><span class="sxs-lookup"><span data-stu-id="d958d-119">Path parameters</span></span>

| <span data-ttu-id="d958d-120">参数名称</span><span class="sxs-lookup"><span data-stu-id="d958d-120">Parameter Name</span></span>                 | <span data-ttu-id="d958d-121">值</span><span class="sxs-lookup"><span data-stu-id="d958d-121">Value</span></span>    | <span data-ttu-id="d958d-122">说明</span><span class="sxs-lookup"><span data-stu-id="d958d-122">Description</span></span>                                                                         |
|:-------------------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="d958d-123">**shareIdOrEncodedSharingUrl**</span><span class="sxs-lookup"><span data-stu-id="d958d-123">**shareIdOrEncodedSharingUrl**</span></span> | `string` | <span data-ttu-id="d958d-p102">必需。 API 返回的共享令牌或正确编码的共享 URL。</span><span class="sxs-lookup"><span data-stu-id="d958d-p102">Required. A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="d958d-126">编码共享 URL</span><span class="sxs-lookup"><span data-stu-id="d958d-126">Encoding sharing URLs</span></span>

<span data-ttu-id="d958d-127">若要编码共享 URL，请使用以下逻辑：</span><span class="sxs-lookup"><span data-stu-id="d958d-127">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="d958d-128">首先，使用 base64 编码 URL。</span><span class="sxs-lookup"><span data-stu-id="d958d-128">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="d958d-129">删除值末尾的 `=` 字符，将 `/` 替换成 `_`，将 `+` 替换成 `-`，从而将 base64 编码结果转换成[未填充的 base64url 格式](https://en.wikipedia.org/wiki/Base64)。</span><span class="sxs-lookup"><span data-stu-id="d958d-129">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="d958d-130">将 `u!` 追加到字符串的开头。</span><span class="sxs-lookup"><span data-stu-id="d958d-130">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="d958d-131">例如，若要对 URL 进行 C# 编码，请使用以下代码：</span><span class="sxs-lookup"><span data-stu-id="d958d-131">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="optional-request-headers"></a><span data-ttu-id="d958d-132">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="d958d-132">Optional request headers</span></span>

| <span data-ttu-id="d958d-133">名称</span><span class="sxs-lookup"><span data-stu-id="d958d-133">Name</span></span>       | <span data-ttu-id="d958d-134">类型</span><span class="sxs-lookup"><span data-stu-id="d958d-134">Type</span></span>   | <span data-ttu-id="d958d-135">说明</span><span class="sxs-lookup"><span data-stu-id="d958d-135">Description</span></span>                                                    |
|:-----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="d958d-136">**Prefer**</span><span class="sxs-lookup"><span data-stu-id="d958d-136">**Prefer**</span></span> | <span data-ttu-id="d958d-137">string</span><span class="sxs-lookup"><span data-stu-id="d958d-137">string</span></span> | <span data-ttu-id="d958d-138">可选。</span><span class="sxs-lookup"><span data-stu-id="d958d-138">Optional.</span></span> <span data-ttu-id="d958d-139">将设置为以下记录`prefer`的值之一。</span><span class="sxs-lookup"><span data-stu-id="d958d-139">Set to one of the `prefer` values documented below.</span></span>  |

### <a name="prefer-header-values"></a><span data-ttu-id="d958d-140">首选标头值</span><span class="sxs-lookup"><span data-stu-id="d958d-140">Prefer header values</span></span>

| <span data-ttu-id="d958d-141">名称</span><span class="sxs-lookup"><span data-stu-id="d958d-141">Name</span></span>                          | <span data-ttu-id="d958d-142">说明</span><span class="sxs-lookup"><span data-stu-id="d958d-142">Description</span></span>                                                                                             |
|:------------------------------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d958d-143">redeemSharingLink</span><span class="sxs-lookup"><span data-stu-id="d958d-143">redeemSharingLink</span></span>             | <span data-ttu-id="d958d-144">如果**shareIdOrEncodedSharingUrl**是共享链接，则向呼叫者授予对项目的持久访问权限</span><span class="sxs-lookup"><span data-stu-id="d958d-144">If the **shareIdOrEncodedSharingUrl** is a sharing link, grant the caller durable access to the item</span></span>    |
| <span data-ttu-id="d958d-145">redeemSharingLinkIfNecessary</span><span class="sxs-lookup"><span data-stu-id="d958d-145">redeemSharingLinkIfNecessary</span></span>  | <span data-ttu-id="d958d-146">与 redeemSharingLink 相同，但仅保证在此请求的持续时间内授予访问权限</span><span class="sxs-lookup"><span data-stu-id="d958d-146">Same as redeemSharingLink, but access is only guaranteed to be granted for the duration of this request</span></span> |

<span data-ttu-id="d958d-147">应将 redeemSharingLink 视为与调用者导航到共享链接的调用者导航到浏览器（接受共享手势），而 redeemSharingLinkIfNecessary 的目的是专门用于查看链接的metadata.</span><span class="sxs-lookup"><span data-stu-id="d958d-147">redeemSharingLink should be considered equivalent to the caller navigating to the sharing link the browser (accepting the sharing gesture), whereas redeemSharingLinkIfNecessary is intended for scenarios where the intention is simply to peek at the link's metadata.</span></span>

## <a name="response"></a><span data-ttu-id="d958d-148">响应</span><span class="sxs-lookup"><span data-stu-id="d958d-148">Response</span></span>

<span data-ttu-id="d958d-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [sharedDriveItem](../resources/shareddriveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="d958d-149">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d958d-150">示例</span><span class="sxs-lookup"><span data-stu-id="d958d-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="d958d-151">请求</span><span class="sxs-lookup"><span data-stu-id="d958d-151">Request</span></span>

<span data-ttu-id="d958d-152">下面是一个请求检索共享项目的示例：</span><span class="sxs-lookup"><span data-stu-id="d958d-152">Here is an example of the request to retrieve a shared item:</span></span>


# <a name="http"></a>[<span data-ttu-id="d958d-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="d958d-153">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-root" } -->

```msgraph-interactive
GET /shares/{shareIdOrEncodedSharingUrl}
```
# <a name="c"></a>[<span data-ttu-id="d958d-154">C#</span><span class="sxs-lookup"><span data-stu-id="d958d-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d958d-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d958d-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d958d-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d958d-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d958d-157">响应</span><span class="sxs-lookup"><span data-stu-id="d958d-157">Response</span></span>

<span data-ttu-id="d958d-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d958d-158">Here is an example of the response.</span></span>

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

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="d958d-159">直接访问共享项目</span><span class="sxs-lookup"><span data-stu-id="d958d-159">Access the shared item directly</span></span>

<span data-ttu-id="d958d-p104">虽然 [**SharedDriveItem**](../resources/shareddriveitem.md) 包含一些有用的信息，但大多数应用程序都需要直接访问共享 [DriveItem](../resources/driveitem.md)。**SharedDriveItem** 资源包括**根**和**项目**关系，这些关系可以访问共享项目范围内的内容。</span><span class="sxs-lookup"><span data-stu-id="d958d-p104">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="d958d-162">示例（单个文件）</span><span class="sxs-lookup"><span data-stu-id="d958d-162">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="d958d-163">请求</span><span class="sxs-lookup"><span data-stu-id="d958d-163">Request</span></span>

<span data-ttu-id="d958d-164">通过请求 **driveItem** 关系，将返回共享的 **DriveItem**。</span><span class="sxs-lookup"><span data-stu-id="d958d-164">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>


# <a name="http"></a>[<span data-ttu-id="d958d-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="d958d-165">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```msgraph-interactive
GET /shares/{shareIdOrUrl}/driveItem
```
# <a name="c"></a>[<span data-ttu-id="d958d-166">C#</span><span class="sxs-lookup"><span data-stu-id="d958d-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d958d-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d958d-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d958d-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d958d-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d958d-169">响应</span><span class="sxs-lookup"><span data-stu-id="d958d-169">Response</span></span>

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

## <a name="example-shared-folder"></a><span data-ttu-id="d958d-170">示例（共享文件夹）</span><span class="sxs-lookup"><span data-stu-id="d958d-170">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="d958d-171">请求</span><span class="sxs-lookup"><span data-stu-id="d958d-171">Request</span></span>

<span data-ttu-id="d958d-172">通过请求 **driveItem** 关系并展开**子**集合，将同时返回共享的 **DriveItem** 以及共享文件夹内的文件。</span><span class="sxs-lookup"><span data-stu-id="d958d-172">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>


# <a name="http"></a>[<span data-ttu-id="d958d-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="d958d-173">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```msgraph-interactive
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```
# <a name="c"></a>[<span data-ttu-id="d958d-174">C#</span><span class="sxs-lookup"><span data-stu-id="d958d-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-expand-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d958d-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d958d-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-expand-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d958d-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d958d-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-expand-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d958d-177">响应</span><span class="sxs-lookup"><span data-stu-id="d958d-177">Response</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="d958d-178">错误响应</span><span class="sxs-lookup"><span data-stu-id="d958d-178">Error Responses</span></span>

<span data-ttu-id="d958d-179">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="d958d-179">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="remarks"></a><span data-ttu-id="d958d-180">注解</span><span class="sxs-lookup"><span data-stu-id="d958d-180">Remarks</span></span>

* <span data-ttu-id="d958d-181">对于 OneDrive for Business 和 SharePoint，共享 API 始终要求进行身份验证，无法用于在没有用户上下文的情况下访问匿名共享内容。</span><span class="sxs-lookup"><span data-stu-id="d958d-181">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

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
