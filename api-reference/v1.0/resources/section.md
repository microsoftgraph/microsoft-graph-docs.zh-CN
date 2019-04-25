---
title: 部分资源类型
description: OneNote 笔记本中的分区。 分区可包含页面。
localization_priority: Normal
ms.openlocfilehash: f9cb5a8e3ddf9cf4a045103e4ecc7909653d797c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579154"
---
# <a name="section-resource-type"></a><span data-ttu-id="d445e-104">部分资源类型</span><span class="sxs-lookup"><span data-stu-id="d445e-104">section resource type</span></span>

<span data-ttu-id="d445e-105">OneNote 笔记本中的分区。</span><span class="sxs-lookup"><span data-stu-id="d445e-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="d445e-106">分区可包含页面。</span><span class="sxs-lookup"><span data-stu-id="d445e-106">Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d445e-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d445e-107">JSON representation</span></span>

<span data-ttu-id="d445e-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d445e-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="d445e-109">属性</span><span class="sxs-lookup"><span data-stu-id="d445e-109">Properties</span></span>
| <span data-ttu-id="d445e-110">属性</span><span class="sxs-lookup"><span data-stu-id="d445e-110">Property</span></span>     | <span data-ttu-id="d445e-111">类型</span><span class="sxs-lookup"><span data-stu-id="d445e-111">Type</span></span>   |<span data-ttu-id="d445e-112">说明</span><span class="sxs-lookup"><span data-stu-id="d445e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d445e-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="d445e-113">createdBy</span></span>|[<span data-ttu-id="d445e-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="d445e-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="d445e-p103">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="d445e-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="d445e-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d445e-117">createdDateTime</span></span>|<span data-ttu-id="d445e-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d445e-118">DateTimeOffset</span></span>|<span data-ttu-id="d445e-119">节的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d445e-119">The date and time when the section was created.</span></span> <span data-ttu-id="d445e-120">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d445e-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d445e-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="d445e-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d445e-122">只读。</span><span class="sxs-lookup"><span data-stu-id="d445e-122">Read-only.</span></span>|
|<span data-ttu-id="d445e-123">id</span><span class="sxs-lookup"><span data-stu-id="d445e-123">id</span></span>|<span data-ttu-id="d445e-124">String</span><span class="sxs-lookup"><span data-stu-id="d445e-124">String</span></span>|<span data-ttu-id="d445e-125">节的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d445e-125">The unique identifier of the section.</span></span>  <span data-ttu-id="d445e-126">只读。</span><span class="sxs-lookup"><span data-stu-id="d445e-126">Read-only.</span></span>|
|<span data-ttu-id="d445e-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="d445e-127">isDefault</span></span>|<span data-ttu-id="d445e-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="d445e-128">Boolean</span></span>|<span data-ttu-id="d445e-129">指示是否为用户的默认节。</span><span class="sxs-lookup"><span data-stu-id="d445e-129">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="d445e-130">只读。</span><span class="sxs-lookup"><span data-stu-id="d445e-130">Read-only.</span></span>|
|<span data-ttu-id="d445e-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d445e-131">lastModifiedBy</span></span>|[<span data-ttu-id="d445e-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="d445e-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="d445e-p107">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="d445e-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="d445e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d445e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d445e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d445e-136">DateTimeOffset</span></span>|<span data-ttu-id="d445e-137">上次修改节的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d445e-137">The date and time when the section was last modified.</span></span> <span data-ttu-id="d445e-138">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d445e-138">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d445e-139">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="d445e-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d445e-140">只读。</span><span class="sxs-lookup"><span data-stu-id="d445e-140">Read-only.</span></span>|
|<span data-ttu-id="d445e-141">links</span><span class="sxs-lookup"><span data-stu-id="d445e-141">links</span></span>|[<span data-ttu-id="d445e-142">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="d445e-142">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="d445e-143">用于打开分区的链接。</span><span class="sxs-lookup"><span data-stu-id="d445e-143">Links for opening the section.</span></span> <span data-ttu-id="d445e-144">如果`oneNoteClientURL`安装了 OneNote 本机客户端, 则链接将在其中打开分区。</span><span class="sxs-lookup"><span data-stu-id="d445e-144">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="d445e-145">`oneNoteWebURL`链接将在 OneNote Online 中打开分区。</span><span class="sxs-lookup"><span data-stu-id="d445e-145">The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="d445e-146">displayName</span><span class="sxs-lookup"><span data-stu-id="d445e-146">displayName</span></span>|<span data-ttu-id="d445e-147">String</span><span class="sxs-lookup"><span data-stu-id="d445e-147">String</span></span>|<span data-ttu-id="d445e-148">节的名称。</span><span class="sxs-lookup"><span data-stu-id="d445e-148">The name of the section.</span></span> |
|<span data-ttu-id="d445e-149">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="d445e-149">pagesUrl</span></span>|<span data-ttu-id="d445e-150">String</span><span class="sxs-lookup"><span data-stu-id="d445e-150">String</span></span>|<span data-ttu-id="d445e-151">`pages`终结点, 您可在其中获取该部分中所有页面的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d445e-151">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="d445e-152">只读。</span><span class="sxs-lookup"><span data-stu-id="d445e-152">Read-only.</span></span>|
|<span data-ttu-id="d445e-153">自学</span><span class="sxs-lookup"><span data-stu-id="d445e-153">self</span></span>|<span data-ttu-id="d445e-154">String</span><span class="sxs-lookup"><span data-stu-id="d445e-154">String</span></span>|<span data-ttu-id="d445e-155">终结点，您可在此处获取关于节的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d445e-155">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="d445e-156">只读。</span><span class="sxs-lookup"><span data-stu-id="d445e-156">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d445e-157">关系</span><span class="sxs-lookup"><span data-stu-id="d445e-157">Relationships</span></span>
| <span data-ttu-id="d445e-158">关系</span><span class="sxs-lookup"><span data-stu-id="d445e-158">Relationship</span></span> | <span data-ttu-id="d445e-159">类型</span><span class="sxs-lookup"><span data-stu-id="d445e-159">Type</span></span>   |<span data-ttu-id="d445e-160">说明</span><span class="sxs-lookup"><span data-stu-id="d445e-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d445e-161">pages</span><span class="sxs-lookup"><span data-stu-id="d445e-161">pages</span></span>|<span data-ttu-id="d445e-162">[OnenotePage](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="d445e-162">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="d445e-163">分区中的一组页面。</span><span class="sxs-lookup"><span data-stu-id="d445e-163">The collection of pages in the section.</span></span>  <span data-ttu-id="d445e-164">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="d445e-164">Read-only.</span></span> <span data-ttu-id="d445e-165">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d445e-165">Nullable.</span></span>|
|<span data-ttu-id="d445e-166">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="d445e-166">parentNotebook</span></span>|[<span data-ttu-id="d445e-167">Notebook</span><span class="sxs-lookup"><span data-stu-id="d445e-167">Notebook</span></span>](notebook.md)|<span data-ttu-id="d445e-168">包含该部分的笔记本。</span><span class="sxs-lookup"><span data-stu-id="d445e-168">The notebook that contains the section.</span></span>  <span data-ttu-id="d445e-169">只读。</span><span class="sxs-lookup"><span data-stu-id="d445e-169">Read-only.</span></span>|
|<span data-ttu-id="d445e-170">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="d445e-170">parentSectionGroup</span></span>|[<span data-ttu-id="d445e-171">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="d445e-171">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="d445e-172">包含节的节组。</span><span class="sxs-lookup"><span data-stu-id="d445e-172">The section group that contains the section.</span></span>  <span data-ttu-id="d445e-173">只读的。</span><span class="sxs-lookup"><span data-stu-id="d445e-173">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="d445e-174">方法</span><span class="sxs-lookup"><span data-stu-id="d445e-174">Methods</span></span>

| <span data-ttu-id="d445e-175">方法</span><span class="sxs-lookup"><span data-stu-id="d445e-175">Method</span></span>           | <span data-ttu-id="d445e-176">返回类型</span><span class="sxs-lookup"><span data-stu-id="d445e-176">Return Type</span></span>    |<span data-ttu-id="d445e-177">说明</span><span class="sxs-lookup"><span data-stu-id="d445e-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d445e-178">获取分区</span><span class="sxs-lookup"><span data-stu-id="d445e-178">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="d445e-179">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="d445e-179">OnenoteSection</span></span>](section.md) |<span data-ttu-id="d445e-180">读取节的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d445e-180">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="d445e-181">创建页面</span><span class="sxs-lookup"><span data-stu-id="d445e-181">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="d445e-182">Page</span><span class="sxs-lookup"><span data-stu-id="d445e-182">Page</span></span>](page.md)| <span data-ttu-id="d445e-183">通过发布到指定分区中的 pages 集合来创建页面。</span><span class="sxs-lookup"><span data-stu-id="d445e-183">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="d445e-184">列出页面</span><span class="sxs-lookup"><span data-stu-id="d445e-184">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="d445e-185">[页面](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="d445e-185">[Page](page.md) collection</span></span>| <span data-ttu-id="d445e-186">获取指定节中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="d445e-186">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="d445e-187">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="d445e-187">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="d445e-188">无</span><span class="sxs-lookup"><span data-stu-id="d445e-188">None</span></span>|<span data-ttu-id="d445e-189">将分区复制到特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="d445e-189">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="d445e-190">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="d445e-190">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="d445e-191">无</span><span class="sxs-lookup"><span data-stu-id="d445e-191">None</span></span>|<span data-ttu-id="d445e-192">将分区复制到特定分区组。</span><span class="sxs-lookup"><span data-stu-id="d445e-192">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
