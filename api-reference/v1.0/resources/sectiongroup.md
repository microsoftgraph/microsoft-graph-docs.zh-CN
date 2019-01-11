---
title: sectionGroup 资源类型
description: OneNote 笔记本中的分区组。分区组可以包含分区和分区组。
localization_priority: Normal
ms.openlocfilehash: f204c5422eb5f0f2580bfbed82ed28306dd0618f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806305"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="0097e-104">sectionGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="0097e-104">sectionGroup resource type</span></span>

<span data-ttu-id="0097e-p102">OneNote 笔记本中的分区组。分区组可以包含分区和分区组。</span><span class="sxs-lookup"><span data-stu-id="0097e-p102">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0097e-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0097e-107">JSON representation</span></span>

<span data-ttu-id="0097e-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0097e-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectionGroup"
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
## <a name="properties"></a><span data-ttu-id="0097e-109">属性</span><span class="sxs-lookup"><span data-stu-id="0097e-109">Properties</span></span>
| <span data-ttu-id="0097e-110">属性</span><span class="sxs-lookup"><span data-stu-id="0097e-110">Property</span></span>     | <span data-ttu-id="0097e-111">类型</span><span class="sxs-lookup"><span data-stu-id="0097e-111">Type</span></span>   |<span data-ttu-id="0097e-112">说明</span><span class="sxs-lookup"><span data-stu-id="0097e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0097e-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="0097e-113">createdBy</span></span>|[<span data-ttu-id="0097e-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="0097e-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="0097e-p103">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="0097e-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="0097e-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0097e-117">createdDateTime</span></span>|<span data-ttu-id="0097e-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0097e-118">DateTimeOffset</span></span>|<span data-ttu-id="0097e-p104">分区组的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="0097e-p104">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="0097e-123">id</span><span class="sxs-lookup"><span data-stu-id="0097e-123">id</span></span>|<span data-ttu-id="0097e-124">字符串</span><span class="sxs-lookup"><span data-stu-id="0097e-124">String</span></span>|<span data-ttu-id="0097e-p105">分区组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="0097e-p105">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="0097e-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="0097e-127">lastModifiedBy</span></span>|[<span data-ttu-id="0097e-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="0097e-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="0097e-p106">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="0097e-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="0097e-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0097e-131">lastModifiedDateTime</span></span>|<span data-ttu-id="0097e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0097e-132">DateTimeOffset</span></span>|<span data-ttu-id="0097e-p107">上次修改分区组的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="0097e-p107">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="0097e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0097e-137">displayName</span></span>|<span data-ttu-id="0097e-138">String</span><span class="sxs-lookup"><span data-stu-id="0097e-138">String</span></span>|<span data-ttu-id="0097e-139">分区组的名称。</span><span class="sxs-lookup"><span data-stu-id="0097e-139">The name of the section group.</span></span>|
|<span data-ttu-id="0097e-140">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="0097e-140">sectionGroupsUrl</span></span>|<span data-ttu-id="0097e-141">String</span><span class="sxs-lookup"><span data-stu-id="0097e-141">String</span></span>|<span data-ttu-id="0097e-p108">`sectionGroups` 导航属性的 URL，其将返回分区组中的所有分区组。只读。</span><span class="sxs-lookup"><span data-stu-id="0097e-p108">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="0097e-144">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="0097e-144">sectionsUrl</span></span>|<span data-ttu-id="0097e-145">String</span><span class="sxs-lookup"><span data-stu-id="0097e-145">String</span></span>|<span data-ttu-id="0097e-p109">`sections` 导航属性的 URL，其将返回分区组中的所有分区。只读。</span><span class="sxs-lookup"><span data-stu-id="0097e-p109">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="0097e-148">self</span><span class="sxs-lookup"><span data-stu-id="0097e-148">self</span></span>|<span data-ttu-id="0097e-149">字符串</span><span class="sxs-lookup"><span data-stu-id="0097e-149">String</span></span>|<span data-ttu-id="0097e-p110">可以在其中获取关于分区阻的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="0097e-p110">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0097e-152">关系</span><span class="sxs-lookup"><span data-stu-id="0097e-152">Relationships</span></span>
| <span data-ttu-id="0097e-153">关系</span><span class="sxs-lookup"><span data-stu-id="0097e-153">Relationship</span></span> | <span data-ttu-id="0097e-154">类型</span><span class="sxs-lookup"><span data-stu-id="0097e-154">Type</span></span>   |<span data-ttu-id="0097e-155">说明</span><span class="sxs-lookup"><span data-stu-id="0097e-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0097e-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="0097e-156">parentNotebook</span></span>|[<span data-ttu-id="0097e-157">Notebook</span><span class="sxs-lookup"><span data-stu-id="0097e-157">Notebook</span></span>](notebook.md)|<span data-ttu-id="0097e-p111">包含分区组的笔记本。只读。</span><span class="sxs-lookup"><span data-stu-id="0097e-p111">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="0097e-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="0097e-160">parentSectionGroup</span></span>|[<span data-ttu-id="0097e-161">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="0097e-161">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="0097e-p112">包含分区组的分区组。只读。</span><span class="sxs-lookup"><span data-stu-id="0097e-p112">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="0097e-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="0097e-164">sectionGroups</span></span>|<span data-ttu-id="0097e-165">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="0097e-165">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="0097e-p113">分区中的分区组。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="0097e-p113">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="0097e-169">sections</span><span class="sxs-lookup"><span data-stu-id="0097e-169">sections</span></span>|<span data-ttu-id="0097e-170">[OnenoteSection](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="0097e-170">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="0097e-p114">分区组中的分区。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="0097e-p114">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="0097e-174">方法</span><span class="sxs-lookup"><span data-stu-id="0097e-174">Methods</span></span>

| <span data-ttu-id="0097e-175">方法</span><span class="sxs-lookup"><span data-stu-id="0097e-175">Method</span></span>           | <span data-ttu-id="0097e-176">返回类型</span><span class="sxs-lookup"><span data-stu-id="0097e-176">Return Type</span></span>    |<span data-ttu-id="0097e-177">说明</span><span class="sxs-lookup"><span data-stu-id="0097e-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0097e-178">Get section group</span><span class="sxs-lookup"><span data-stu-id="0097e-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="0097e-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="0097e-179">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="0097e-180">读取分区组的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0097e-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="0097e-181">Create section group</span><span class="sxs-lookup"><span data-stu-id="0097e-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="0097e-182">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="0097e-182">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="0097e-183">通过发布到指定分区组中的 sectionGroups 集合创建分区组。</span><span class="sxs-lookup"><span data-stu-id="0097e-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="0097e-184">List section groups</span><span class="sxs-lookup"><span data-stu-id="0097e-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="0097e-185">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="0097e-185">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="0097e-186">获取指定分区组中的分区组集合。</span><span class="sxs-lookup"><span data-stu-id="0097e-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="0097e-187">Create section</span><span class="sxs-lookup"><span data-stu-id="0097e-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="0097e-188">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="0097e-188">OnenoteSection</span></span>](section.md)| <span data-ttu-id="0097e-189">通过发布到指定分区组中的分区集合创建分区。</span><span class="sxs-lookup"><span data-stu-id="0097e-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="0097e-190">List sections</span><span class="sxs-lookup"><span data-stu-id="0097e-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="0097e-191">[OnenoteSection](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="0097e-191">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="0097e-192">获取指定分区组中的分区集合。</span><span class="sxs-lookup"><span data-stu-id="0097e-192">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
