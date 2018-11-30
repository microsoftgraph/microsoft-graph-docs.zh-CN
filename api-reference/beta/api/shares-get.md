---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 访问共享项目
ms.openlocfilehash: d3f6ef956501cded8af9ed641b2bb37666174cef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045006"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="ca6d5-102">访问共享 DriveItem</span><span class="sxs-lookup"><span data-stu-id="ca6d5-102">Accessing shared DriveItems</span></span>

<span data-ttu-id="ca6d5-103">通过使用 **shareId** 或共享 URL 访问共享 [DriveItem](../resources/driveitem.md) 或共享项目集合。</span><span class="sxs-lookup"><span data-stu-id="ca6d5-103">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="ca6d5-104">要与此 API 一起使用共享 URL，应用需要[将此 URL 转换为共享令牌](#encoding-sharing-urls)。</span><span class="sxs-lookup"><span data-stu-id="ca6d5-104">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca6d5-105">权限</span><span class="sxs-lookup"><span data-stu-id="ca6d5-105">Permissions</span></span>

<span data-ttu-id="ca6d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca6d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca6d5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca6d5-108">Permission type</span></span>      | <span data-ttu-id="ca6d5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca6d5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca6d5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca6d5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ca6d5-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca6d5-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ca6d5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca6d5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca6d5-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca6d5-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ca6d5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca6d5-114">Application</span></span> | <span data-ttu-id="ca6d5-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca6d5-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca6d5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca6d5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="ca6d5-117">路径参数</span><span class="sxs-lookup"><span data-stu-id="ca6d5-117">Path Parameters</span></span>

| <span data-ttu-id="ca6d5-118">参数名称</span><span class="sxs-lookup"><span data-stu-id="ca6d5-118">Parameter Name</span></span>        | <span data-ttu-id="ca6d5-119">值</span><span class="sxs-lookup"><span data-stu-id="ca6d5-119">Value</span></span>    | <span data-ttu-id="ca6d5-120">说明</span><span class="sxs-lookup"><span data-stu-id="ca6d5-120">Description</span></span>                                                                         |
|:----------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="ca6d5-121">**sharingTokenOrUrl**</span><span class="sxs-lookup"><span data-stu-id="ca6d5-121">**sharingTokenOrUrl**</span></span> | `string` | <span data-ttu-id="ca6d5-122">必需。</span><span class="sxs-lookup"><span data-stu-id="ca6d5-122">Required.</span></span> <span data-ttu-id="ca6d5-123">API 返回的共享令牌或正确编码的共享 URL。</span><span class="sxs-lookup"><span data-stu-id="ca6d5-123">A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="ca6d5-124">编码共享 URL</span><span class="sxs-lookup"><span data-stu-id="ca6d5-124">Encoding sharing URLs</span></span>

<span data-ttu-id="ca6d5-125">若要编码共享 URL，请使用以下逻辑：</span><span class="sxs-lookup"><span data-stu-id="ca6d5-125">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="ca6d5-126">首先，使用 base64 编码 URL。</span><span class="sxs-lookup"><span data-stu-id="ca6d5-126">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="ca6d5-127">删除值末尾的 `=` 字符，将 `/` 替换成 `_`，将 `+` 替换成 `-`，从而将 base64 编码结果转换成[未填充的 base64url 格式](https://en.wikipedia.org/wiki/Base64)。</span><span class="sxs-lookup"><span data-stu-id="ca6d5-127">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="ca6d5-128">将 `u!` 追加到字符串的开头。</span><span class="sxs-lookup"><span data-stu-id="ca6d5-128">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="ca6d5-129">例如，若要对 URL 进行 C# 编码，请使用以下代码：</span><span class="sxs-lookup"><span data-stu-id="ca6d5-129">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="response"></a><span data-ttu-id="ca6d5-130">响应</span><span class="sxs-lookup"><span data-stu-id="ca6d5-130">Response</span></span>

<span data-ttu-id="ca6d5-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [sharedDriveItem](../resources/shareddriveitem.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="ca6d5-131">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca6d5-132">示例</span><span class="sxs-lookup"><span data-stu-id="ca6d5-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca6d5-133">请求</span><span class="sxs-lookup"><span data-stu-id="ca6d5-133">Request</span></span>

<span data-ttu-id="ca6d5-134">下面是一个请求检索共享项目的示例：</span><span class="sxs-lookup"><span data-stu-id="ca6d5-134">Here is an example of the request to retrieve a shared item:</span></span>

<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET https://graph.microsoft.com/beta/shares/{shareIdOrEncodedSharingUrl}
```

### <a name="response"></a><span data-ttu-id="ca6d5-135">响应</span><span class="sxs-lookup"><span data-stu-id="ca6d5-135">Response</span></span>

<span data-ttu-id="ca6d5-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ca6d5-136">Here is an example of the response.</span></span>

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
  },
  "remoteItem": { 
    "driveId": "",
    "id": ""
  }
}
```

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="ca6d5-137">直接访问共享项目</span><span class="sxs-lookup"><span data-stu-id="ca6d5-137">Access the shared item directly</span></span>

<span data-ttu-id="ca6d5-p103">虽然 [**SharedDriveItem**](../resources/shareddriveitem.md) 包含一些有用的信息，但大多数应用程序都需要直接访问共享 [DriveItem](../resources/driveitem.md)。**SharedDriveItem** 资源包括**根**和**项目**关系，这些关系可以访问共享项目范围内的内容。</span><span class="sxs-lookup"><span data-stu-id="ca6d5-p103">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="ca6d5-140">示例（单个文件）</span><span class="sxs-lookup"><span data-stu-id="ca6d5-140">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="ca6d5-141">请求</span><span class="sxs-lookup"><span data-stu-id="ca6d5-141">Request</span></span>

<span data-ttu-id="ca6d5-142">通过请求 **driveItem** 关系，将返回共享的 **DriveItem**。</span><span class="sxs-lookup"><span data-stu-id="ca6d5-142">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```

### <a name="response"></a><span data-ttu-id="ca6d5-143">响应</span><span class="sxs-lookup"><span data-stu-id="ca6d5-143">Response</span></span>

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

## <a name="example-shared-folder"></a><span data-ttu-id="ca6d5-144">示例（共享文件夹）</span><span class="sxs-lookup"><span data-stu-id="ca6d5-144">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="ca6d5-145">请求</span><span class="sxs-lookup"><span data-stu-id="ca6d5-145">Request</span></span>

<span data-ttu-id="ca6d5-146">通过请求 **driveItem** 关系并展开**子**集合，将同时返回共享的 **DriveItem** 以及共享文件夹内的文件。</span><span class="sxs-lookup"><span data-stu-id="ca6d5-146">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET https://graph.microsoft.com/beta/shares/{shareIdOrUrl}/driveItem?$expand=children
```

### <a name="response"></a><span data-ttu-id="ca6d5-147">响应</span><span class="sxs-lookup"><span data-stu-id="ca6d5-147">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="ca6d5-148">注解</span><span class="sxs-lookup"><span data-stu-id="ca6d5-148">Remarks</span></span>

* <span data-ttu-id="ca6d5-149">对于 OneDrive for Business 和 SharePoint，共享 API 始终要求进行身份验证，无法用于在没有用户上下文的情况下访问匿名共享内容。</span><span class="sxs-lookup"><span data-stu-id="ca6d5-149">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link"
} -->
