---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 使用链接共享文件
ms.openlocfilehash: 85621a167d3ec3a8ecf9218ceca79367dade76e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046483"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="80c13-102">为 DriveItem 创建共享链接</span><span class="sxs-lookup"><span data-stu-id="80c13-102">Create a sharing link for a DriveItem</span></span>

> <span data-ttu-id="80c13-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="80c13-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80c13-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="80c13-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="80c13-105">可以使用 **createLink** 操作通过共享链接共享 [DriveItem](../resources/driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="80c13-105">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="80c13-p102">如果调用应用程序指定的链接类型尚不存在，**CreateLink** 操作将创建新的共享链接。如果应用程序指定的共享链接类型已存在，则返回现有的共享链接。</span><span class="sxs-lookup"><span data-stu-id="80c13-p102">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="80c13-108">DriveItem 资源从其上级继承共享权限。</span><span class="sxs-lookup"><span data-stu-id="80c13-108">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="80c13-109">权限</span><span class="sxs-lookup"><span data-stu-id="80c13-109">Permissions</span></span>

<span data-ttu-id="80c13-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80c13-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80c13-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="80c13-112">Permission type</span></span>      | <span data-ttu-id="80c13-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80c13-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80c13-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80c13-114">Delegated (work or school account)</span></span> | <span data-ttu-id="80c13-115">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80c13-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="80c13-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80c13-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80c13-117">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80c13-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="80c13-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="80c13-118">Application</span></span> | <span data-ttu-id="80c13-119">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80c13-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80c13-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80c13-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a><span data-ttu-id="80c13-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="80c13-121">Request body</span></span>

<span data-ttu-id="80c13-122">请求正文定义应用程序正在请求的共享链接的属性。</span><span class="sxs-lookup"><span data-stu-id="80c13-122">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="80c13-123">请求应为具有以下属性的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="80c13-123">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="80c13-124">名称</span><span class="sxs-lookup"><span data-stu-id="80c13-124">Name</span></span>    |  <span data-ttu-id="80c13-125">类型</span><span class="sxs-lookup"><span data-stu-id="80c13-125">Type</span></span>  |                                 <span data-ttu-id="80c13-126">说明</span><span class="sxs-lookup"><span data-stu-id="80c13-126">Description</span></span>                                  |
| :-------- | :----- | :--------------------------------------------------------------------------- |
| <span data-ttu-id="80c13-127">**类型**</span><span class="sxs-lookup"><span data-stu-id="80c13-127">**type**</span></span>  | <span data-ttu-id="80c13-128">string</span><span class="sxs-lookup"><span data-stu-id="80c13-128">string</span></span> | <span data-ttu-id="80c13-p105">要创建的共享链接的类型。`view`、`edit` 或 `embed`。</span><span class="sxs-lookup"><span data-stu-id="80c13-p105">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="80c13-131">**scope**</span><span class="sxs-lookup"><span data-stu-id="80c13-131">**scope**</span></span> | <span data-ttu-id="80c13-132">string</span><span class="sxs-lookup"><span data-stu-id="80c13-132">string</span></span> | <span data-ttu-id="80c13-133">可选。</span><span class="sxs-lookup"><span data-stu-id="80c13-133">Optional.</span></span> <span data-ttu-id="80c13-134">要创建的链接的范围。</span><span class="sxs-lookup"><span data-stu-id="80c13-134">The scope of link to create.</span></span> <span data-ttu-id="80c13-135">`anonymous` 或 `organization`。</span><span class="sxs-lookup"><span data-stu-id="80c13-135">Either `anonymous` or `organization`.</span></span> |


### <a name="link-types"></a><span data-ttu-id="80c13-136">链接类型</span><span class="sxs-lookup"><span data-stu-id="80c13-136">Link types</span></span>

<span data-ttu-id="80c13-137">**type** 参数允许使用以下值：</span><span class="sxs-lookup"><span data-stu-id="80c13-137">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="80c13-138">类型值</span><span class="sxs-lookup"><span data-stu-id="80c13-138">Type value</span></span> | <span data-ttu-id="80c13-139">说明</span><span class="sxs-lookup"><span data-stu-id="80c13-139">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="80c13-140">创建到 DriveItem 的只读链接。</span><span class="sxs-lookup"><span data-stu-id="80c13-140">Creates a read-only link to the DriveItem.</span></span>                                                        |
| `edit`     | <span data-ttu-id="80c13-141">创建到 DriveItem 的读写链接。</span><span class="sxs-lookup"><span data-stu-id="80c13-141">Creates a read-write link to the DriveItem.</span></span>                                                       |
| `embed`    | <span data-ttu-id="80c13-142">创建到 DriveItem 的可嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="80c13-142">Creates an embeddable link to the DriveItem.</span></span> <span data-ttu-id="80c13-143">此选项仅适用于 OneDrive 个人版中的文件。</span><span class="sxs-lookup"><span data-stu-id="80c13-143">This option is only available for files in OneDrive personal.</span></span> |

### <a name="scope-types"></a><span data-ttu-id="80c13-144">范围类型</span><span class="sxs-lookup"><span data-stu-id="80c13-144">Scope types</span></span>

<span data-ttu-id="80c13-145">**scope** 参数允许使用以下值。</span><span class="sxs-lookup"><span data-stu-id="80c13-145">The following values are allowed for the **scope** parameter.</span></span>
<span data-ttu-id="80c13-146">如果未指定 **scope** 参数，则为组织创建默认的链接类型。</span><span class="sxs-lookup"><span data-stu-id="80c13-146">If the **scope** parameter is not specified, the default link type for the organization is created.</span></span>

