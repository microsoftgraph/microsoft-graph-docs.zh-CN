---
title: sectionGroup 资源类型
description: OneNote 笔记本中的分区组。 节组可以包含节和节组。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: dee2ca947af83f81f482ad280d0ae0c77b69fc56
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087626"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="aa296-104">sectionGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa296-104">sectionGroup resource type</span></span>

<span data-ttu-id="aa296-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa296-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa296-106">OneNote 笔记本中的分区组。</span><span class="sxs-lookup"><span data-stu-id="aa296-106">A section group in a OneNote notebook.</span></span> <span data-ttu-id="aa296-107">节组可以包含节和节组。</span><span class="sxs-lookup"><span data-stu-id="aa296-107">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa296-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa296-108">JSON representation</span></span>

<span data-ttu-id="aa296-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa296-109">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "keyProperty": "id",
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
## <a name="properties"></a><span data-ttu-id="aa296-110">属性</span><span class="sxs-lookup"><span data-stu-id="aa296-110">Properties</span></span>
| <span data-ttu-id="aa296-111">属性</span><span class="sxs-lookup"><span data-stu-id="aa296-111">Property</span></span>     | <span data-ttu-id="aa296-112">类型</span><span class="sxs-lookup"><span data-stu-id="aa296-112">Type</span></span>   |<span data-ttu-id="aa296-113">说明</span><span class="sxs-lookup"><span data-stu-id="aa296-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa296-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="aa296-114">createdBy</span></span>|[<span data-ttu-id="aa296-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="aa296-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="aa296-p103">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="aa296-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="aa296-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa296-118">createdDateTime</span></span>|<span data-ttu-id="aa296-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa296-119">DateTimeOffset</span></span>|<span data-ttu-id="aa296-120">节组的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="aa296-120">The date and time when the section group was created.</span></span> <span data-ttu-id="aa296-121">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="aa296-121">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aa296-122">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="aa296-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="aa296-123">只读。</span><span class="sxs-lookup"><span data-stu-id="aa296-123">Read-only.</span></span>|
|<span data-ttu-id="aa296-124">id</span><span class="sxs-lookup"><span data-stu-id="aa296-124">id</span></span>|<span data-ttu-id="aa296-125">字符串</span><span class="sxs-lookup"><span data-stu-id="aa296-125">String</span></span>|<span data-ttu-id="aa296-126">节组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aa296-126">The unique identifier of the section group.</span></span> <span data-ttu-id="aa296-127">只读。</span><span class="sxs-lookup"><span data-stu-id="aa296-127">Read-only.</span></span>|
|<span data-ttu-id="aa296-128">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="aa296-128">lastModifiedBy</span></span>|[<span data-ttu-id="aa296-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="aa296-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="aa296-p106">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="aa296-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="aa296-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa296-132">lastModifiedDateTime</span></span>|<span data-ttu-id="aa296-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa296-133">DateTimeOffset</span></span>|<span data-ttu-id="aa296-134">上次修改节组的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="aa296-134">The date and time when the section group was last modified.</span></span> <span data-ttu-id="aa296-135">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="aa296-135">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aa296-136">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="aa296-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="aa296-137">只读。</span><span class="sxs-lookup"><span data-stu-id="aa296-137">Read-only.</span></span>|
|<span data-ttu-id="aa296-138">displayName</span><span class="sxs-lookup"><span data-stu-id="aa296-138">displayName</span></span>|<span data-ttu-id="aa296-139">字符串</span><span class="sxs-lookup"><span data-stu-id="aa296-139">String</span></span>|<span data-ttu-id="aa296-140">节组的名称。</span><span class="sxs-lookup"><span data-stu-id="aa296-140">The name of the section group.</span></span>|
|<span data-ttu-id="aa296-141">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="aa296-141">sectionGroupsUrl</span></span>|<span data-ttu-id="aa296-142">字符串</span><span class="sxs-lookup"><span data-stu-id="aa296-142">String</span></span>|<span data-ttu-id="aa296-143">导航属性的 URL `sectionGroups` ，该 URL 返回节组中的所有节组。</span><span class="sxs-lookup"><span data-stu-id="aa296-143">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="aa296-144">只读。</span><span class="sxs-lookup"><span data-stu-id="aa296-144">Read-only.</span></span>|
|<span data-ttu-id="aa296-145">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="aa296-145">sectionsUrl</span></span>|<span data-ttu-id="aa296-146">字符串</span><span class="sxs-lookup"><span data-stu-id="aa296-146">String</span></span>|<span data-ttu-id="aa296-147">导航属性的 URL `sections` ，该 URL 返回节组中的所有节。</span><span class="sxs-lookup"><span data-stu-id="aa296-147">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="aa296-148">只读。</span><span class="sxs-lookup"><span data-stu-id="aa296-148">Read-only.</span></span>|
|<span data-ttu-id="aa296-149">自学</span><span class="sxs-lookup"><span data-stu-id="aa296-149">self</span></span>|<span data-ttu-id="aa296-150">字符串</span><span class="sxs-lookup"><span data-stu-id="aa296-150">String</span></span>|<span data-ttu-id="aa296-151">终结点，您可在此处获取关于节组的详细信息。</span><span class="sxs-lookup"><span data-stu-id="aa296-151">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="aa296-152">只读。</span><span class="sxs-lookup"><span data-stu-id="aa296-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa296-153">关系</span><span class="sxs-lookup"><span data-stu-id="aa296-153">Relationships</span></span>
| <span data-ttu-id="aa296-154">关系</span><span class="sxs-lookup"><span data-stu-id="aa296-154">Relationship</span></span> | <span data-ttu-id="aa296-155">类型</span><span class="sxs-lookup"><span data-stu-id="aa296-155">Type</span></span>   |<span data-ttu-id="aa296-156">说明</span><span class="sxs-lookup"><span data-stu-id="aa296-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa296-157">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="aa296-157">parentNotebook</span></span>|[<span data-ttu-id="aa296-158">笔记本</span><span class="sxs-lookup"><span data-stu-id="aa296-158">notebook</span></span>](notebook.md)|<span data-ttu-id="aa296-159">包含分区组的笔记本。</span><span class="sxs-lookup"><span data-stu-id="aa296-159">The notebook that contains the section group.</span></span> <span data-ttu-id="aa296-160">只读。</span><span class="sxs-lookup"><span data-stu-id="aa296-160">Read-only.</span></span>|
|<span data-ttu-id="aa296-161">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="aa296-161">parentSectionGroup</span></span>|[<span data-ttu-id="aa296-162">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="aa296-162">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="aa296-163">包含节组的节组。</span><span class="sxs-lookup"><span data-stu-id="aa296-163">The section group that contains the section group.</span></span> <span data-ttu-id="aa296-164">只读。</span><span class="sxs-lookup"><span data-stu-id="aa296-164">Read-only.</span></span>|
|<span data-ttu-id="aa296-165">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="aa296-165">sectionGroups</span></span>|<span data-ttu-id="aa296-166">[sectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa296-166">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="aa296-167">节中的节组。</span><span class="sxs-lookup"><span data-stu-id="aa296-167">The section groups in the section.</span></span> <span data-ttu-id="aa296-168">只读。</span><span class="sxs-lookup"><span data-stu-id="aa296-168">Read-only.</span></span> <span data-ttu-id="aa296-169">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="aa296-169">Nullable.</span></span>|
|<span data-ttu-id="aa296-170">sections</span><span class="sxs-lookup"><span data-stu-id="aa296-170">sections</span></span>|<span data-ttu-id="aa296-171">[onenoteSection](onenotesection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa296-171">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="aa296-172">分区组中的节。</span><span class="sxs-lookup"><span data-stu-id="aa296-172">The sections in the section group.</span></span> <span data-ttu-id="aa296-173">只读。</span><span class="sxs-lookup"><span data-stu-id="aa296-173">Read-only.</span></span> <span data-ttu-id="aa296-174">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="aa296-174">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="aa296-175">方法</span><span class="sxs-lookup"><span data-stu-id="aa296-175">Methods</span></span>

| <span data-ttu-id="aa296-176">方法</span><span class="sxs-lookup"><span data-stu-id="aa296-176">Method</span></span>           | <span data-ttu-id="aa296-177">返回类型</span><span class="sxs-lookup"><span data-stu-id="aa296-177">Return Type</span></span>    |<span data-ttu-id="aa296-178">说明</span><span class="sxs-lookup"><span data-stu-id="aa296-178">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aa296-179">获取分区组</span><span class="sxs-lookup"><span data-stu-id="aa296-179">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="aa296-180">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="aa296-180">sectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="aa296-181">读取分区组的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aa296-181">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="aa296-182">创建分区组</span><span class="sxs-lookup"><span data-stu-id="aa296-182">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="aa296-183">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="aa296-183">sectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="aa296-184">通过发布到指定分区组中的 sectionGroups 集合创建分区组。</span><span class="sxs-lookup"><span data-stu-id="aa296-184">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="aa296-185">列出分区组</span><span class="sxs-lookup"><span data-stu-id="aa296-185">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="aa296-186">[sectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa296-186">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="aa296-187">获取指定分区组中的分区组的集合。</span><span class="sxs-lookup"><span data-stu-id="aa296-187">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="aa296-188">创建分区</span><span class="sxs-lookup"><span data-stu-id="aa296-188">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="aa296-189">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="aa296-189">onenoteSection</span></span>](onenotesection.md)| <span data-ttu-id="aa296-190">通过发布到指定分区组中的节集合来创建节。</span><span class="sxs-lookup"><span data-stu-id="aa296-190">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="aa296-191">列出节</span><span class="sxs-lookup"><span data-stu-id="aa296-191">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="aa296-192">[onenoteSection](onenotesection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa296-192">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="aa296-193">获取指定分区组中的节的集合。</span><span class="sxs-lookup"><span data-stu-id="aa296-193">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


