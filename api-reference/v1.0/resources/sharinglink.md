---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
description: SharingLink 资源将与链接相关的数据项分组到一个单一结构。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3195207588061840c4e1394e1460f74d3728510c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446861"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="0f572-103">SharingLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f572-103">SharingLink resource type</span></span>

<span data-ttu-id="0f572-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0f572-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f572-105">**SharingLink** 资源将与链接相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="0f572-105">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="0f572-106">如果 [**权限**](permission.md) 资源有一个非 NULL **sharingLink** facet，则该权限表示共享链接（而不是授予给用户或组的权限）。</span><span class="sxs-lookup"><span data-stu-id="0f572-106">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f572-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f572-107">JSON representation</span></span>

<span data-ttu-id="0f572-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f572-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0f572-109">属性</span><span class="sxs-lookup"><span data-stu-id="0f572-109">Properties</span></span>

| <span data-ttu-id="0f572-110">属性</span><span class="sxs-lookup"><span data-stu-id="0f572-110">Property</span></span>    | <span data-ttu-id="0f572-111">类型</span><span class="sxs-lookup"><span data-stu-id="0f572-111">Type</span></span>          | <span data-ttu-id="0f572-112">说明</span><span class="sxs-lookup"><span data-stu-id="0f572-112">Description</span></span>
|:------------|:--------------|:-------------------------------------
| <span data-ttu-id="0f572-113">application</span><span class="sxs-lookup"><span data-stu-id="0f572-113">application</span></span> | <span data-ttu-id="0f572-114">[Identity][]</span><span class="sxs-lookup"><span data-stu-id="0f572-114">[identity][]</span></span>  | <span data-ttu-id="0f572-115">链接所关联的应用。</span><span class="sxs-lookup"><span data-stu-id="0f572-115">The app the link is associated with.</span></span>
| <span data-ttu-id="0f572-116">type</span><span class="sxs-lookup"><span data-stu-id="0f572-116">type</span></span>        | <span data-ttu-id="0f572-117">String</span><span class="sxs-lookup"><span data-stu-id="0f572-117">String</span></span>        | <span data-ttu-id="0f572-118">创建的链接类型。</span><span class="sxs-lookup"><span data-stu-id="0f572-118">The type of the link created.</span></span>
| <span data-ttu-id="0f572-119">scope</span><span class="sxs-lookup"><span data-stu-id="0f572-119">scope</span></span>       | <span data-ttu-id="0f572-120">字符串</span><span class="sxs-lookup"><span data-stu-id="0f572-120">String</span></span>        | <span data-ttu-id="0f572-p101">由该权限表示的链接范围。值 `anonymous` 表示该链接对任何人均可用，`organization` 表示该链接仅可由登录到同一个租户的用户使用。</span><span class="sxs-lookup"><span data-stu-id="0f572-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="0f572-123">webHtml</span><span class="sxs-lookup"><span data-stu-id="0f572-123">webHtml</span></span>     | <span data-ttu-id="0f572-124">String</span><span class="sxs-lookup"><span data-stu-id="0f572-124">String</span></span>        | <span data-ttu-id="0f572-125">对于 `embed` 链接，此属性包含在网页上嵌入项的 `<iframe>` 元素的 HTML 代码。</span><span class="sxs-lookup"><span data-stu-id="0f572-125">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="0f572-126">webUrl</span><span class="sxs-lookup"><span data-stu-id="0f572-126">webUrl</span></span>      | <span data-ttu-id="0f572-127">String</span><span class="sxs-lookup"><span data-stu-id="0f572-127">String</span></span>        | <span data-ttu-id="0f572-128">在 OneDrive 网站上的浏览器中打开项的 URL。</span><span class="sxs-lookup"><span data-stu-id="0f572-128">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

## <a name="type-options"></a><span data-ttu-id="0f572-130">类型选项</span><span class="sxs-lookup"><span data-stu-id="0f572-130">Type options</span></span>

<span data-ttu-id="0f572-131">此表定义了 **type** 属性的可能值：</span><span class="sxs-lookup"><span data-stu-id="0f572-131">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="0f572-132">值</span><span class="sxs-lookup"><span data-stu-id="0f572-132">Value</span></span>   | <span data-ttu-id="0f572-133">Role</span><span class="sxs-lookup"><span data-stu-id="0f572-133">Role</span></span>    | <span data-ttu-id="0f572-134">说明</span><span class="sxs-lookup"><span data-stu-id="0f572-134">Description</span></span>
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | <span data-ttu-id="0f572-135">可查看共享链接，允许只读访问。</span><span class="sxs-lookup"><span data-stu-id="0f572-135">A view-only sharing link, allowing read-only access.</span></span>
| `edit`  | `write` | <span data-ttu-id="0f572-136">授予读写权限的编辑共享链接。</span><span class="sxs-lookup"><span data-stu-id="0f572-136">An edit sharing link, allowing read-write access.</span></span>
| `embed` | `read`  | <span data-ttu-id="0f572-p102">可用于将内容嵌入托管网页的仅供查看共享链接。 OneDrive for Business 或 SharePoint 不支持嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="0f572-p102">A view-only sharing link that can be used to embed content into a host webpage. Embed links are not available for OneDrive for Business or SharePoint.</span></span>

## <a name="scope-options"></a><span data-ttu-id="0f572-139">作用域选项</span><span class="sxs-lookup"><span data-stu-id="0f572-139">Scope options</span></span>

| <span data-ttu-id="0f572-140">值</span><span class="sxs-lookup"><span data-stu-id="0f572-140">Value</span></span>          | <span data-ttu-id="0f572-141">说明</span><span class="sxs-lookup"><span data-stu-id="0f572-141">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="0f572-142">拥有该链接的任何人都可以访问，无需登录。</span><span class="sxs-lookup"><span data-stu-id="0f572-142">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="0f572-143">这可能包括组织外部的人员。</span><span class="sxs-lookup"><span data-stu-id="0f572-143">This may include people outside of your organization.</span></span>
| `organization` | <span data-ttu-id="0f572-144">登录到组织（租户）的任何人都可以使用该链接获取访问权限。</span><span class="sxs-lookup"><span data-stu-id="0f572-144">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="0f572-145">仅适用于 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="0f572-145">Only available in OneDrive for Business and SharePoint.</span></span>

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
