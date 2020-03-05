---
title: sectionGroup 资源类型
description: OneNote 笔记本中的分区组。 节组可以包含节和节组。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 2e0d9b3b963e02bf017630ad898501518449a20f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446938"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="0fc2c-104">sectionGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fc2c-104">sectionGroup resource type</span></span>

<span data-ttu-id="0fc2c-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0fc2c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0fc2c-106">OneNote 笔记本中的分区组。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-106">A section group in a OneNote notebook.</span></span> <span data-ttu-id="0fc2c-107">节组可以包含节和节组。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-107">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fc2c-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fc2c-108">JSON representation</span></span>

<span data-ttu-id="0fc2c-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-109">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="0fc2c-110">属性</span><span class="sxs-lookup"><span data-stu-id="0fc2c-110">Properties</span></span>
| <span data-ttu-id="0fc2c-111">属性</span><span class="sxs-lookup"><span data-stu-id="0fc2c-111">Property</span></span>     | <span data-ttu-id="0fc2c-112">类型</span><span class="sxs-lookup"><span data-stu-id="0fc2c-112">Type</span></span>   |<span data-ttu-id="0fc2c-113">说明</span><span class="sxs-lookup"><span data-stu-id="0fc2c-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fc2c-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="0fc2c-114">createdBy</span></span>|[<span data-ttu-id="0fc2c-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="0fc2c-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="0fc2c-p103">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="0fc2c-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fc2c-118">createdDateTime</span></span>|<span data-ttu-id="0fc2c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fc2c-119">DateTimeOffset</span></span>|<span data-ttu-id="0fc2c-120">节组的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-120">The date and time when the section group was created.</span></span> <span data-ttu-id="0fc2c-121">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-121">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0fc2c-122">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0fc2c-123">只读。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-123">Read-only.</span></span>|
|<span data-ttu-id="0fc2c-124">id</span><span class="sxs-lookup"><span data-stu-id="0fc2c-124">id</span></span>|<span data-ttu-id="0fc2c-125">String</span><span class="sxs-lookup"><span data-stu-id="0fc2c-125">String</span></span>|<span data-ttu-id="0fc2c-126">节组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-126">The unique identifier of the section group.</span></span> <span data-ttu-id="0fc2c-127">只读。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-127">Read-only.</span></span>|
|<span data-ttu-id="0fc2c-128">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="0fc2c-128">lastModifiedBy</span></span>|[<span data-ttu-id="0fc2c-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="0fc2c-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="0fc2c-p106">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="0fc2c-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fc2c-132">lastModifiedDateTime</span></span>|<span data-ttu-id="0fc2c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fc2c-133">DateTimeOffset</span></span>|<span data-ttu-id="0fc2c-134">上次修改节组的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-134">The date and time when the section group was last modified.</span></span> <span data-ttu-id="0fc2c-135">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-135">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0fc2c-136">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0fc2c-137">只读。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-137">Read-only.</span></span>|
|<span data-ttu-id="0fc2c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0fc2c-138">displayName</span></span>|<span data-ttu-id="0fc2c-139">String</span><span class="sxs-lookup"><span data-stu-id="0fc2c-139">String</span></span>|<span data-ttu-id="0fc2c-140">节组的名称。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-140">The name of the section group.</span></span>|
|<span data-ttu-id="0fc2c-141">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="0fc2c-141">sectionGroupsUrl</span></span>|<span data-ttu-id="0fc2c-142">String</span><span class="sxs-lookup"><span data-stu-id="0fc2c-142">String</span></span>|<span data-ttu-id="0fc2c-143">`sectionGroups`导航属性的 URL，该 URL 返回节组中的所有节组。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-143">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="0fc2c-144">只读。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-144">Read-only.</span></span>|
|<span data-ttu-id="0fc2c-145">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="0fc2c-145">sectionsUrl</span></span>|<span data-ttu-id="0fc2c-146">String</span><span class="sxs-lookup"><span data-stu-id="0fc2c-146">String</span></span>|<span data-ttu-id="0fc2c-147">`sections`导航属性的 URL，该 URL 返回节组中的所有节。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-147">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="0fc2c-148">只读。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-148">Read-only.</span></span>|
|<span data-ttu-id="0fc2c-149">自学</span><span class="sxs-lookup"><span data-stu-id="0fc2c-149">self</span></span>|<span data-ttu-id="0fc2c-150">String</span><span class="sxs-lookup"><span data-stu-id="0fc2c-150">String</span></span>|<span data-ttu-id="0fc2c-151">终结点，您可在此处获取关于节组的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-151">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="0fc2c-152">只读。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fc2c-153">关系</span><span class="sxs-lookup"><span data-stu-id="0fc2c-153">Relationships</span></span>
| <span data-ttu-id="0fc2c-154">关系</span><span class="sxs-lookup"><span data-stu-id="0fc2c-154">Relationship</span></span> | <span data-ttu-id="0fc2c-155">类型</span><span class="sxs-lookup"><span data-stu-id="0fc2c-155">Type</span></span>   |<span data-ttu-id="0fc2c-156">说明</span><span class="sxs-lookup"><span data-stu-id="0fc2c-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fc2c-157">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="0fc2c-157">parentNotebook</span></span>|[<span data-ttu-id="0fc2c-158">笔记本</span><span class="sxs-lookup"><span data-stu-id="0fc2c-158">Notebook</span></span>](notebook.md)|<span data-ttu-id="0fc2c-159">包含分区组的笔记本。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-159">The notebook that contains the section group.</span></span> <span data-ttu-id="0fc2c-160">只读。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-160">Read-only.</span></span>|
|<span data-ttu-id="0fc2c-161">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="0fc2c-161">parentSectionGroup</span></span>|[<span data-ttu-id="0fc2c-162">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="0fc2c-162">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="0fc2c-163">包含节组的节组。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-163">The section group that contains the section group.</span></span> <span data-ttu-id="0fc2c-164">只读。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-164">Read-only.</span></span>|
|<span data-ttu-id="0fc2c-165">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="0fc2c-165">sectionGroups</span></span>|<span data-ttu-id="0fc2c-166">[SectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fc2c-166">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="0fc2c-167">节中的节组。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-167">The section groups in the section.</span></span> <span data-ttu-id="0fc2c-168">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-168">Read-only.</span></span> <span data-ttu-id="0fc2c-169">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-169">Nullable.</span></span>|
|<span data-ttu-id="0fc2c-170">sections</span><span class="sxs-lookup"><span data-stu-id="0fc2c-170">sections</span></span>|<span data-ttu-id="0fc2c-171">[OnenoteSection](section.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fc2c-171">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="0fc2c-172">分区组中的节。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-172">The sections in the section group.</span></span> <span data-ttu-id="0fc2c-173">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-173">Read-only.</span></span> <span data-ttu-id="0fc2c-174">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-174">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="0fc2c-175">方法</span><span class="sxs-lookup"><span data-stu-id="0fc2c-175">Methods</span></span>

| <span data-ttu-id="0fc2c-176">方法</span><span class="sxs-lookup"><span data-stu-id="0fc2c-176">Method</span></span>           | <span data-ttu-id="0fc2c-177">返回类型</span><span class="sxs-lookup"><span data-stu-id="0fc2c-177">Return Type</span></span>    |<span data-ttu-id="0fc2c-178">说明</span><span class="sxs-lookup"><span data-stu-id="0fc2c-178">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0fc2c-179">获取分区组</span><span class="sxs-lookup"><span data-stu-id="0fc2c-179">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="0fc2c-180">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="0fc2c-180">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="0fc2c-181">读取分区组的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-181">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="0fc2c-182">创建分区组</span><span class="sxs-lookup"><span data-stu-id="0fc2c-182">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="0fc2c-183">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="0fc2c-183">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="0fc2c-184">通过发布到指定分区组中的 sectionGroups 集合创建分区组。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-184">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="0fc2c-185">列出分区组</span><span class="sxs-lookup"><span data-stu-id="0fc2c-185">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="0fc2c-186">[SectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fc2c-186">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="0fc2c-187">获取指定分区组中的分区组的集合。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-187">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="0fc2c-188">创建分区</span><span class="sxs-lookup"><span data-stu-id="0fc2c-188">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="0fc2c-189">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="0fc2c-189">OnenoteSection</span></span>](section.md)| <span data-ttu-id="0fc2c-190">通过发布到指定分区组中的节集合来创建节。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-190">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="0fc2c-191">列出节</span><span class="sxs-lookup"><span data-stu-id="0fc2c-191">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="0fc2c-192">[OnenoteSection](section.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fc2c-192">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="0fc2c-193">获取指定分区组中的节的集合。</span><span class="sxs-lookup"><span data-stu-id="0fc2c-193">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
