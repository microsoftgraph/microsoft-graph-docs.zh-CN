---
title: sectionGroup 资源类型
description: OneNote 笔记本中的节组。 节组可以包含节和节组。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 6e52b922b9e882121ab926ca02f94089f9f55a0a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719344"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="a0da0-104">sectionGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0da0-104">sectionGroup resource type</span></span>

<span data-ttu-id="a0da0-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0da0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0da0-106">OneNote 笔记本中的节组。</span><span class="sxs-lookup"><span data-stu-id="a0da0-106">A section group in a OneNote notebook.</span></span> <span data-ttu-id="a0da0-107">节组可以包含节和节组。</span><span class="sxs-lookup"><span data-stu-id="a0da0-107">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0da0-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0da0-108">JSON representation</span></span>

<span data-ttu-id="a0da0-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0da0-109">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a0da0-110">属性</span><span class="sxs-lookup"><span data-stu-id="a0da0-110">Properties</span></span>
| <span data-ttu-id="a0da0-111">属性</span><span class="sxs-lookup"><span data-stu-id="a0da0-111">Property</span></span>     | <span data-ttu-id="a0da0-112">类型</span><span class="sxs-lookup"><span data-stu-id="a0da0-112">Type</span></span>   |<span data-ttu-id="a0da0-113">说明</span><span class="sxs-lookup"><span data-stu-id="a0da0-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0da0-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="a0da0-114">createdBy</span></span>|[<span data-ttu-id="a0da0-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="a0da0-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="a0da0-p103">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="a0da0-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="a0da0-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0da0-118">createdDateTime</span></span>|<span data-ttu-id="a0da0-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0da0-119">DateTimeOffset</span></span>|<span data-ttu-id="a0da0-120">节组的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a0da0-120">The date and time when the section group was created.</span></span> <span data-ttu-id="a0da0-121">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="a0da0-121">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a0da0-122">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="a0da0-122">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="a0da0-123">只读。</span><span class="sxs-lookup"><span data-stu-id="a0da0-123">Read-only.</span></span>|
|<span data-ttu-id="a0da0-124">id</span><span class="sxs-lookup"><span data-stu-id="a0da0-124">id</span></span>|<span data-ttu-id="a0da0-125">String</span><span class="sxs-lookup"><span data-stu-id="a0da0-125">String</span></span>|<span data-ttu-id="a0da0-126">节组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a0da0-126">The unique identifier of the section group.</span></span> <span data-ttu-id="a0da0-127">只读。</span><span class="sxs-lookup"><span data-stu-id="a0da0-127">Read-only.</span></span>|
|<span data-ttu-id="a0da0-128">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a0da0-128">lastModifiedBy</span></span>|[<span data-ttu-id="a0da0-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="a0da0-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="a0da0-p106">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="a0da0-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="a0da0-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0da0-132">lastModifiedDateTime</span></span>|<span data-ttu-id="a0da0-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0da0-133">DateTimeOffset</span></span>|<span data-ttu-id="a0da0-134">上次修改节组的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a0da0-134">The date and time when the section group was last modified.</span></span> <span data-ttu-id="a0da0-135">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="a0da0-135">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a0da0-136">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="a0da0-136">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="a0da0-137">只读。</span><span class="sxs-lookup"><span data-stu-id="a0da0-137">Read-only.</span></span>|
|<span data-ttu-id="a0da0-138">displayName</span><span class="sxs-lookup"><span data-stu-id="a0da0-138">displayName</span></span>|<span data-ttu-id="a0da0-139">String</span><span class="sxs-lookup"><span data-stu-id="a0da0-139">String</span></span>|<span data-ttu-id="a0da0-140">节组的名称。</span><span class="sxs-lookup"><span data-stu-id="a0da0-140">The name of the section group.</span></span>|
|<span data-ttu-id="a0da0-141">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="a0da0-141">sectionGroupsUrl</span></span>|<span data-ttu-id="a0da0-142">String</span><span class="sxs-lookup"><span data-stu-id="a0da0-142">String</span></span>|<span data-ttu-id="a0da0-143">导航属性的 `sectionGroups` URL，该属性返回节组的所有节组。</span><span class="sxs-lookup"><span data-stu-id="a0da0-143">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="a0da0-144">只读。</span><span class="sxs-lookup"><span data-stu-id="a0da0-144">Read-only.</span></span>|
|<span data-ttu-id="a0da0-145">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="a0da0-145">sectionsUrl</span></span>|<span data-ttu-id="a0da0-146">String</span><span class="sxs-lookup"><span data-stu-id="a0da0-146">String</span></span>|<span data-ttu-id="a0da0-147">导航属性的 `sections` URL，该属性返回节组中的所有节。</span><span class="sxs-lookup"><span data-stu-id="a0da0-147">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="a0da0-148">只读。</span><span class="sxs-lookup"><span data-stu-id="a0da0-148">Read-only.</span></span>|
|<span data-ttu-id="a0da0-149">self</span><span class="sxs-lookup"><span data-stu-id="a0da0-149">self</span></span>|<span data-ttu-id="a0da0-150">String</span><span class="sxs-lookup"><span data-stu-id="a0da0-150">String</span></span>|<span data-ttu-id="a0da0-151">终结点，您可在此处获取关于节组的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a0da0-151">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="a0da0-152">只读。</span><span class="sxs-lookup"><span data-stu-id="a0da0-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0da0-153">关系</span><span class="sxs-lookup"><span data-stu-id="a0da0-153">Relationships</span></span>
| <span data-ttu-id="a0da0-154">关系</span><span class="sxs-lookup"><span data-stu-id="a0da0-154">Relationship</span></span> | <span data-ttu-id="a0da0-155">类型</span><span class="sxs-lookup"><span data-stu-id="a0da0-155">Type</span></span>   |<span data-ttu-id="a0da0-156">说明</span><span class="sxs-lookup"><span data-stu-id="a0da0-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0da0-157">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="a0da0-157">parentNotebook</span></span>|[<span data-ttu-id="a0da0-158">笔记本</span><span class="sxs-lookup"><span data-stu-id="a0da0-158">notebook</span></span>](notebook.md)|<span data-ttu-id="a0da0-159">包含分区组的笔记本。</span><span class="sxs-lookup"><span data-stu-id="a0da0-159">The notebook that contains the section group.</span></span> <span data-ttu-id="a0da0-160">只读。</span><span class="sxs-lookup"><span data-stu-id="a0da0-160">Read-only.</span></span>|
|<span data-ttu-id="a0da0-161">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="a0da0-161">parentSectionGroup</span></span>|[<span data-ttu-id="a0da0-162">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="a0da0-162">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="a0da0-163">包含节组的节组。</span><span class="sxs-lookup"><span data-stu-id="a0da0-163">The section group that contains the section group.</span></span> <span data-ttu-id="a0da0-164">只读。</span><span class="sxs-lookup"><span data-stu-id="a0da0-164">Read-only.</span></span>|
|<span data-ttu-id="a0da0-165">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="a0da0-165">sectionGroups</span></span>|<span data-ttu-id="a0da0-166">[sectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a0da0-166">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="a0da0-167">分区中的节组。</span><span class="sxs-lookup"><span data-stu-id="a0da0-167">The section groups in the section.</span></span> <span data-ttu-id="a0da0-168">只读。</span><span class="sxs-lookup"><span data-stu-id="a0da0-168">Read-only.</span></span> <span data-ttu-id="a0da0-169">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="a0da0-169">Nullable.</span></span>|
|<span data-ttu-id="a0da0-170">sections</span><span class="sxs-lookup"><span data-stu-id="a0da0-170">sections</span></span>|<span data-ttu-id="a0da0-171">[onenoteSection](onenotesection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a0da0-171">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="a0da0-172">分区组中的各个部分。</span><span class="sxs-lookup"><span data-stu-id="a0da0-172">The sections in the section group.</span></span> <span data-ttu-id="a0da0-173">只读。</span><span class="sxs-lookup"><span data-stu-id="a0da0-173">Read-only.</span></span> <span data-ttu-id="a0da0-174">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a0da0-174">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="a0da0-175">方法</span><span class="sxs-lookup"><span data-stu-id="a0da0-175">Methods</span></span>

| <span data-ttu-id="a0da0-176">方法</span><span class="sxs-lookup"><span data-stu-id="a0da0-176">Method</span></span>           | <span data-ttu-id="a0da0-177">返回类型</span><span class="sxs-lookup"><span data-stu-id="a0da0-177">Return Type</span></span>    |<span data-ttu-id="a0da0-178">说明</span><span class="sxs-lookup"><span data-stu-id="a0da0-178">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a0da0-179">获取分区组</span><span class="sxs-lookup"><span data-stu-id="a0da0-179">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="a0da0-180">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="a0da0-180">sectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="a0da0-181">读取节组的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a0da0-181">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="a0da0-182">创建分区组</span><span class="sxs-lookup"><span data-stu-id="a0da0-182">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="a0da0-183">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="a0da0-183">sectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="a0da0-184">通过发布到指定节组的 sectionGroups 集合来创建节组。</span><span class="sxs-lookup"><span data-stu-id="a0da0-184">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="a0da0-185">列出分区组</span><span class="sxs-lookup"><span data-stu-id="a0da0-185">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="a0da0-186">[sectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a0da0-186">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="a0da0-187">获取指定节组中节组的集合。</span><span class="sxs-lookup"><span data-stu-id="a0da0-187">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="a0da0-188">创建分区</span><span class="sxs-lookup"><span data-stu-id="a0da0-188">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="a0da0-189">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="a0da0-189">onenoteSection</span></span>](onenotesection.md)| <span data-ttu-id="a0da0-190">通过发布到指定节组中的节集合来创建节。</span><span class="sxs-lookup"><span data-stu-id="a0da0-190">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="a0da0-191">列出节</span><span class="sxs-lookup"><span data-stu-id="a0da0-191">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="a0da0-192">[onenoteSection](onenotesection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a0da0-192">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="a0da0-193">获取指定节组中节的集合。</span><span class="sxs-lookup"><span data-stu-id="a0da0-193">Get a collection of sections in the specified section group.</span></span>|

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


