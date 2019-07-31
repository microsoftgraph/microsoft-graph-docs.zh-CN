---
title: sectionGroup 资源类型
description: OneNote 笔记本中的分区组。 节组可以包含节和节组。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 4637784ac20d92c82e7a4771c815136ddd3e175a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965269"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="37196-104">sectionGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="37196-104">sectionGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37196-105">OneNote 笔记本中的分区组。</span><span class="sxs-lookup"><span data-stu-id="37196-105">A section group in a OneNote notebook.</span></span> <span data-ttu-id="37196-106">节组可以包含节和节组。</span><span class="sxs-lookup"><span data-stu-id="37196-106">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="37196-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37196-107">JSON representation</span></span>

<span data-ttu-id="37196-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37196-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="37196-109">属性</span><span class="sxs-lookup"><span data-stu-id="37196-109">Properties</span></span>
| <span data-ttu-id="37196-110">属性</span><span class="sxs-lookup"><span data-stu-id="37196-110">Property</span></span>     | <span data-ttu-id="37196-111">类型</span><span class="sxs-lookup"><span data-stu-id="37196-111">Type</span></span>   |<span data-ttu-id="37196-112">说明</span><span class="sxs-lookup"><span data-stu-id="37196-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37196-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="37196-113">createdBy</span></span>|[<span data-ttu-id="37196-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="37196-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="37196-p103">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="37196-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="37196-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37196-117">createdDateTime</span></span>|<span data-ttu-id="37196-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37196-118">DateTimeOffset</span></span>|<span data-ttu-id="37196-119">节组的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="37196-119">The date and time when the section group was created.</span></span> <span data-ttu-id="37196-120">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="37196-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="37196-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="37196-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="37196-122">只读。</span><span class="sxs-lookup"><span data-stu-id="37196-122">Read-only.</span></span>|
|<span data-ttu-id="37196-123">id</span><span class="sxs-lookup"><span data-stu-id="37196-123">id</span></span>|<span data-ttu-id="37196-124">String</span><span class="sxs-lookup"><span data-stu-id="37196-124">String</span></span>|<span data-ttu-id="37196-125">节组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="37196-125">The unique identifier of the section group.</span></span> <span data-ttu-id="37196-126">只读。</span><span class="sxs-lookup"><span data-stu-id="37196-126">Read-only.</span></span>|
|<span data-ttu-id="37196-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="37196-127">lastModifiedBy</span></span>|[<span data-ttu-id="37196-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="37196-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="37196-p106">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="37196-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="37196-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37196-131">lastModifiedDateTime</span></span>|<span data-ttu-id="37196-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37196-132">DateTimeOffset</span></span>|<span data-ttu-id="37196-133">上次修改节组的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="37196-133">The date and time when the section group was last modified.</span></span> <span data-ttu-id="37196-134">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="37196-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="37196-135">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="37196-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="37196-136">只读。</span><span class="sxs-lookup"><span data-stu-id="37196-136">Read-only.</span></span>|
|<span data-ttu-id="37196-137">displayName</span><span class="sxs-lookup"><span data-stu-id="37196-137">displayName</span></span>|<span data-ttu-id="37196-138">String</span><span class="sxs-lookup"><span data-stu-id="37196-138">String</span></span>|<span data-ttu-id="37196-139">节组的名称。</span><span class="sxs-lookup"><span data-stu-id="37196-139">The name of the section group.</span></span>|
|<span data-ttu-id="37196-140">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="37196-140">sectionGroupsUrl</span></span>|<span data-ttu-id="37196-141">String</span><span class="sxs-lookup"><span data-stu-id="37196-141">String</span></span>|<span data-ttu-id="37196-142">`sectionGroups`导航属性的 URL, 该 URL 返回节组中的所有节组。</span><span class="sxs-lookup"><span data-stu-id="37196-142">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="37196-143">只读。</span><span class="sxs-lookup"><span data-stu-id="37196-143">Read-only.</span></span>|
|<span data-ttu-id="37196-144">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="37196-144">sectionsUrl</span></span>|<span data-ttu-id="37196-145">String</span><span class="sxs-lookup"><span data-stu-id="37196-145">String</span></span>|<span data-ttu-id="37196-146">`sections`导航属性的 URL, 该 URL 返回节组中的所有节。</span><span class="sxs-lookup"><span data-stu-id="37196-146">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="37196-147">只读。</span><span class="sxs-lookup"><span data-stu-id="37196-147">Read-only.</span></span>|
|<span data-ttu-id="37196-148">自学</span><span class="sxs-lookup"><span data-stu-id="37196-148">self</span></span>|<span data-ttu-id="37196-149">String</span><span class="sxs-lookup"><span data-stu-id="37196-149">String</span></span>|<span data-ttu-id="37196-150">终结点，您可在此处获取关于节组的详细信息。</span><span class="sxs-lookup"><span data-stu-id="37196-150">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="37196-151">只读。</span><span class="sxs-lookup"><span data-stu-id="37196-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37196-152">关系</span><span class="sxs-lookup"><span data-stu-id="37196-152">Relationships</span></span>
| <span data-ttu-id="37196-153">关系</span><span class="sxs-lookup"><span data-stu-id="37196-153">Relationship</span></span> | <span data-ttu-id="37196-154">类型</span><span class="sxs-lookup"><span data-stu-id="37196-154">Type</span></span>   |<span data-ttu-id="37196-155">说明</span><span class="sxs-lookup"><span data-stu-id="37196-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37196-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="37196-156">parentNotebook</span></span>|[<span data-ttu-id="37196-157">笔记</span><span class="sxs-lookup"><span data-stu-id="37196-157">notebook</span></span>](notebook.md)|<span data-ttu-id="37196-158">包含分区组的笔记本。</span><span class="sxs-lookup"><span data-stu-id="37196-158">The notebook that contains the section group.</span></span> <span data-ttu-id="37196-159">只读。</span><span class="sxs-lookup"><span data-stu-id="37196-159">Read-only.</span></span>|
|<span data-ttu-id="37196-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="37196-160">parentSectionGroup</span></span>|[<span data-ttu-id="37196-161">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="37196-161">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="37196-162">包含节组的节组。</span><span class="sxs-lookup"><span data-stu-id="37196-162">The section group that contains the section group.</span></span> <span data-ttu-id="37196-163">只读。</span><span class="sxs-lookup"><span data-stu-id="37196-163">Read-only.</span></span>|
|<span data-ttu-id="37196-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="37196-164">sectionGroups</span></span>|<span data-ttu-id="37196-165">[sectionGroup](sectiongroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="37196-165">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="37196-166">节中的节组。</span><span class="sxs-lookup"><span data-stu-id="37196-166">The section groups in the section.</span></span> <span data-ttu-id="37196-167">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="37196-167">Read-only.</span></span> <span data-ttu-id="37196-168">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="37196-168">Nullable.</span></span>|
|<span data-ttu-id="37196-169">sections</span><span class="sxs-lookup"><span data-stu-id="37196-169">sections</span></span>|<span data-ttu-id="37196-170">[onenoteSection](onenotesection.md)集合</span><span class="sxs-lookup"><span data-stu-id="37196-170">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="37196-171">分区组中的节。</span><span class="sxs-lookup"><span data-stu-id="37196-171">The sections in the section group.</span></span> <span data-ttu-id="37196-172">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="37196-172">Read-only.</span></span> <span data-ttu-id="37196-173">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="37196-173">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="37196-174">方法</span><span class="sxs-lookup"><span data-stu-id="37196-174">Methods</span></span>

