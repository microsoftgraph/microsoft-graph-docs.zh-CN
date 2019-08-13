---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 使用链接共享文件
localization_priority: Normal
ms.prod: sharepoint
description: 可以使用 createLink 操作通过共享链接共享 DriveItem。
doc_type: apiPageType
ms.openlocfilehash: 9f203a590b0ca24ee0980854edd1f08752c90193
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365011"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="b7cc0-103">为 DriveItem 创建共享链接</span><span class="sxs-lookup"><span data-stu-id="b7cc0-103">Create a sharing link for a DriveItem</span></span>

<span data-ttu-id="b7cc0-104">可以使用 **createLink** 操作通过共享链接共享 [DriveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-104">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="b7cc0-p101">如果调用应用程序指定的链接类型尚不存在，**CreateLink** 操作将创建新的共享链接。如果应用程序指定的共享链接类型已存在，则返回现有的共享链接。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="b7cc0-107">DriveItem 资源从其上级继承共享权限。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-107">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7cc0-108">权限</span><span class="sxs-lookup"><span data-stu-id="b7cc0-108">Permissions</span></span>

<span data-ttu-id="b7cc0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7cc0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7cc0-111">Permission type</span></span>      | <span data-ttu-id="b7cc0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7cc0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7cc0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7cc0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b7cc0-114">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7cc0-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b7cc0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7cc0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7cc0-116">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7cc0-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b7cc0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7cc0-117">Application</span></span> | <span data-ttu-id="b7cc0-118">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7cc0-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7cc0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7cc0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a><span data-ttu-id="b7cc0-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7cc0-120">Request body</span></span>

<span data-ttu-id="b7cc0-121">请求正文定义应用程序正在请求的共享链接的属性。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-121">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="b7cc0-122">请求应为具有以下属性的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="b7cc0-123">名称</span><span class="sxs-lookup"><span data-stu-id="b7cc0-123">Name</span></span>    |  <span data-ttu-id="b7cc0-124">类型</span><span class="sxs-lookup"><span data-stu-id="b7cc0-124">Type</span></span>  |                                 <span data-ttu-id="b7cc0-125">说明</span><span class="sxs-lookup"><span data-stu-id="b7cc0-125">Description</span></span>                                  |
| :-------- | :----- | :--------------------------------------------------------------------------- |
| <span data-ttu-id="b7cc0-126">**类型**</span><span class="sxs-lookup"><span data-stu-id="b7cc0-126">**type**</span></span>  | <span data-ttu-id="b7cc0-127">string</span><span class="sxs-lookup"><span data-stu-id="b7cc0-127">string</span></span> | <span data-ttu-id="b7cc0-p104">要创建的共享链接的类型。`view`、`edit` 或 `embed`。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-p104">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="b7cc0-130">**scope**</span><span class="sxs-lookup"><span data-stu-id="b7cc0-130">**scope**</span></span> | <span data-ttu-id="b7cc0-131">字符串</span><span class="sxs-lookup"><span data-stu-id="b7cc0-131">string</span></span> | <span data-ttu-id="b7cc0-132">可选。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-132">Optional.</span></span> <span data-ttu-id="b7cc0-133">要创建的链接的范围。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-133">The scope of link to create.</span></span> <span data-ttu-id="b7cc0-134">`anonymous` 或 `organization`。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-134">Either `anonymous` or `organization`.</span></span> |


### <a name="link-types"></a><span data-ttu-id="b7cc0-135">链接类型</span><span class="sxs-lookup"><span data-stu-id="b7cc0-135">Link types</span></span>

<span data-ttu-id="b7cc0-136">**type** 参数允许使用以下值：</span><span class="sxs-lookup"><span data-stu-id="b7cc0-136">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="b7cc0-137">类型值</span><span class="sxs-lookup"><span data-stu-id="b7cc0-137">Type value</span></span> | <span data-ttu-id="b7cc0-138">说明</span><span class="sxs-lookup"><span data-stu-id="b7cc0-138">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="b7cc0-139">创建到 DriveItem 的只读链接。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-139">Creates a read-only link to the DriveItem.</span></span>                                                        |
| `edit`     | <span data-ttu-id="b7cc0-140">创建到 DriveItem 的读写链接。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-140">Creates a read-write link to the DriveItem.</span></span>                                                       |
| `embed`    | <span data-ttu-id="b7cc0-141">创建到 DriveItem 的可嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-141">Creates an embeddable link to the DriveItem.</span></span> <span data-ttu-id="b7cc0-142">此选项仅适用于 OneDrive 个人版中的文件。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-142">This option is only available for files in OneDrive personal.</span></span> |

### <a name="scope-types"></a><span data-ttu-id="b7cc0-143">范围类型</span><span class="sxs-lookup"><span data-stu-id="b7cc0-143">Scope types</span></span>

<span data-ttu-id="b7cc0-144">**scope** 参数允许使用以下值。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-144">The following values are allowed for the **scope** parameter.</span></span>
<span data-ttu-id="b7cc0-145">如果未指定 **scope** 参数，则为组织创建默认的链接类型。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-145">If the **scope** parameter is not specified, the default link type for the organization is created.</span></span>

| <span data-ttu-id="b7cc0-146">值</span><span class="sxs-lookup"><span data-stu-id="b7cc0-146">Value</span></span>          | <span data-ttu-id="b7cc0-147">说明</span><span class="sxs-lookup"><span data-stu-id="b7cc0-147">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="b7cc0-148">拥有该链接的任何人都可以访问, 而无需登录。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-148">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="b7cc0-149">这可能包括组织外部的人员。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-149">This may include people outside of your organization.</span></span> <span data-ttu-id="b7cc0-150">管理员可能禁用了匿名链接支持。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-150">Anonymous link support may be disabled by an administrator.</span></span>
| `organization` | <span data-ttu-id="b7cc0-151">登录到组织 (租户) 的任何人都可以使用链接获取访问权限。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-151">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="b7cc0-152">仅在 OneDrive for Business 和 SharePoint 中可用。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-152">Only available in OneDrive for Business and SharePoint.</span></span>


## <a name="response"></a><span data-ttu-id="b7cc0-153">响应</span><span class="sxs-lookup"><span data-stu-id="b7cc0-153">Response</span></span>

<span data-ttu-id="b7cc0-154">如果成功，此方法将在响应正文中返回单个 [Permission](../resources/permission.md) 资源，此响应正文表示请求的共享权限。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-154">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="b7cc0-155">如果已经为此项目创建新的共享链接，则响应为 `201 Created`；如果返回现有链接，则为 `200 OK`。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-155">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="b7cc0-156">示例</span><span class="sxs-lookup"><span data-stu-id="b7cc0-156">Example</span></span>

<span data-ttu-id="b7cc0-157">下面的示例请求为在用户的 OneDrive 中按 {itemId} 指定的 DriveItem 创建共享链接。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-157">The following example requests a sharing link to be created for the DriveItem specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="b7cc0-158">共享链接配置为只读并且可由具有该链接的任何用户使用。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-158">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

### <a name="request"></a><span data-ttu-id="b7cc0-159">请求</span><span class="sxs-lookup"><span data-stu-id="b7cc0-159">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b7cc0-160">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b7cc0-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-link"
}-->

