---
title: sectionGroup 资源类型
description: OneNote 笔记本中的分区组。分区组可以包含分区和分区组。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 65e420d014add658a538deb42c01518cd94d611c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523706"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="93be9-104">sectionGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="93be9-104">sectionGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93be9-p102">OneNote 笔记本中的分区组。分区组可以包含分区和分区组。</span><span class="sxs-lookup"><span data-stu-id="93be9-p102">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="93be9-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93be9-107">JSON representation</span></span>

<span data-ttu-id="93be9-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93be9-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="93be9-109">属性</span><span class="sxs-lookup"><span data-stu-id="93be9-109">Properties</span></span>
| <span data-ttu-id="93be9-110">属性</span><span class="sxs-lookup"><span data-stu-id="93be9-110">Property</span></span>     | <span data-ttu-id="93be9-111">类型</span><span class="sxs-lookup"><span data-stu-id="93be9-111">Type</span></span>   |<span data-ttu-id="93be9-112">说明</span><span class="sxs-lookup"><span data-stu-id="93be9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93be9-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="93be9-113">createdBy</span></span>|[<span data-ttu-id="93be9-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="93be9-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="93be9-p103">创建项的用户、设备和应用程序标识。只读。</span><span class="sxs-lookup"><span data-stu-id="93be9-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="93be9-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93be9-117">createdDateTime</span></span>|<span data-ttu-id="93be9-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93be9-118">DateTimeOffset</span></span>|<span data-ttu-id="93be9-p104">分区组的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="93be9-p104">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="93be9-123">id</span><span class="sxs-lookup"><span data-stu-id="93be9-123">id</span></span>|<span data-ttu-id="93be9-124">字串符号</span><span class="sxs-lookup"><span data-stu-id="93be9-124">String</span></span>|<span data-ttu-id="93be9-p105">分区组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="93be9-p105">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="93be9-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="93be9-127">lastModifiedBy</span></span>|[<span data-ttu-id="93be9-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="93be9-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="93be9-p106">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="93be9-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="93be9-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93be9-131">lastModifiedDateTime</span></span>|<span data-ttu-id="93be9-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93be9-132">DateTimeOffset</span></span>|<span data-ttu-id="93be9-p107">上次修改分区组的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="93be9-p107">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="93be9-137">displayName</span><span class="sxs-lookup"><span data-stu-id="93be9-137">displayName</span></span>|<span data-ttu-id="93be9-138">String</span><span class="sxs-lookup"><span data-stu-id="93be9-138">String</span></span>|<span data-ttu-id="93be9-139">分区组的名称。</span><span class="sxs-lookup"><span data-stu-id="93be9-139">The name of the section group.</span></span>|
|<span data-ttu-id="93be9-140">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="93be9-140">sectionGroupsUrl</span></span>|<span data-ttu-id="93be9-141">String</span><span class="sxs-lookup"><span data-stu-id="93be9-141">String</span></span>|<span data-ttu-id="93be9-p108">`sectionGroups` 导航属性的 URL，其将返回分区组中的所有分区组。只读。</span><span class="sxs-lookup"><span data-stu-id="93be9-p108">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="93be9-144">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="93be9-144">sectionsUrl</span></span>|<span data-ttu-id="93be9-145">String</span><span class="sxs-lookup"><span data-stu-id="93be9-145">String</span></span>|<span data-ttu-id="93be9-p109">`sections` 导航属性的 URL，其将返回分区组中的所有分区。只读。</span><span class="sxs-lookup"><span data-stu-id="93be9-p109">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="93be9-148">self</span><span class="sxs-lookup"><span data-stu-id="93be9-148">self</span></span>|<span data-ttu-id="93be9-149">字符串</span><span class="sxs-lookup"><span data-stu-id="93be9-149">String</span></span>|<span data-ttu-id="93be9-p110">可以在其中获取关于分区阻的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="93be9-p110">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93be9-152">关系</span><span class="sxs-lookup"><span data-stu-id="93be9-152">Relationships</span></span>
| <span data-ttu-id="93be9-153">关系</span><span class="sxs-lookup"><span data-stu-id="93be9-153">Relationship</span></span> | <span data-ttu-id="93be9-154">类型</span><span class="sxs-lookup"><span data-stu-id="93be9-154">Type</span></span>   |<span data-ttu-id="93be9-155">说明</span><span class="sxs-lookup"><span data-stu-id="93be9-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93be9-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="93be9-156">parentNotebook</span></span>|[<span data-ttu-id="93be9-157">Notebook</span><span class="sxs-lookup"><span data-stu-id="93be9-157">Notebook</span></span>](notebook.md)|<span data-ttu-id="93be9-p111">包含分区组的笔记本。只读。</span><span class="sxs-lookup"><span data-stu-id="93be9-p111">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="93be9-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="93be9-160">parentSectionGroup</span></span>|[<span data-ttu-id="93be9-161">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="93be9-161">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="93be9-p112">包含分区组的分区组。只读。</span><span class="sxs-lookup"><span data-stu-id="93be9-p112">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="93be9-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="93be9-164">sectionGroups</span></span>|<span data-ttu-id="93be9-165">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="93be9-165">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="93be9-p113">分区中的分区组。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="93be9-p113">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="93be9-169">节</span><span class="sxs-lookup"><span data-stu-id="93be9-169">sections</span></span>|<span data-ttu-id="93be9-170">[Section](section.md) collection</span><span class="sxs-lookup"><span data-stu-id="93be9-170">[Section](section.md) collection</span></span>|<span data-ttu-id="93be9-p114">分区组中的分区。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="93be9-p114">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="93be9-174">方法</span><span class="sxs-lookup"><span data-stu-id="93be9-174">Methods</span></span>

| <span data-ttu-id="93be9-175">方法</span><span class="sxs-lookup"><span data-stu-id="93be9-175">Method</span></span>           | <span data-ttu-id="93be9-176">返回类型</span><span class="sxs-lookup"><span data-stu-id="93be9-176">Return Type</span></span>    |<span data-ttu-id="93be9-177">说明</span><span class="sxs-lookup"><span data-stu-id="93be9-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="93be9-178">Get section group</span><span class="sxs-lookup"><span data-stu-id="93be9-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="93be9-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="93be9-179">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="93be9-180">读取分区组的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="93be9-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="93be9-181">Create section group</span><span class="sxs-lookup"><span data-stu-id="93be9-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="93be9-182">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="93be9-182">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="93be9-183">通过发布到指定分区组中的 sectionGroups 集合创建分区组。</span><span class="sxs-lookup"><span data-stu-id="93be9-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="93be9-184">List section groups</span><span class="sxs-lookup"><span data-stu-id="93be9-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="93be9-185">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="93be9-185">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="93be9-186">获取指定分区组中的分区组集合。</span><span class="sxs-lookup"><span data-stu-id="93be9-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="93be9-187">Create section</span><span class="sxs-lookup"><span data-stu-id="93be9-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="93be9-188">Section</span><span class="sxs-lookup"><span data-stu-id="93be9-188">Section</span></span>](section.md)| <span data-ttu-id="93be9-189">通过发布到指定分区组中的分区集合创建分区。</span><span class="sxs-lookup"><span data-stu-id="93be9-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="93be9-190">List sections</span><span class="sxs-lookup"><span data-stu-id="93be9-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="93be9-191">[Section](section.md) collection</span><span class="sxs-lookup"><span data-stu-id="93be9-191">[Section](section.md) collection</span></span>| <span data-ttu-id="93be9-192">获取指定分区组中的分区集合。</span><span class="sxs-lookup"><span data-stu-id="93be9-192">Get a collection of sections in the specified section group.</span></span>|

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
