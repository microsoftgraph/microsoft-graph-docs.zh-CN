---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
ms.openlocfilehash: 7639dab9f63a948b3e9a849d8d320de60f5a0954
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23270487"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="b9507-102">SharingLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9507-102">SharingLink resource type</span></span>

<span data-ttu-id="b9507-103">**SharingLink** 资源将与链接相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="b9507-103">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="b9507-104">如果 [**权限**](permission.md) 资源有一个非 NULL **sharingLink** facet，则该权限表示共享链接（而不是授予给用户或组的权限）。</span><span class="sxs-lookup"><span data-stu-id="b9507-104">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9507-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9507-105">JSON representation</span></span>

<span data-ttu-id="b9507-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9507-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b9507-107">属性</span><span class="sxs-lookup"><span data-stu-id="b9507-107">Properties</span></span>

| <span data-ttu-id="b9507-108">属性</span><span class="sxs-lookup"><span data-stu-id="b9507-108">Property</span></span>    | <span data-ttu-id="b9507-109">类型</span><span class="sxs-lookup"><span data-stu-id="b9507-109">Type</span></span>          | <span data-ttu-id="b9507-110">说明</span><span class="sxs-lookup"><span data-stu-id="b9507-110">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="b9507-111">application</span><span class="sxs-lookup"><span data-stu-id="b9507-111">application</span></span> | <span data-ttu-id="b9507-112">[Identity][]</span><span class="sxs-lookup"><span data-stu-id="b9507-112">[identity][]</span></span>  | <span data-ttu-id="b9507-113">链接所关联的应用。</span><span class="sxs-lookup"><span data-stu-id="b9507-113">The app the link is associated with.</span></span>
| <span data-ttu-id="b9507-114">类型</span><span class="sxs-lookup"><span data-stu-id="b9507-114">type</span></span>        | <span data-ttu-id="b9507-115">字符串</span><span class="sxs-lookup"><span data-stu-id="b9507-115">String</span></span>        | <span data-ttu-id="b9507-116">创建的链接类型。</span><span class="sxs-lookup"><span data-stu-id="b9507-116">The type of the link created.</span></span>
| <span data-ttu-id="b9507-117">范围</span><span class="sxs-lookup"><span data-stu-id="b9507-117">scope</span></span>       | <span data-ttu-id="b9507-118">字符串</span><span class="sxs-lookup"><span data-stu-id="b9507-118">String</span></span>        | <span data-ttu-id="b9507-p101">由该权限表示的链接范围。值 `anonymous` 表示该链接对任何人均可用，`organization` 表示该链接仅可由登录到同一个租户的用户使用。</span><span class="sxs-lookup"><span data-stu-id="b9507-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="b9507-121">webHtml</span><span class="sxs-lookup"><span data-stu-id="b9507-121">webHtml</span></span>     | <span data-ttu-id="b9507-122">字符串</span><span class="sxs-lookup"><span data-stu-id="b9507-122">String</span></span>        | <span data-ttu-id="b9507-123">对于 `embed` 链接，此属性包含在网页上嵌入项的 `<iframe>` 元素的 HTML 代码。</span><span class="sxs-lookup"><span data-stu-id="b9507-123">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="b9507-124">WebUrl</span><span class="sxs-lookup"><span data-stu-id="b9507-124">webUrl</span></span>      | <span data-ttu-id="b9507-125">字符串</span><span class="sxs-lookup"><span data-stu-id="b9507-125">String</span></span>        | <span data-ttu-id="b9507-126">在 OneDrive 网站上的浏览器中打开项的 URL。</span><span class="sxs-lookup"><span data-stu-id="b9507-126">A URL that opens the item in the browser on the OneDrive website.</span></span>

[标识]: identity.md
[Identity]: identity.md

## <a name="type-options"></a><span data-ttu-id="b9507-128">类型选项</span><span class="sxs-lookup"><span data-stu-id="b9507-128">Type options</span></span>

<span data-ttu-id="b9507-129">此表定义了 **type** 属性的可能值：</span><span class="sxs-lookup"><span data-stu-id="b9507-129">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="b9507-130">值</span><span class="sxs-lookup"><span data-stu-id="b9507-130">Value</span></span>   | <span data-ttu-id="b9507-131">角色</span><span class="sxs-lookup"><span data-stu-id="b9507-131">Role</span></span>    | <span data-ttu-id="b9507-132">说明</span><span class="sxs-lookup"><span data-stu-id="b9507-132">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="b9507-133">可查看共享链接，允许只读访问。</span><span class="sxs-lookup"><span data-stu-id="b9507-133">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="b9507-134">授予读写权限的编辑共享链接。</span><span class="sxs-lookup"><span data-stu-id="b9507-134">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="b9507-135">可用于将内容嵌入托管网页的仅供查看共享链接。</span><span class="sxs-lookup"><span data-stu-id="b9507-135">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="b9507-136">OneDrive for Business 或 SharePoint 不支持嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="b9507-136">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-options"></a><span data-ttu-id="b9507-137">范围选项</span><span class="sxs-lookup"><span data-stu-id="b9507-137">Scope options folder</span></span>

| <span data-ttu-id="b9507-138">值</span><span class="sxs-lookup"><span data-stu-id="b9507-138">Value</span></span>          | <span data-ttu-id="b9507-139">说明</span><span class="sxs-lookup"><span data-stu-id="b9507-139">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="b9507-140">带链接的任何人都可访问，而无需登录。</span><span class="sxs-lookup"><span data-stu-id="b9507-140">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="b9507-141">这可能包括您的组织外部的人员。</span><span class="sxs-lookup"><span data-stu-id="b9507-141">This may include people outside of your organization.</span></span>
| `organization` | <span data-ttu-id="b9507-142">任何登录到你的组织（承租人）可以使用该链接获取访问权限。</span><span class="sxs-lookup"><span data-stu-id="b9507-142">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="b9507-143">仅适用于商业版OneDrive和SharePoint。</span><span class="sxs-lookup"><span data-stu-id="b9507-143">Only available in OneDrive for Business and SharePoint.</span></span>

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
