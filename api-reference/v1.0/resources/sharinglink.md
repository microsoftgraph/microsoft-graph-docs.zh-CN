---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
description: SharingLink 资源将与链接相关的数据项分组到一个单一结构。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6a696a95c3c636a84bb79498375b0c023617548d
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2020
ms.locfileid: "43934883"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="b02f0-103">SharingLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="b02f0-103">SharingLink resource type</span></span>

<span data-ttu-id="b02f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b02f0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b02f0-105">**SharingLink** 资源将与链接相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="b02f0-105">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="b02f0-106">如果 [**权限**](permission.md) 资源有一个非 NULL **sharingLink** facet，则该权限表示共享链接（而不是授予给用户或组的权限）。</span><span class="sxs-lookup"><span data-stu-id="b02f0-106">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b02f0-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b02f0-107">JSON representation</span></span>

<span data-ttu-id="b02f0-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b02f0-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b02f0-109">属性</span><span class="sxs-lookup"><span data-stu-id="b02f0-109">Properties</span></span>

| <span data-ttu-id="b02f0-110">属性</span><span class="sxs-lookup"><span data-stu-id="b02f0-110">Property</span></span>    | <span data-ttu-id="b02f0-111">类型</span><span class="sxs-lookup"><span data-stu-id="b02f0-111">Type</span></span>          | <span data-ttu-id="b02f0-112">说明</span><span class="sxs-lookup"><span data-stu-id="b02f0-112">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="b02f0-113">application</span><span class="sxs-lookup"><span data-stu-id="b02f0-113">application</span></span> | <span data-ttu-id="b02f0-114">[Identity][]</span><span class="sxs-lookup"><span data-stu-id="b02f0-114">[identity][]</span></span>  | <span data-ttu-id="b02f0-115">链接所关联的应用。</span><span class="sxs-lookup"><span data-stu-id="b02f0-115">The app the link is associated with.</span></span>
| <span data-ttu-id="b02f0-116">type</span><span class="sxs-lookup"><span data-stu-id="b02f0-116">type</span></span>        | <span data-ttu-id="b02f0-117">字符串</span><span class="sxs-lookup"><span data-stu-id="b02f0-117">String</span></span>        | <span data-ttu-id="b02f0-118">创建的链接类型。</span><span class="sxs-lookup"><span data-stu-id="b02f0-118">The type of the link created.</span></span>
| <span data-ttu-id="b02f0-119">scope</span><span class="sxs-lookup"><span data-stu-id="b02f0-119">scope</span></span>       | <span data-ttu-id="b02f0-120">字符串</span><span class="sxs-lookup"><span data-stu-id="b02f0-120">String</span></span>        | <span data-ttu-id="b02f0-p101">由该权限表示的链接范围。值 `anonymous` 表示该链接对任何人均可用，`organization` 表示该链接仅可由登录到同一个租户的用户使用。</span><span class="sxs-lookup"><span data-stu-id="b02f0-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="b02f0-123">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="b02f0-123">preventsDownload</span></span> | <span data-ttu-id="b02f0-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="b02f0-124">Boolean</span></span>       | <span data-ttu-id="b02f0-125">如果为 true，则用户只能使用此链接查看 web 上的项目，并且无法使用它下载项目的内容。</span><span class="sxs-lookup"><span data-stu-id="b02f0-125">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="b02f0-126">仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="b02f0-126">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="b02f0-127">webHtml</span><span class="sxs-lookup"><span data-stu-id="b02f0-127">webHtml</span></span>     | <span data-ttu-id="b02f0-128">String</span><span class="sxs-lookup"><span data-stu-id="b02f0-128">String</span></span>        | <span data-ttu-id="b02f0-129">对于 `embed` 链接，此属性包含在网页上嵌入项的 `<iframe>` 元素的 HTML 代码。</span><span class="sxs-lookup"><span data-stu-id="b02f0-129">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="b02f0-130">WebUrl</span><span class="sxs-lookup"><span data-stu-id="b02f0-130">webUrl</span></span>      | <span data-ttu-id="b02f0-131">字符串</span><span class="sxs-lookup"><span data-stu-id="b02f0-131">String</span></span>        | <span data-ttu-id="b02f0-132">在 OneDrive 网站上的浏览器中打开项的 URL。</span><span class="sxs-lookup"><span data-stu-id="b02f0-132">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-options"></a><span data-ttu-id="b02f0-134">类型选项</span><span class="sxs-lookup"><span data-stu-id="b02f0-134">Type options</span></span>

<span data-ttu-id="b02f0-135">此表定义了 **type** 属性的可能值：</span><span class="sxs-lookup"><span data-stu-id="b02f0-135">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="b02f0-136">值</span><span class="sxs-lookup"><span data-stu-id="b02f0-136">Value</span></span>   | <span data-ttu-id="b02f0-137">Role</span><span class="sxs-lookup"><span data-stu-id="b02f0-137">Role</span></span>    | <span data-ttu-id="b02f0-138">说明</span><span class="sxs-lookup"><span data-stu-id="b02f0-138">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="b02f0-139">可查看共享链接，允许只读访问。</span><span class="sxs-lookup"><span data-stu-id="b02f0-139">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="b02f0-140">授予读写权限的编辑共享链接。</span><span class="sxs-lookup"><span data-stu-id="b02f0-140">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="b02f0-p103">可用于将内容嵌入托管网页的仅供查看共享链接。 OneDrive for Business 或 SharePoint 不支持嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="b02f0-p103">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-options"></a><span data-ttu-id="b02f0-143">作用域选项</span><span class="sxs-lookup"><span data-stu-id="b02f0-143">Scope options</span></span>

| <span data-ttu-id="b02f0-144">值</span><span class="sxs-lookup"><span data-stu-id="b02f0-144">Value</span></span>          | <span data-ttu-id="b02f0-145">说明</span><span class="sxs-lookup"><span data-stu-id="b02f0-145">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="b02f0-146">拥有该链接的任何人都可以访问，无需登录。</span><span class="sxs-lookup"><span data-stu-id="b02f0-146">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="b02f0-147">这可能包括组织外部的人员。</span><span class="sxs-lookup"><span data-stu-id="b02f0-147">This may include people outside of your organization.</span></span>
| `organization` | <span data-ttu-id="b02f0-148">登录到组织（租户）的任何人都可以使用该链接获取访问权限。</span><span class="sxs-lookup"><span data-stu-id="b02f0-148">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="b02f0-149">仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="b02f0-149">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(view,edit,embed) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization) are in resource, but () are in table"
  ],
  "tocPath": "Facets/SharingLink"
} -->