| <span data-ttu-id="37196-175">方法</span><span class="sxs-lookup"><span data-stu-id="37196-175">Method</span></span>           | <span data-ttu-id="37196-176">返回类型</span><span class="sxs-lookup"><span data-stu-id="37196-176">Return Type</span></span>    |<span data-ttu-id="37196-177">说明</span><span class="sxs-lookup"><span data-stu-id="37196-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="37196-178">获取分区组</span><span class="sxs-lookup"><span data-stu-id="37196-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="37196-179">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="37196-179">sectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="37196-180">读取分区组的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="37196-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="37196-181">创建分区组</span><span class="sxs-lookup"><span data-stu-id="37196-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="37196-182">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="37196-182">sectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="37196-183">通过发布到指定分区组中的 sectionGroups 集合创建分区组。</span><span class="sxs-lookup"><span data-stu-id="37196-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="37196-184">列出分区组</span><span class="sxs-lookup"><span data-stu-id="37196-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="37196-185">[sectionGroup](sectiongroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="37196-185">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="37196-186">获取指定分区组中的分区组的集合。</span><span class="sxs-lookup"><span data-stu-id="37196-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="37196-187">创建分区</span><span class="sxs-lookup"><span data-stu-id="37196-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="37196-188">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="37196-188">onenoteSection</span></span>](onenotesection.md)| <span data-ttu-id="37196-189">通过发布到指定分区组中的节集合来创建节。</span><span class="sxs-lookup"><span data-stu-id="37196-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="37196-190">列出节</span><span class="sxs-lookup"><span data-stu-id="37196-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="37196-191">[onenoteSection](onenotesection.md)集合</span><span class="sxs-lookup"><span data-stu-id="37196-191">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="37196-192">获取指定分区组中的节的集合。</span><span class="sxs-lookup"><span data-stu-id="37196-192">Get a collection of sections in the specified section group.</span></span>|

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
