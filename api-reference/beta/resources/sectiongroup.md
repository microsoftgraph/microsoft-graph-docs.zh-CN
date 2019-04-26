---
title: sectionGroup 资源类型
description: OneNote 笔记本中的分区组。 节组可以包含节和节组。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 65e420d014add658a538deb42c01518cd94d611c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562877"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="31300-104">sectionGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="31300-104">sectionGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31300-105">OneNote 笔记本中的分区组。</span><span class="sxs-lookup"><span data-stu-id="31300-105">A section group in a OneNote notebook.</span></span> <span data-ttu-id="31300-106">节组可以包含节和节组。</span><span class="sxs-lookup"><span data-stu-id="31300-106">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31300-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31300-107">JSON representation</span></span>

<span data-ttu-id="31300-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31300-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectiongroup"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="31300-109">属性</span><span class="sxs-lookup"><span data-stu-id="31300-109">Properties</span></span>
| <span data-ttu-id="31300-110">属性</span><span class="sxs-lookup"><span data-stu-id="31300-110">Property</span></span>     | <span data-ttu-id="31300-111">类型</span><span class="sxs-lookup"><span data-stu-id="31300-111">Type</span></span>   |<span data-ttu-id="31300-112">说明</span><span class="sxs-lookup"><span data-stu-id="31300-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31300-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="31300-113">createdBy</span></span>|[<span data-ttu-id="31300-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="31300-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="31300-p103">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="31300-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="31300-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31300-117">createdDateTime</span></span>|<span data-ttu-id="31300-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31300-118">DateTimeOffset</span></span>|<span data-ttu-id="31300-119">节组的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="31300-119">The date and time when the section group was created.</span></span> <span data-ttu-id="31300-120">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="31300-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="31300-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="31300-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="31300-122">只读。</span><span class="sxs-lookup"><span data-stu-id="31300-122">Read-only.</span></span>|
|<span data-ttu-id="31300-123">id</span><span class="sxs-lookup"><span data-stu-id="31300-123">id</span></span>|<span data-ttu-id="31300-124">String</span><span class="sxs-lookup"><span data-stu-id="31300-124">String</span></span>|<span data-ttu-id="31300-125">节组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="31300-125">The unique identifier of the section group.</span></span> <span data-ttu-id="31300-126">只读。</span><span class="sxs-lookup"><span data-stu-id="31300-126">Read-only.</span></span>|
|<span data-ttu-id="31300-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="31300-127">lastModifiedBy</span></span>|[<span data-ttu-id="31300-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="31300-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="31300-p106">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="31300-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="31300-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31300-131">lastModifiedDateTime</span></span>|<span data-ttu-id="31300-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31300-132">DateTimeOffset</span></span>|<span data-ttu-id="31300-133">上次修改节组的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="31300-133">The date and time when the section group was last modified.</span></span> <span data-ttu-id="31300-134">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="31300-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="31300-135">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="31300-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="31300-136">只读。</span><span class="sxs-lookup"><span data-stu-id="31300-136">Read-only.</span></span>|
|<span data-ttu-id="31300-137">displayName</span><span class="sxs-lookup"><span data-stu-id="31300-137">displayName</span></span>|<span data-ttu-id="31300-138">String</span><span class="sxs-lookup"><span data-stu-id="31300-138">String</span></span>|<span data-ttu-id="31300-139">节组的名称。</span><span class="sxs-lookup"><span data-stu-id="31300-139">The name of the section group.</span></span>|
|<span data-ttu-id="31300-140">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="31300-140">sectionGroupsUrl</span></span>|<span data-ttu-id="31300-141">String</span><span class="sxs-lookup"><span data-stu-id="31300-141">String</span></span>|<span data-ttu-id="31300-142">`sectionGroups`导航属性的 URL, 该 URL 返回节组中的所有节组。</span><span class="sxs-lookup"><span data-stu-id="31300-142">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="31300-143">只读。</span><span class="sxs-lookup"><span data-stu-id="31300-143">Read-only.</span></span>|
|<span data-ttu-id="31300-144">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="31300-144">sectionsUrl</span></span>|<span data-ttu-id="31300-145">String</span><span class="sxs-lookup"><span data-stu-id="31300-145">String</span></span>|<span data-ttu-id="31300-146">`sections`导航属性的 URL, 该 URL 返回节组中的所有节。</span><span class="sxs-lookup"><span data-stu-id="31300-146">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="31300-147">只读。</span><span class="sxs-lookup"><span data-stu-id="31300-147">Read-only.</span></span>|
|<span data-ttu-id="31300-148">自学</span><span class="sxs-lookup"><span data-stu-id="31300-148">self</span></span>|<span data-ttu-id="31300-149">String</span><span class="sxs-lookup"><span data-stu-id="31300-149">String</span></span>|<span data-ttu-id="31300-150">终结点，您可在此处获取关于节组的详细信息。</span><span class="sxs-lookup"><span data-stu-id="31300-150">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="31300-151">只读。</span><span class="sxs-lookup"><span data-stu-id="31300-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31300-152">关系</span><span class="sxs-lookup"><span data-stu-id="31300-152">Relationships</span></span>
| <span data-ttu-id="31300-153">关系</span><span class="sxs-lookup"><span data-stu-id="31300-153">Relationship</span></span> | <span data-ttu-id="31300-154">类型</span><span class="sxs-lookup"><span data-stu-id="31300-154">Type</span></span>   |<span data-ttu-id="31300-155">说明</span><span class="sxs-lookup"><span data-stu-id="31300-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31300-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="31300-156">parentNotebook</span></span>|[<span data-ttu-id="31300-157">Notebook</span><span class="sxs-lookup"><span data-stu-id="31300-157">Notebook</span></span>](notebook.md)|<span data-ttu-id="31300-158">包含分区组的笔记本。</span><span class="sxs-lookup"><span data-stu-id="31300-158">The notebook that contains the section group.</span></span> <span data-ttu-id="31300-159">只读。</span><span class="sxs-lookup"><span data-stu-id="31300-159">Read-only.</span></span>|
|<span data-ttu-id="31300-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="31300-160">parentSectionGroup</span></span>|[<span data-ttu-id="31300-161">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="31300-161">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="31300-162">包含节组的节组。</span><span class="sxs-lookup"><span data-stu-id="31300-162">The section group that contains the section group.</span></span> <span data-ttu-id="31300-163">只读。</span><span class="sxs-lookup"><span data-stu-id="31300-163">Read-only.</span></span>|
|<span data-ttu-id="31300-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="31300-164">sectionGroups</span></span>|<span data-ttu-id="31300-165">[SectionGroup](sectiongroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="31300-165">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="31300-166">节中的节组。</span><span class="sxs-lookup"><span data-stu-id="31300-166">The section groups in the section.</span></span> <span data-ttu-id="31300-167">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="31300-167">Read-only.</span></span> <span data-ttu-id="31300-168">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="31300-168">Nullable.</span></span>|
|<span data-ttu-id="31300-169">分区</span><span class="sxs-lookup"><span data-stu-id="31300-169">sections</span></span>|<span data-ttu-id="31300-170">[节](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="31300-170">[Section](section.md) collection</span></span>|<span data-ttu-id="31300-171">分区组中的节。</span><span class="sxs-lookup"><span data-stu-id="31300-171">The sections in the section group.</span></span> <span data-ttu-id="31300-172">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="31300-172">Read-only.</span></span> <span data-ttu-id="31300-173">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="31300-173">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="31300-174">方法</span><span class="sxs-lookup"><span data-stu-id="31300-174">Methods</span></span>

| <span data-ttu-id="31300-175">方法</span><span class="sxs-lookup"><span data-stu-id="31300-175">Method</span></span>           | <span data-ttu-id="31300-176">返回类型</span><span class="sxs-lookup"><span data-stu-id="31300-176">Return Type</span></span>    |<span data-ttu-id="31300-177">说明</span><span class="sxs-lookup"><span data-stu-id="31300-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="31300-178">获取分区组</span><span class="sxs-lookup"><span data-stu-id="31300-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="31300-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="31300-179">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="31300-180">读取分区组的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="31300-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="31300-181">创建分区组</span><span class="sxs-lookup"><span data-stu-id="31300-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="31300-182">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="31300-182">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="31300-183">通过发布到指定分区组中的 sectionGroups 集合创建分区组。</span><span class="sxs-lookup"><span data-stu-id="31300-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="31300-184">列出分区组</span><span class="sxs-lookup"><span data-stu-id="31300-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="31300-185">[SectionGroup](sectiongroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="31300-185">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="31300-186">获取指定分区组中的分区组的集合。</span><span class="sxs-lookup"><span data-stu-id="31300-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="31300-187">创建分区</span><span class="sxs-lookup"><span data-stu-id="31300-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="31300-188">Section</span><span class="sxs-lookup"><span data-stu-id="31300-188">Section</span></span>](section.md)| <span data-ttu-id="31300-189">通过发布到指定分区组中的节集合来创建节。</span><span class="sxs-lookup"><span data-stu-id="31300-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="31300-190">列出分区</span><span class="sxs-lookup"><span data-stu-id="31300-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="31300-191">[节](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="31300-191">[Section](section.md) collection</span></span>| <span data-ttu-id="31300-192">获取指定分区组中的节的集合。</span><span class="sxs-lookup"><span data-stu-id="31300-192">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sectiongroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
