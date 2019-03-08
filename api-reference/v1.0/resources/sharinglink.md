---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: f16f8240800be4b9c1780a4057583381b736f079
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481424"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="91c63-102">SharingLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="91c63-102">SharingLink resource type</span></span>

<span data-ttu-id="91c63-103">**SharingLink** 资源将与链接相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="91c63-103">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="91c63-104">如果 [**权限**](permission.md) 资源有一个非 NULL **sharingLink** facet，则该权限表示共享链接（而不是授予给用户或组的权限）。</span><span class="sxs-lookup"><span data-stu-id="91c63-104">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="91c63-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91c63-105">JSON representation</span></span>

<span data-ttu-id="91c63-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91c63-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": { "@odata.type": "microsoft.graph.identity" },
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="91c63-107">属性</span><span class="sxs-lookup"><span data-stu-id="91c63-107">Properties</span></span>

| <span data-ttu-id="91c63-108">属性</span><span class="sxs-lookup"><span data-stu-id="91c63-108">Property</span></span>    | <span data-ttu-id="91c63-109">类型</span><span class="sxs-lookup"><span data-stu-id="91c63-109">Type</span></span>          | <span data-ttu-id="91c63-110">说明</span><span class="sxs-lookup"><span data-stu-id="91c63-110">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="91c63-111">application</span><span class="sxs-lookup"><span data-stu-id="91c63-111">application</span></span> | <span data-ttu-id="91c63-112">[Identity][]</span><span class="sxs-lookup"><span data-stu-id="91c63-112">[identity][]</span></span>  | <span data-ttu-id="91c63-113">链接所关联的应用。</span><span class="sxs-lookup"><span data-stu-id="91c63-113">The app the link is associated with.</span></span>
| <span data-ttu-id="91c63-114">type</span><span class="sxs-lookup"><span data-stu-id="91c63-114">type</span></span>        | <span data-ttu-id="91c63-115">字符串</span><span class="sxs-lookup"><span data-stu-id="91c63-115">String</span></span>        | <span data-ttu-id="91c63-116">创建的链接类型。</span><span class="sxs-lookup"><span data-stu-id="91c63-116">The type of the link created.</span></span>
| <span data-ttu-id="91c63-117">scope</span><span class="sxs-lookup"><span data-stu-id="91c63-117">scope</span></span>       | <span data-ttu-id="91c63-118">字符串</span><span class="sxs-lookup"><span data-stu-id="91c63-118">String</span></span>        | <span data-ttu-id="91c63-p101">由该权限表示的链接范围。值 `anonymous` 表示该链接对任何人均可用，`organization` 表示该链接仅可由登录到同一个租户的用户使用。</span><span class="sxs-lookup"><span data-stu-id="91c63-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="91c63-121">webHtml</span><span class="sxs-lookup"><span data-stu-id="91c63-121">webHtml</span></span>     | <span data-ttu-id="91c63-122">String</span><span class="sxs-lookup"><span data-stu-id="91c63-122">String</span></span>        | <span data-ttu-id="91c63-123">对于 `embed` 链接，此属性包含在网页上嵌入项的 `<iframe>` 元素的 HTML 代码。</span><span class="sxs-lookup"><span data-stu-id="91c63-123">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="91c63-124">webUrl</span><span class="sxs-lookup"><span data-stu-id="91c63-124">webUrl</span></span>      | <span data-ttu-id="91c63-125">String</span><span class="sxs-lookup"><span data-stu-id="91c63-125">String</span></span>        | <span data-ttu-id="91c63-126">在 OneDrive 网站上的浏览器中打开项的 URL。</span><span class="sxs-lookup"><span data-stu-id="91c63-126">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-options"></a><span data-ttu-id="91c63-128">类型选项</span><span class="sxs-lookup"><span data-stu-id="91c63-128">Type options</span></span>

<span data-ttu-id="91c63-129">此表定义了 **type** 属性的可能值：</span><span class="sxs-lookup"><span data-stu-id="91c63-129">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="91c63-130">值</span><span class="sxs-lookup"><span data-stu-id="91c63-130">Value</span></span>   | <span data-ttu-id="91c63-131">角色</span><span class="sxs-lookup"><span data-stu-id="91c63-131">Role</span></span>    | <span data-ttu-id="91c63-132">说明</span><span class="sxs-lookup"><span data-stu-id="91c63-132">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="91c63-133">可查看共享链接，允许只读访问。</span><span class="sxs-lookup"><span data-stu-id="91c63-133">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="91c63-134">授予读写权限的编辑共享链接。</span><span class="sxs-lookup"><span data-stu-id="91c63-134">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="91c63-p102">可用于将内容嵌入托管网页的仅供查看共享链接。 OneDrive for Business 或 SharePoint 不支持嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="91c63-p102">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-options"></a><span data-ttu-id="91c63-137">作用域选项</span><span class="sxs-lookup"><span data-stu-id="91c63-137">Scope options</span></span>

| <span data-ttu-id="91c63-138">值</span><span class="sxs-lookup"><span data-stu-id="91c63-138">Value</span></span>          | <span data-ttu-id="91c63-139">说明</span><span class="sxs-lookup"><span data-stu-id="91c63-139">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="91c63-140">拥有该链接的任何人都可以访问, 而无需登录。</span><span class="sxs-lookup"><span data-stu-id="91c63-140">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="91c63-141">这可能包括组织外部的人员。</span><span class="sxs-lookup"><span data-stu-id="91c63-141">This may include people outside of your organization.</span></span>
| `organization` | <span data-ttu-id="91c63-142">登录到组织 (租户) 的任何人都可以使用链接获取访问权限。</span><span class="sxs-lookup"><span data-stu-id="91c63-142">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="91c63-143">仅在 OneDrive for business 和 SharePoint 中可用。</span><span class="sxs-lookup"><span data-stu-id="91c63-143">Only available in OneDrive for Business and SharePoint.</span></span>

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