| <span data-ttu-id="80c13-147">类型值</span><span class="sxs-lookup"><span data-stu-id="80c13-147">Type value</span></span>     | <span data-ttu-id="80c13-148">说明</span><span class="sxs-lookup"><span data-stu-id="80c13-148">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="80c13-149">创建到任意用户都可使用链接访问的 DriveItem 的链接。</span><span class="sxs-lookup"><span data-stu-id="80c13-149">Creates a link to the DriveItem accessible to anyone with the link.</span></span> <span data-ttu-id="80c13-150">管理员可能会禁用匿名链接。</span><span class="sxs-lookup"><span data-stu-id="80c13-150">Anonymous links may be disabled by an administrator.</span></span>                 |
| `organization` | <span data-ttu-id="80c13-151">创建到用户组织内任意用户都可访问的 DriveItem 的链接。</span><span class="sxs-lookup"><span data-stu-id="80c13-151">Creates a link to the DriveItem accessible to anyone within the user's organization.</span></span> <span data-ttu-id="80c13-152">OneDrive 个人版不支持组织链接范围。</span><span class="sxs-lookup"><span data-stu-id="80c13-152">Organization link scope is not available for OneDrive personal.</span></span> |

## <a name="response"></a><span data-ttu-id="80c13-153">响应</span><span class="sxs-lookup"><span data-stu-id="80c13-153">Response</span></span>

<span data-ttu-id="80c13-154">如果成功，此方法将在响应正文中返回单个 [Permission](../resources/permission.md) 资源，此响应正文表示请求的共享权限。</span><span class="sxs-lookup"><span data-stu-id="80c13-154">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="80c13-155">如果已经为此项目创建新的共享链接，则响应为 `201 Created`；如果返回现有链接，则为 `200 OK`。</span><span class="sxs-lookup"><span data-stu-id="80c13-155">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="80c13-156">示例</span><span class="sxs-lookup"><span data-stu-id="80c13-156">Example</span></span>

<span data-ttu-id="80c13-157">下面的示例请求为在用户的 OneDrive 中按 {itemId} 指定的 DriveItem 创建共享链接。</span><span class="sxs-lookup"><span data-stu-id="80c13-157">The following example requests a sharing link to be created for the DriveItem specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="80c13-158">共享链接配置为只读并且可由具有该链接的任何用户使用。</span><span class="sxs-lookup"><span data-stu-id="80c13-158">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

### <a name="request"></a><span data-ttu-id="80c13-159">请求</span><span class="sxs-lookup"><span data-stu-id="80c13-159">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

### <a name="response"></a><span data-ttu-id="80c13-160">响应</span><span class="sxs-lookup"><span data-stu-id="80c13-160">Response</span></span>

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

## <a name="creating-company-sharable-links"></a><span data-ttu-id="80c13-161">创建公司可共享的链接</span><span class="sxs-lookup"><span data-stu-id="80c13-161">Creating company sharable links</span></span>

<span data-ttu-id="80c13-162">OneDrive for Business 和 SharePoint 都支持公司可共享的链接。</span><span class="sxs-lookup"><span data-stu-id="80c13-162">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="80c13-163">此类链接与匿名链接类似，只不过仅适用于拥有组织的成员。</span><span class="sxs-lookup"><span data-stu-id="80c13-163">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="80c13-164">若要创建公司可共享的链接，请使用值为 `organization` 的 **scope** 参数。</span><span class="sxs-lookup"><span data-stu-id="80c13-164">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

### <a name="request"></a><span data-ttu-id="80c13-165">请求</span><span class="sxs-lookup"><span data-stu-id="80c13-165">Request</span></span>

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

### <a name="response"></a><span data-ttu-id="80c13-166">响应</span><span class="sxs-lookup"><span data-stu-id="80c13-166">Response</span></span>

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

## <a name="creating-embeddable-links"></a><span data-ttu-id="80c13-167">创建可嵌入的链接</span><span class="sxs-lookup"><span data-stu-id="80c13-167">Creating embeddable links</span></span>

<span data-ttu-id="80c13-p113">使用 `embed` 链接类型时，可以在 `<iframe>` HTML 元素中嵌入返回的 webUrl。创建嵌入链接时，`webHtml` 属性包含 `<iframe>` 的 HTML 代码以托管内容。</span><span class="sxs-lookup"><span data-stu-id="80c13-p113">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="80c13-170">**注意：** 仅 OneDrive 个人版支持嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="80c13-170">**Note:** Embed links are only supported for OneDrive personal.</span></span>

### <a name="request"></a><span data-ttu-id="80c13-171">请求</span><span class="sxs-lookup"><span data-stu-id="80c13-171">Request</span></span>

<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite service.onedrive" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

### <a name="response"></a><span data-ttu-id="80c13-172">响应</span><span class="sxs-lookup"><span data-stu-id="80c13-172">Response</span></span>

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
    "webUrl": "https://onedive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a><span data-ttu-id="80c13-173">注解</span><span class="sxs-lookup"><span data-stu-id="80c13-173">Remarks</span></span>

* <span data-ttu-id="80c13-174">使用此操作创建的链接不会过期，除非对组织强制执行了默认过期策略。</span><span class="sxs-lookup"><span data-stu-id="80c13-174">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="80c13-175">链接在项的共享权限中可见，可以由该项的所有者删除。</span><span class="sxs-lookup"><span data-stu-id="80c13-175">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="80c13-176">除非项已被签出，否则链接始终指向该项的最新版本（仅限 SharePoint）。</span><span class="sxs-lookup"><span data-stu-id="80c13-176">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link"
} -->