```http
POST /me/drive/items/{item-id}/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b7cc0-161">C#</span><span class="sxs-lookup"><span data-stu-id="b7cc0-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b7cc0-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7cc0-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b7cc0-163">目标-C</span><span class="sxs-lookup"><span data-stu-id="b7cc0-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b7cc0-164">Java</span><span class="sxs-lookup"><span data-stu-id="b7cc0-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-link-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b7cc0-165">响应</span><span class="sxs-lookup"><span data-stu-id="b7cc0-165">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a><span data-ttu-id="b7cc0-166">创建公司可共享的链接</span><span class="sxs-lookup"><span data-stu-id="b7cc0-166">Creating company sharable links</span></span>

<span data-ttu-id="b7cc0-167">OneDrive for Business 和 SharePoint 都支持公司可共享的链接。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-167">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="b7cc0-168">此类链接与匿名链接类似，只不过仅适用于拥有组织的成员。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-168">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="b7cc0-169">若要创建公司可共享的链接，请使用值为 `organization` 的 **scope** 参数。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-169">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

### <a name="request"></a><span data-ttu-id="b7cc0-170">请求</span><span class="sxs-lookup"><span data-stu-id="b7cc0-170">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b7cc0-171">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b7cc0-171">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite", "tags": "service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b7cc0-172">C#</span><span class="sxs-lookup"><span data-stu-id="b7cc0-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-scoped-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b7cc0-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7cc0-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-scoped-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b7cc0-174">目标-C</span><span class="sxs-lookup"><span data-stu-id="b7cc0-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-scoped-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b7cc0-175">Java</span><span class="sxs-lookup"><span data-stu-id="b7cc0-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-link-scoped-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b7cc0-176">响应</span><span class="sxs-lookup"><span data-stu-id="b7cc0-176">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-embeddable-links"></a><span data-ttu-id="b7cc0-177">创建可嵌入的链接</span><span class="sxs-lookup"><span data-stu-id="b7cc0-177">Creating embeddable links</span></span>

<span data-ttu-id="b7cc0-p112">使用 `embed` 链接类型时，可以在 `<iframe>` HTML 元素中嵌入返回的 webUrl。创建嵌入链接时，`webHtml` 属性包含 `<iframe>` 的 HTML 代码以托管内容。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-p112">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="b7cc0-180">**注意：** 仅 OneDrive 个人版支持嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-180">**Note:** Embed links are only supported for OneDrive personal.</span></span>

### <a name="request"></a><span data-ttu-id="b7cc0-181">请求</span><span class="sxs-lookup"><span data-stu-id="b7cc0-181">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b7cc0-182">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b7cc0-182">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite", "tags": "service.onedrive service.graph" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b7cc0-183">C#</span><span class="sxs-lookup"><span data-stu-id="b7cc0-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-embedded-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b7cc0-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7cc0-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-embedded-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b7cc0-185">目标-C</span><span class="sxs-lookup"><span data-stu-id="b7cc0-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-embedded-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b7cc0-186">Java</span><span class="sxs-lookup"><span data-stu-id="b7cc0-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-embedded-link-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b7cc0-187">响应</span><span class="sxs-lookup"><span data-stu-id="b7cc0-187">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["read"],
  "link": {
    "type": "embed",
    "webHtml": "<IFRAME src=\"https://onedrive.live.com/...\"></IFRAME>",
    "webUrl": "https://onedrive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a><span data-ttu-id="b7cc0-188">注解</span><span class="sxs-lookup"><span data-stu-id="b7cc0-188">Remarks</span></span>

* <span data-ttu-id="b7cc0-189">使用此操作创建的链接不会过期，除非对组织强制执行了默认过期策略。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-189">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="b7cc0-190">链接在项的共享权限中可见，可以由该项的所有者删除。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-190">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="b7cc0-191">除非项已被签出，否则链接始终指向该项的最新版本（仅限 SharePoint）。</span><span class="sxs-lookup"><span data-stu-id="b7cc0-191">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
} -->
