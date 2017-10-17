---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
ms.openlocfilehash: 7b7729899d134fa1d5de7debb1f209ec5aadd70d
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="9e74e-102">SharingLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e74e-102">SharingLink resource type</span></span>

<span data-ttu-id="9e74e-103">**SharingLink** 资源将与链接相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="9e74e-103">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="9e74e-104">如果 [**权限**](permission.md) 资源有一个非 NULL **sharingLink** facet，则该权限表示共享链接（而不是授予给用户或组的权限）。</span><span class="sxs-lookup"><span data-stu-id="9e74e-104">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e74e-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e74e-105">JSON representation</span></span>

<span data-ttu-id="9e74e-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e74e-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="9e74e-107">属性</span><span class="sxs-lookup"><span data-stu-id="9e74e-107">Properties</span></span>

| <span data-ttu-id="9e74e-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e74e-108">Property</span></span>    | <span data-ttu-id="9e74e-109">类型</span><span class="sxs-lookup"><span data-stu-id="9e74e-109">Type</span></span>          | <span data-ttu-id="9e74e-110">说明</span><span class="sxs-lookup"><span data-stu-id="9e74e-110">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="9e74e-111">application</span><span class="sxs-lookup"><span data-stu-id="9e74e-111">application</span></span> | <span data-ttu-id="9e74e-112">[标识][]</span><span class="sxs-lookup"><span data-stu-id="9e74e-112">[identity][]</span></span>  | <span data-ttu-id="9e74e-113">链接所关联的应用。</span><span class="sxs-lookup"><span data-stu-id="9e74e-113">The app the link is associated with.</span></span>
| <span data-ttu-id="9e74e-114">type</span><span class="sxs-lookup"><span data-stu-id="9e74e-114">type</span></span>        | <span data-ttu-id="9e74e-115">String</span><span class="sxs-lookup"><span data-stu-id="9e74e-115">String</span></span>        | <span data-ttu-id="9e74e-116">创建的链接类型。</span><span class="sxs-lookup"><span data-stu-id="9e74e-116">The type of the link created.</span></span>
| <span data-ttu-id="9e74e-117">scope</span><span class="sxs-lookup"><span data-stu-id="9e74e-117">scope</span></span>       | <span data-ttu-id="9e74e-118">String</span><span class="sxs-lookup"><span data-stu-id="9e74e-118">String</span></span>        | <span data-ttu-id="9e74e-p101">由该权限表示的链接范围。值 `anonymous` 表示该链接对任何人均可用，`organization` 表示该链接仅可由登录到同一个租户的用户使用。</span><span class="sxs-lookup"><span data-stu-id="9e74e-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="9e74e-121">webHtml</span><span class="sxs-lookup"><span data-stu-id="9e74e-121">webHtml</span></span>     | <span data-ttu-id="9e74e-122">String</span><span class="sxs-lookup"><span data-stu-id="9e74e-122">String</span></span>        | <span data-ttu-id="9e74e-123">对于 `embed` 链接，此属性包含在网页中嵌入项的 `<iframe>` 元素的 HTML 代码。</span><span class="sxs-lookup"><span data-stu-id="9e74e-123">For embeddable links, this property contains the HTML code for an  element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="9e74e-124">WebUrl</span><span class="sxs-lookup"><span data-stu-id="9e74e-124">webUrl</span></span>      | <span data-ttu-id="9e74e-125">String</span><span class="sxs-lookup"><span data-stu-id="9e74e-125">String</span></span>        | <span data-ttu-id="9e74e-126">在 OneDrive 网站上的浏览器中打开项的 URL。</span><span class="sxs-lookup"><span data-stu-id="9e74e-126">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-enumeration"></a><span data-ttu-id="9e74e-128">Type 枚举</span><span class="sxs-lookup"><span data-stu-id="9e74e-128">Type enumeration</span></span>

<span data-ttu-id="9e74e-129">此表定义了 **type** 属性的可能值：</span><span class="sxs-lookup"><span data-stu-id="9e74e-129">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="9e74e-130">值</span><span class="sxs-lookup"><span data-stu-id="9e74e-130">Value</span></span>   | <span data-ttu-id="9e74e-131">角色</span><span class="sxs-lookup"><span data-stu-id="9e74e-131">Role</span></span>    | <span data-ttu-id="9e74e-132">说明</span><span class="sxs-lookup"><span data-stu-id="9e74e-132">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="9e74e-133">可查看共享链接，允许只读访问。</span><span class="sxs-lookup"><span data-stu-id="9e74e-133">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="9e74e-134">授予读写权限的编辑共享链接。</span><span class="sxs-lookup"><span data-stu-id="9e74e-134">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="9e74e-135">可用于将内容嵌入托管网页的仅供查看共享链接。</span><span class="sxs-lookup"><span data-stu-id="9e74e-135">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="9e74e-136">OneDrive for Business 或 SharePoint 不支持嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="9e74e-136">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-enumeration"></a><span data-ttu-id="9e74e-137">作用域枚举</span><span class="sxs-lookup"><span data-stu-id="9e74e-137">Scope enumeration</span></span>

| <span data-ttu-id="9e74e-138">值</span><span class="sxs-lookup"><span data-stu-id="9e74e-138">Value</span></span>          | <span data-ttu-id="9e74e-139">说明</span><span class="sxs-lookup"><span data-stu-id="9e74e-139">Description</span></span>                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="9e74e-140">任何人均可使用共享链接。</span><span class="sxs-lookup"><span data-stu-id="9e74e-140">The sharing link is available for anyone to use.</span></span>                                                                            |
| `organization` | <span data-ttu-id="9e74e-p103">同一组织（租户）中的任何人均可使用共享链接。不适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="9e74e-p103">The sharing link is available for anyone within the same organization (tenant) to use. Not available for OneDrive Personal.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "Facets/SharingLink"
} -->
