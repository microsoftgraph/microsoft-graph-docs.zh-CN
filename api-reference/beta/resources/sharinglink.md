---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
ms.openlocfilehash: 094de0cbdb77fe427ba70b9418ced5cc6e9cc731
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043131"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="c4655-102">sharingLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4655-102">sharingLink resource type</span></span>

> <span data-ttu-id="c4655-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c4655-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4655-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c4655-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4655-105">**SharingLink**资源组合到单个结构链接相关的数据项。</span><span class="sxs-lookup"><span data-stu-id="c4655-105">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="c4655-106">如果[**权限**](permission.md)资源有一个非空**sharingLink**方面，则权限表示共享链接 （而不是授予用户或用户组的权限）。</span><span class="sxs-lookup"><span data-stu-id="c4655-106">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4655-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4655-107">JSON representation</span></span>

<span data-ttu-id="c4655-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4655-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": { "@odata.type": "microsoft.graph.identity" },
  "preventsDownload": false,
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="c4655-109">属性</span><span class="sxs-lookup"><span data-stu-id="c4655-109">Properties</span></span>

| <span data-ttu-id="c4655-110">属性</span><span class="sxs-lookup"><span data-stu-id="c4655-110">Property</span></span>       | <span data-ttu-id="c4655-111">类型</span><span class="sxs-lookup"><span data-stu-id="c4655-111">Type</span></span>          | <span data-ttu-id="c4655-112">说明</span><span class="sxs-lookup"><span data-stu-id="c4655-112">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="c4655-113">application</span><span class="sxs-lookup"><span data-stu-id="c4655-113">application</span></span>    | <span data-ttu-id="c4655-114">[Identity][]</span><span class="sxs-lookup"><span data-stu-id="c4655-114">[identity][]</span></span>  | <span data-ttu-id="c4655-115">链接所关联的应用。</span><span class="sxs-lookup"><span data-stu-id="c4655-115">The app the link is associated with.</span></span>
| <span data-ttu-id="c4655-116">type</span><span class="sxs-lookup"><span data-stu-id="c4655-116">type</span></span>           | <span data-ttu-id="c4655-117">String</span><span class="sxs-lookup"><span data-stu-id="c4655-117">String</span></span>        | <span data-ttu-id="c4655-118">创建的链接类型。</span><span class="sxs-lookup"><span data-stu-id="c4655-118">The type of the link created.</span></span>
| <span data-ttu-id="c4655-119">scope</span><span class="sxs-lookup"><span data-stu-id="c4655-119">scope</span></span>          | <span data-ttu-id="c4655-120">String</span><span class="sxs-lookup"><span data-stu-id="c4655-120">String</span></span>        | <span data-ttu-id="c4655-p102">由该权限表示的链接范围。值 `anonymous` 表示该链接对任何人均可用，`organization` 表示该链接仅可由登录到同一个租户的用户使用。</span><span class="sxs-lookup"><span data-stu-id="c4655-p102">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="c4655-123">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="c4655-123">preventsDownload</span></span> | <span data-ttu-id="c4655-124">布尔</span><span class="sxs-lookup"><span data-stu-id="c4655-124">Boolean</span></span>       | <span data-ttu-id="c4655-125">如果为 true 则用户只能使用此链接要在 web 上，查看的项目，并且无法将其用于下载项目的内容。</span><span class="sxs-lookup"><span data-stu-id="c4655-125">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="c4655-126">仅为 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="c4655-126">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="c4655-127">webHtml</span><span class="sxs-lookup"><span data-stu-id="c4655-127">webHtml</span></span>        | <span data-ttu-id="c4655-128">String</span><span class="sxs-lookup"><span data-stu-id="c4655-128">String</span></span>        | <span data-ttu-id="c4655-129">对于 `embed` 链接，此属性包含在网页上嵌入项的 `<iframe>` 元素的 HTML 代码。</span><span class="sxs-lookup"><span data-stu-id="c4655-129">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="c4655-130">WebUrl</span><span class="sxs-lookup"><span data-stu-id="c4655-130">webUrl</span></span>         | <span data-ttu-id="c4655-131">String</span><span class="sxs-lookup"><span data-stu-id="c4655-131">String</span></span>        | <span data-ttu-id="c4655-132">在 OneDrive 网站上的浏览器中打开项的 URL。</span><span class="sxs-lookup"><span data-stu-id="c4655-132">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="c4655-134">类型选项</span><span class="sxs-lookup"><span data-stu-id="c4655-134">Type options</span></span>

<span data-ttu-id="c4655-135">下表定义的**type**属性的可能值。</span><span class="sxs-lookup"><span data-stu-id="c4655-135">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="c4655-136">值</span><span class="sxs-lookup"><span data-stu-id="c4655-136">Value</span></span>    | <span data-ttu-id="c4655-137">角色</span><span class="sxs-lookup"><span data-stu-id="c4655-137">Role</span></span>     | <span data-ttu-id="c4655-138">说明</span><span class="sxs-lookup"><span data-stu-id="c4655-138">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="c4655-139">可查看共享链接，允许只读访问。</span><span class="sxs-lookup"><span data-stu-id="c4655-139">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="c4655-140">授予读写权限的编辑共享链接。</span><span class="sxs-lookup"><span data-stu-id="c4655-140">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="c4655-141">可用于将内容嵌入托管网页的仅供查看共享链接。</span><span class="sxs-lookup"><span data-stu-id="c4655-141">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="c4655-142">OneDrive for Business 或 SharePoint 不支持嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="c4655-142">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="c4655-143">作用域选项</span><span class="sxs-lookup"><span data-stu-id="c4655-143">Scope options</span></span>

<span data-ttu-id="c4655-144">下表定义的**范围**属性的可能值。</span><span class="sxs-lookup"><span data-stu-id="c4655-144">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="c4655-145">值</span><span class="sxs-lookup"><span data-stu-id="c4655-145">Value</span></span>            | <span data-ttu-id="c4655-146">说明</span><span class="sxs-lookup"><span data-stu-id="c4655-146">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="c4655-147">带链接的任何人都访问，而无需登录。</span><span class="sxs-lookup"><span data-stu-id="c4655-147">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="c4655-148">这可能包括您的组织外部的人员。</span><span class="sxs-lookup"><span data-stu-id="c4655-148">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="c4655-149">登录到您的组织 （租户） 的任何人都可以使用以下链接获取的访问权限。</span><span class="sxs-lookup"><span data-stu-id="c4655-149">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="c4655-150">仅在 OneDrive for Business 和 SharePoint 中可用。</span><span class="sxs-lookup"><span data-stu-id="c4655-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="c4655-151">仅已被授予访问通过其他手段项的人员可以访问使用此链接的项目。</span><span class="sxs-lookup"><span data-stu-id="c4655-151">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="c4655-152">仅在 OneDrive for Business 和 SharePoint 中可用。</span><span class="sxs-lookup"><span data-stu-id="c4655-152">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="c4655-153">链接授予仅对特定列表的人员的访问权限。</span><span class="sxs-lookup"><span data-stu-id="c4655-153">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="c4655-154">仅在 OneDrive for Business 和 SharePoint 中可用。</span><span class="sxs-lookup"><span data-stu-id="c4655-154">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": ""
}-->
