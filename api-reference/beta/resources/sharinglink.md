---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: c5a08ca3a1a7b91d5cd2277a71f1301adf5edc93
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343085"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="6be14-102">sharingLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="6be14-102">sharingLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6be14-103">**sharingLink**资源将与链接相关的数据项分组到一个单一结构中。</span><span class="sxs-lookup"><span data-stu-id="6be14-103">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="6be14-104">如果[**权限**](permission.md)资源具有非 null **sharingLink** facet, 则该权限表示共享链接 (而不是授予给个人或组的权限)。</span><span class="sxs-lookup"><span data-stu-id="6be14-104">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="6be14-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6be14-105">JSON representation</span></span>

<span data-ttu-id="6be14-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6be14-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6be14-107">属性</span><span class="sxs-lookup"><span data-stu-id="6be14-107">Properties</span></span>

| <span data-ttu-id="6be14-108">属性</span><span class="sxs-lookup"><span data-stu-id="6be14-108">Property</span></span>       | <span data-ttu-id="6be14-109">类型</span><span class="sxs-lookup"><span data-stu-id="6be14-109">Type</span></span>          | <span data-ttu-id="6be14-110">说明</span><span class="sxs-lookup"><span data-stu-id="6be14-110">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="6be14-111">application</span><span class="sxs-lookup"><span data-stu-id="6be14-111">application</span></span>    | <span data-ttu-id="6be14-112">[Identity][]</span><span class="sxs-lookup"><span data-stu-id="6be14-112">[identity][]</span></span>  | <span data-ttu-id="6be14-113">链接所关联的应用。</span><span class="sxs-lookup"><span data-stu-id="6be14-113">The app the link is associated with.</span></span>
| <span data-ttu-id="6be14-114">type</span><span class="sxs-lookup"><span data-stu-id="6be14-114">type</span></span>           | <span data-ttu-id="6be14-115">String</span><span class="sxs-lookup"><span data-stu-id="6be14-115">String</span></span>        | <span data-ttu-id="6be14-116">创建的链接类型。</span><span class="sxs-lookup"><span data-stu-id="6be14-116">The type of the link created.</span></span>
| <span data-ttu-id="6be14-117">scope</span><span class="sxs-lookup"><span data-stu-id="6be14-117">scope</span></span>          | <span data-ttu-id="6be14-118">字符串</span><span class="sxs-lookup"><span data-stu-id="6be14-118">String</span></span>        | <span data-ttu-id="6be14-p101">由该权限表示的链接范围。值 `anonymous` 表示该链接对任何人均可用，`organization` 表示该链接仅可由登录到同一个租户的用户使用。</span><span class="sxs-lookup"><span data-stu-id="6be14-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="6be14-121">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="6be14-121">preventsDownload</span></span> | <span data-ttu-id="6be14-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="6be14-122">Boolean</span></span>       | <span data-ttu-id="6be14-123">如果为 true, 则用户只能使用此链接查看 web 上的项目, 并且无法使用它下载项目的内容。</span><span class="sxs-lookup"><span data-stu-id="6be14-123">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="6be14-124">仅适用于 OneDrive for business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="6be14-124">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="6be14-125">webHtml</span><span class="sxs-lookup"><span data-stu-id="6be14-125">webHtml</span></span>        | <span data-ttu-id="6be14-126">String</span><span class="sxs-lookup"><span data-stu-id="6be14-126">String</span></span>        | <span data-ttu-id="6be14-127">对于 `embed` 链接，此属性包含在网页上嵌入项的 `<iframe>` 元素的 HTML 代码。</span><span class="sxs-lookup"><span data-stu-id="6be14-127">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="6be14-128">WebUrl</span><span class="sxs-lookup"><span data-stu-id="6be14-128">webUrl</span></span>         | <span data-ttu-id="6be14-129">String</span><span class="sxs-lookup"><span data-stu-id="6be14-129">String</span></span>        | <span data-ttu-id="6be14-130">在 OneDrive 网站上的浏览器中打开项的 URL。</span><span class="sxs-lookup"><span data-stu-id="6be14-130">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="6be14-132">类型选项</span><span class="sxs-lookup"><span data-stu-id="6be14-132">Type options</span></span>

<span data-ttu-id="6be14-133">下表定义了**type**属性的可能值。</span><span class="sxs-lookup"><span data-stu-id="6be14-133">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="6be14-134">值</span><span class="sxs-lookup"><span data-stu-id="6be14-134">Value</span></span>    | <span data-ttu-id="6be14-135">角色</span><span class="sxs-lookup"><span data-stu-id="6be14-135">Role</span></span>     | <span data-ttu-id="6be14-136">说明</span><span class="sxs-lookup"><span data-stu-id="6be14-136">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="6be14-137">可查看共享链接，允许只读访问。</span><span class="sxs-lookup"><span data-stu-id="6be14-137">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="6be14-138">授予读写权限的编辑共享链接。</span><span class="sxs-lookup"><span data-stu-id="6be14-138">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="6be14-p103">可用于将内容嵌入托管网页的仅供查看共享链接。 OneDrive for Business 或 SharePoint 不支持嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="6be14-p103">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="6be14-141">作用域选项</span><span class="sxs-lookup"><span data-stu-id="6be14-141">Scope options</span></span>

<span data-ttu-id="6be14-142">下表定义了**scope**属性的可能值。</span><span class="sxs-lookup"><span data-stu-id="6be14-142">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="6be14-143">值</span><span class="sxs-lookup"><span data-stu-id="6be14-143">Value</span></span>            | <span data-ttu-id="6be14-144">说明</span><span class="sxs-lookup"><span data-stu-id="6be14-144">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="6be14-145">拥有该链接的任何人都可以访问, 而无需登录。</span><span class="sxs-lookup"><span data-stu-id="6be14-145">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="6be14-146">这可能包括组织外部的人员。</span><span class="sxs-lookup"><span data-stu-id="6be14-146">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="6be14-147">登录到组织 (租户) 的任何人都可以使用链接获取访问权限。</span><span class="sxs-lookup"><span data-stu-id="6be14-147">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="6be14-148">仅在 OneDrive for business 和 SharePoint 中可用。</span><span class="sxs-lookup"><span data-stu-id="6be14-148">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="6be14-149">只有已通过其他方式授予对项目的访问权限的人员才能使用此链接访问项目。</span><span class="sxs-lookup"><span data-stu-id="6be14-149">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="6be14-150">仅在 OneDrive for business 和 SharePoint 中可用。</span><span class="sxs-lookup"><span data-stu-id="6be14-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="6be14-151">链接仅向特定人员列表授予访问权限。</span><span class="sxs-lookup"><span data-stu-id="6be14-151">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="6be14-152">仅在 OneDrive for business 和 SharePoint 中可用。</span><span class="sxs-lookup"><span data-stu-id="6be14-152">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
