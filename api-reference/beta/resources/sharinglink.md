---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: c21c891981106faa4b631bb2713913bfa8ed0713
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521451"
---
# <a name="sharinglink-resource-type"></a><span data-ttu-id="72759-102">SharingLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="72759-102">sharingLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72759-103">**SharingLink** 资源将与链接相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="72759-103">The **sharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="72759-104">如果 [**权限**](permission.md) 资源有一个非 NULL **sharingLink** facet，则该权限表示共享链接（而不是授予给用户或组的权限）。</span><span class="sxs-lookup"><span data-stu-id="72759-104">If a [**permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="72759-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72759-105">JSON representation</span></span>

<span data-ttu-id="72759-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72759-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="72759-107">属性</span><span class="sxs-lookup"><span data-stu-id="72759-107">Properties</span></span>

| <span data-ttu-id="72759-108">属性</span><span class="sxs-lookup"><span data-stu-id="72759-108">Property</span></span>       | <span data-ttu-id="72759-109">类型</span><span class="sxs-lookup"><span data-stu-id="72759-109">Type</span></span>          | <span data-ttu-id="72759-110">说明</span><span class="sxs-lookup"><span data-stu-id="72759-110">Description</span></span>
|:---------------|:--------------|:-------------------------------------
| <span data-ttu-id="72759-111">application</span><span class="sxs-lookup"><span data-stu-id="72759-111">application</span></span>    | <span data-ttu-id="72759-112">[Identity][]</span><span class="sxs-lookup"><span data-stu-id="72759-112">[identity][]</span></span>  | <span data-ttu-id="72759-113">链接所关联的应用。</span><span class="sxs-lookup"><span data-stu-id="72759-113">The app the link is associated with.</span></span>
| <span data-ttu-id="72759-114">type</span><span class="sxs-lookup"><span data-stu-id="72759-114">type</span></span>           | <span data-ttu-id="72759-115">String</span><span class="sxs-lookup"><span data-stu-id="72759-115">String</span></span>        | <span data-ttu-id="72759-116">创建的链接类型。</span><span class="sxs-lookup"><span data-stu-id="72759-116">The type of the link created.</span></span>
| <span data-ttu-id="72759-117">scope</span><span class="sxs-lookup"><span data-stu-id="72759-117">scope</span></span>          | <span data-ttu-id="72759-118">String</span><span class="sxs-lookup"><span data-stu-id="72759-118">String</span></span>        | <span data-ttu-id="72759-p101">由该权限表示的链接范围。值 `anonymous` 表示该链接对任何人均可用，`organization` 表示该链接仅可由登录到同一个租户的用户使用。</span><span class="sxs-lookup"><span data-stu-id="72759-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span>
| <span data-ttu-id="72759-121">preventsDownload</span><span class="sxs-lookup"><span data-stu-id="72759-121">preventsDownload</span></span> | <span data-ttu-id="72759-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="72759-122">Boolean</span></span>       | <span data-ttu-id="72759-123">如果为 true 则用户只能使用此链接要在 web 上，查看的项目，并且无法将其用于下载项目的内容。</span><span class="sxs-lookup"><span data-stu-id="72759-123">If true then the user can only use this link to view the item on the web, and cannot use it to download the contents of the item.</span></span> <span data-ttu-id="72759-124">仅为 OneDrive for Business 和 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="72759-124">Only for OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="72759-125">webHtml</span><span class="sxs-lookup"><span data-stu-id="72759-125">webHtml</span></span>        | <span data-ttu-id="72759-126">String</span><span class="sxs-lookup"><span data-stu-id="72759-126">String</span></span>        | <span data-ttu-id="72759-127">对于 `embed` 链接，此属性包含在网页上嵌入项的 `<iframe>` 元素的 HTML 代码。</span><span class="sxs-lookup"><span data-stu-id="72759-127">For `embed` links, this property contains the HTML code for an `<iframe>` element that will embed the item in a webpage.</span></span>
| <span data-ttu-id="72759-128">WebUrl</span><span class="sxs-lookup"><span data-stu-id="72759-128">webUrl</span></span>         | <span data-ttu-id="72759-129">String</span><span class="sxs-lookup"><span data-stu-id="72759-129">String</span></span>        | <span data-ttu-id="72759-130">在 OneDrive 网站上的浏览器中打开项的 URL。</span><span class="sxs-lookup"><span data-stu-id="72759-130">A URL that opens the item in the browser on the OneDrive website.</span></span>

