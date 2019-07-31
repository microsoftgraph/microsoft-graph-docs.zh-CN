---
author: JeremyKelley
description: SharingLink 资源将与链接相关的数据项分组到一个单一结构中。
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f1ebff332227410bcb67d87de50a97dd2e078660
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965129"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="20d4b-103">sharingLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="20d4b-103">sharingLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20d4b-104">**SharingLink**资源将与链接相关的数据项分组到一个单一结构中。</span><span class="sxs-lookup"><span data-stu-id="20d4b-104">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="20d4b-105">如果[**权限**](permission.md)资源具有非 null **sharingLink** facet, 则该权限表示共享链接 (而不是授予给个人或组的权限)。</span><span class="sxs-lookup"><span data-stu-id="20d4b-105">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="20d4b-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20d4b-106">JSON representation</span></span>

<span data-ttu-id="20d4b-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20d4b-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="20d4b-108">属性</span><span class="sxs-lookup"><span data-stu-id="20d4b-108">Properties</span></span>

| <span data-ttu-id="20d4b-109">属性</span><span class="sxs-lookup"><span data-stu-id="20d4b-109">Property</span></span>       | <span data-ttu-id="20d4b-110">类型</span><span class="sxs-lookup"><span data-stu-id="20d4b-110">Type</span></span>          | <span data-ttu-id="20d4b-111">说明</span><span class="sxs-lookup"><span data-stu-id="20d4b-111">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="20d4b-112">application</span><span class="sxs-lookup"><span data-stu-id="20d4b-112">application</span></span>    | <span data-ttu-id="20d4b-113">[Identity][]</span><span class="sxs-lookup"><span data-stu-id="20d4b-113">[identity][]</span></span>  | <span data-ttu-id="20d4b-114">链接所关联的应用。</span><span class="sxs-lookup"><span data-stu-id="20d4b-114">The app the link is associated with.</span></span>
| <span data-ttu-id="20d4b-115">type</span><span class="sxs-lookup"><span data-stu-id="20d4b-115">type</span></span>           | <span data-ttu-id="20d4b-116">String</span><span class="sxs-lookup"><span data-stu-id="20d4b-116">String</span></span>        | <span data-ttu-id="20d4b-117">创建的链接类型。</span><span class="sxs-lookup"><span data-stu-id="20d4b-117">The type of the link created.</span></span>
| <span data-ttu-id="20d4b-118">scope</span><span class="sxs-lookup"><span data-stu-id="20d4b-118">scope</span></span>          | <span data-ttu-id="20d4b-119">字符串</span><span class="sxs-lookup"><span data-stu-id="20d4b-119">String</span></span>        | <span data-ttu-id="20d4b-p101">由该权限表示的链接范围。值 `anonymous` 表示该链接对任何人均可用，`organization` 表示该链接仅可由登录到同一个租户的用户使用。</span><span class="sxs-lookup"><span data-stu-id="20d4b-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="20d4b-122">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="20d4b-122">preventsDownload</span></span> | <span data-ttu-id="20d4b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="20d4b-123">Boolean</span></span>       | <span data-ttu-id="20d4b-124">如果为 true, 则用户只能使用此链接查看 web 上的项目, 并且无法使用它下载项目的内容。</span><span class="sxs-lookup"><span data-stu-id="20d4b-124">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="20d4b-125">仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="20d4b-125">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="20d4b-126">webHtml</span><span class="sxs-lookup"><span data-stu-id="20d4b-126">webHtml</span></span>        | <span data-ttu-id="20d4b-127">String</span><span class="sxs-lookup"><span data-stu-id="20d4b-127">String</span></span>        | <span data-ttu-id="20d4b-128">对于 `embed` 链接，此属性包含在网页上嵌入项的 `<iframe>` 元素的 HTML 代码。</span><span class="sxs-lookup"><span data-stu-id="20d4b-128">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="20d4b-129">WebUrl</span><span class="sxs-lookup"><span data-stu-id="20d4b-129">webUrl</span></span>         | <span data-ttu-id="20d4b-130">String</span><span class="sxs-lookup"><span data-stu-id="20d4b-130">String</span></span>        | <span data-ttu-id="20d4b-131">在 OneDrive 网站上的浏览器中打开项的 URL。</span><span class="sxs-lookup"><span data-stu-id="20d4b-131">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="20d4b-133">类型选项</span><span class="sxs-lookup"><span data-stu-id="20d4b-133">Type options</span></span>

<span data-ttu-id="20d4b-134">下表定义了**type**属性的可能值。</span><span class="sxs-lookup"><span data-stu-id="20d4b-134">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="20d4b-135">值</span><span class="sxs-lookup"><span data-stu-id="20d4b-135">Value</span></span>    | <span data-ttu-id="20d4b-136">角色</span><span class="sxs-lookup"><span data-stu-id="20d4b-136">Role</span></span>     | <span data-ttu-id="20d4b-137">说明</span><span class="sxs-lookup"><span data-stu-id="20d4b-137">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="20d4b-138">可查看共享链接，允许只读访问。</span><span class="sxs-lookup"><span data-stu-id="20d4b-138">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="20d4b-139">授予读写权限的编辑共享链接。</span><span class="sxs-lookup"><span data-stu-id="20d4b-139">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="20d4b-p103">可用于将内容嵌入托管网页的仅供查看共享链接。 OneDrive for Business 或 SharePoint 不支持嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="20d4b-p103">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="20d4b-142">作用域选项</span><span class="sxs-lookup"><span data-stu-id="20d4b-142">Scope options</span></span>

<span data-ttu-id="20d4b-143">下表定义了**scope**属性的可能值。</span><span class="sxs-lookup"><span data-stu-id="20d4b-143">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="20d4b-144">值</span><span class="sxs-lookup"><span data-stu-id="20d4b-144">Value</span></span>            | <span data-ttu-id="20d4b-145">说明</span><span class="sxs-lookup"><span data-stu-id="20d4b-145">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="20d4b-146">拥有该链接的任何人都可以访问, 而无需登录。</span><span class="sxs-lookup"><span data-stu-id="20d4b-146">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="20d4b-147">这可能包括组织外部的人员。</span><span class="sxs-lookup"><span data-stu-id="20d4b-147">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="20d4b-148">登录到组织 (租户) 的任何人都可以使用链接获取访问权限。</span><span class="sxs-lookup"><span data-stu-id="20d4b-148">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="20d4b-149">仅在 OneDrive for Business 和 SharePoint 中可用。</span><span class="sxs-lookup"><span data-stu-id="20d4b-149">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="20d4b-150">只有已通过其他方式授予对项目的访问权限的人员才能使用此链接访问项目。</span><span class="sxs-lookup"><span data-stu-id="20d4b-150">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="20d4b-151">仅在 OneDrive for Business 和 SharePoint 中可用。</span><span class="sxs-lookup"><span data-stu-id="20d4b-151">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="20d4b-152">链接仅向特定人员列表授予访问权限。</span><span class="sxs-lookup"><span data-stu-id="20d4b-152">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="20d4b-153">仅在 OneDrive for Business 和 SharePoint 中可用。</span><span class="sxs-lookup"><span data-stu-id="20d4b-153">Only available in OneDrive for Business and SharePoint.</span></span>

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