[Identity]: identity.md

### <a name="type-options"></a><span data-ttu-id="72759-132">类型选项</span><span class="sxs-lookup"><span data-stu-id="72759-132">Type options</span></span>

<span data-ttu-id="72759-133">下表定义的**type**属性的可能值。</span><span class="sxs-lookup"><span data-stu-id="72759-133">The following table defines the possible values for the **type** property.</span></span>

| <span data-ttu-id="72759-134">值</span><span class="sxs-lookup"><span data-stu-id="72759-134">Value</span></span>    | <span data-ttu-id="72759-135">角色</span><span class="sxs-lookup"><span data-stu-id="72759-135">Role</span></span>     | <span data-ttu-id="72759-136">说明</span><span class="sxs-lookup"><span data-stu-id="72759-136">Description</span></span>
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | <span data-ttu-id="72759-137">可查看共享链接，允许只读访问。</span><span class="sxs-lookup"><span data-stu-id="72759-137">A view-only sharing link, allowing read-only access.</span></span>
| `edit`   | `write`  | <span data-ttu-id="72759-138">授予读写权限的编辑共享链接。</span><span class="sxs-lookup"><span data-stu-id="72759-138">An edit sharing link, allowing read-write access.</span></span>
| `embed`  | `read`   | <span data-ttu-id="72759-139">可用于将内容嵌入托管网页的仅供查看共享链接。</span><span class="sxs-lookup"><span data-stu-id="72759-139">A view-only sharing link that can be used to embed content into a host webpage.</span></span> <span data-ttu-id="72759-140">OneDrive for Business 或 SharePoint 不支持嵌入链接。</span><span class="sxs-lookup"><span data-stu-id="72759-140">Embed links are not available for OneDrive for Business or SharePoint.</span></span>

### <a name="scope-options"></a><span data-ttu-id="72759-141">作用域选项</span><span class="sxs-lookup"><span data-stu-id="72759-141">Scope options</span></span>

<span data-ttu-id="72759-142">下表定义的**范围**属性的可能值。</span><span class="sxs-lookup"><span data-stu-id="72759-142">The following table defines the possible values for the **scope** property.</span></span>

| <span data-ttu-id="72759-143">值</span><span class="sxs-lookup"><span data-stu-id="72759-143">Value</span></span>            | <span data-ttu-id="72759-144">说明</span><span class="sxs-lookup"><span data-stu-id="72759-144">Description</span></span>
|:-----------------|:------------------------------------------------------------
| `anonymous`      | <span data-ttu-id="72759-145">带链接的任何人都访问，而无需登录。</span><span class="sxs-lookup"><span data-stu-id="72759-145">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="72759-146">这可能包括您的组织外部的人员。</span><span class="sxs-lookup"><span data-stu-id="72759-146">This may include people outside of your organization.</span></span>
| `organization`   | <span data-ttu-id="72759-147">登录到您的组织 （租户） 的任何人都可以使用以下链接获取的访问权限。</span><span class="sxs-lookup"><span data-stu-id="72759-147">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="72759-148">仅在 OneDrive for Business 和 SharePoint 中可用。</span><span class="sxs-lookup"><span data-stu-id="72759-148">Only available in OneDrive for Business and SharePoint.</span></span>
| `existingAccess` | <span data-ttu-id="72759-149">仅已被授予访问通过其他手段项的人员可以访问使用此链接的项目。</span><span class="sxs-lookup"><span data-stu-id="72759-149">Only people who have already been granted access to the item through other means can access the item using this link.</span></span> <span data-ttu-id="72759-150">仅在 OneDrive for Business 和 SharePoint 中可用。</span><span class="sxs-lookup"><span data-stu-id="72759-150">Only available in OneDrive for Business and SharePoint.</span></span>
| `users`          | <span data-ttu-id="72759-151">链接授予仅对特定列表的人员的访问权限。</span><span class="sxs-lookup"><span data-stu-id="72759-151">The link grants access only to a specific list of people.</span></span> <span data-ttu-id="72759-152">仅在 OneDrive for Business 和 SharePoint 中可用。</span><span class="sxs-lookup"><span data-stu-id="72759-152">Only available in OneDrive for Business and SharePoint.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharinglink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
