---
title: sectionGroup 资源类型
description: OneNote 笔记本中的分区组。分区组可以包含分区和分区组。
ms.openlocfilehash: e27f3f468d660b2ffe778a46078054751ed8063e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048332"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="6c64e-104">sectionGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c64e-104">sectionGroup resource type</span></span>

> <span data-ttu-id="6c64e-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6c64e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c64e-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6c64e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c64e-p103">OneNote 笔记本中的分区组。分区组可以包含分区和分区组。</span><span class="sxs-lookup"><span data-stu-id="6c64e-p103">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c64e-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c64e-109">JSON representation</span></span>

<span data-ttu-id="6c64e-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c64e-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="6c64e-111">属性</span><span class="sxs-lookup"><span data-stu-id="6c64e-111">Properties</span></span>
| <span data-ttu-id="6c64e-112">属性</span><span class="sxs-lookup"><span data-stu-id="6c64e-112">Property</span></span>     | <span data-ttu-id="6c64e-113">类型</span><span class="sxs-lookup"><span data-stu-id="6c64e-113">Type</span></span>   |<span data-ttu-id="6c64e-114">说明</span><span class="sxs-lookup"><span data-stu-id="6c64e-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c64e-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="6c64e-115">createdBy</span></span>|[<span data-ttu-id="6c64e-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="6c64e-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="6c64e-p104">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="6c64e-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="6c64e-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c64e-119">createdDateTime</span></span>|<span data-ttu-id="6c64e-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c64e-120">DateTimeOffset</span></span>|<span data-ttu-id="6c64e-p105">分区组的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="6c64e-p105">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="6c64e-125">id</span><span class="sxs-lookup"><span data-stu-id="6c64e-125">id</span></span>|<span data-ttu-id="6c64e-126">字符串</span><span class="sxs-lookup"><span data-stu-id="6c64e-126">String</span></span>|<span data-ttu-id="6c64e-p106">分区组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="6c64e-p106">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="6c64e-129">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6c64e-129">lastModifiedBy</span></span>|[<span data-ttu-id="6c64e-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="6c64e-130">identitySet</span></span>](identityset.md)|<span data-ttu-id="6c64e-p107">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="6c64e-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="6c64e-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c64e-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6c64e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c64e-134">DateTimeOffset</span></span>|<span data-ttu-id="6c64e-p108">上次修改分区组的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="6c64e-p108">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="6c64e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="6c64e-139">displayName</span></span>|<span data-ttu-id="6c64e-140">String</span><span class="sxs-lookup"><span data-stu-id="6c64e-140">String</span></span>|<span data-ttu-id="6c64e-141">分区组的名称。</span><span class="sxs-lookup"><span data-stu-id="6c64e-141">The name of the section group.</span></span>|
|<span data-ttu-id="6c64e-142">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="6c64e-142">sectionGroupsUrl</span></span>|<span data-ttu-id="6c64e-143">String</span><span class="sxs-lookup"><span data-stu-id="6c64e-143">String</span></span>|<span data-ttu-id="6c64e-p109">`sectionGroups` 导航属性的 URL，其将返回分区组中的所有分区组。只读。</span><span class="sxs-lookup"><span data-stu-id="6c64e-p109">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="6c64e-146">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="6c64e-146">sectionsUrl</span></span>|<span data-ttu-id="6c64e-147">String</span><span class="sxs-lookup"><span data-stu-id="6c64e-147">String</span></span>|<span data-ttu-id="6c64e-p110">`sections` 导航属性的 URL，其将返回分区组中的所有分区。只读。</span><span class="sxs-lookup"><span data-stu-id="6c64e-p110">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="6c64e-150">self</span><span class="sxs-lookup"><span data-stu-id="6c64e-150">self</span></span>|<span data-ttu-id="6c64e-151">字符串</span><span class="sxs-lookup"><span data-stu-id="6c64e-151">String</span></span>|<span data-ttu-id="6c64e-p111">可以在其中获取关于分区阻的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="6c64e-p111">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c64e-154">关系</span><span class="sxs-lookup"><span data-stu-id="6c64e-154">Relationships</span></span>
| <span data-ttu-id="6c64e-155">关系</span><span class="sxs-lookup"><span data-stu-id="6c64e-155">Relationship</span></span> | <span data-ttu-id="6c64e-156">类型</span><span class="sxs-lookup"><span data-stu-id="6c64e-156">Type</span></span>   |<span data-ttu-id="6c64e-157">说明</span><span class="sxs-lookup"><span data-stu-id="6c64e-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c64e-158">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="6c64e-158">parentNotebook</span></span>|[<span data-ttu-id="6c64e-159">Notebook</span><span class="sxs-lookup"><span data-stu-id="6c64e-159">Notebook</span></span>](notebook.md)|<span data-ttu-id="6c64e-p112">包含分区组的笔记本。只读。</span><span class="sxs-lookup"><span data-stu-id="6c64e-p112">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="6c64e-162">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="6c64e-162">parentSectionGroup</span></span>|[<span data-ttu-id="6c64e-163">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="6c64e-163">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="6c64e-p113">包含分区组的分区组。只读。</span><span class="sxs-lookup"><span data-stu-id="6c64e-p113">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="6c64e-166">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="6c64e-166">sectionGroups</span></span>|<span data-ttu-id="6c64e-167">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="6c64e-167">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="6c64e-p114">分区中的分区组。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="6c64e-p114">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6c64e-171">节</span><span class="sxs-lookup"><span data-stu-id="6c64e-171">sections</span></span>|<span data-ttu-id="6c64e-172">[Section](section.md) collection</span><span class="sxs-lookup"><span data-stu-id="6c64e-172">[Section](section.md) collection</span></span>|<span data-ttu-id="6c64e-p115">分区组中的分区。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="6c64e-p115">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="6c64e-176">方法</span><span class="sxs-lookup"><span data-stu-id="6c64e-176">Methods</span></span>

| <span data-ttu-id="6c64e-177">方法</span><span class="sxs-lookup"><span data-stu-id="6c64e-177">Method</span></span>           | <span data-ttu-id="6c64e-178">返回类型</span><span class="sxs-lookup"><span data-stu-id="6c64e-178">Return Type</span></span>    |<span data-ttu-id="6c64e-179">说明</span><span class="sxs-lookup"><span data-stu-id="6c64e-179">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c64e-180">Get section group</span><span class="sxs-lookup"><span data-stu-id="6c64e-180">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="6c64e-181">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="6c64e-181">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="6c64e-182">读取分区组的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6c64e-182">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="6c64e-183">Create section group</span><span class="sxs-lookup"><span data-stu-id="6c64e-183">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="6c64e-184">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="6c64e-184">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="6c64e-185">通过发布到指定分区组中的 sectionGroups 集合创建分区组。</span><span class="sxs-lookup"><span data-stu-id="6c64e-185">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="6c64e-186">List section groups</span><span class="sxs-lookup"><span data-stu-id="6c64e-186">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="6c64e-187">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="6c64e-187">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="6c64e-188">获取指定分区组中的分区组集合。</span><span class="sxs-lookup"><span data-stu-id="6c64e-188">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="6c64e-189">Create section</span><span class="sxs-lookup"><span data-stu-id="6c64e-189">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="6c64e-190">Section</span><span class="sxs-lookup"><span data-stu-id="6c64e-190">Section</span></span>](section.md)| <span data-ttu-id="6c64e-191">通过发布到指定分区组中的分区集合创建分区。</span><span class="sxs-lookup"><span data-stu-id="6c64e-191">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="6c64e-192">List sections</span><span class="sxs-lookup"><span data-stu-id="6c64e-192">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="6c64e-193">[Section](section.md) collection</span><span class="sxs-lookup"><span data-stu-id="6c64e-193">[Section](section.md) collection</span></span>| <span data-ttu-id="6c64e-194">获取指定分区组中的分区集合。</span><span class="sxs-lookup"><span data-stu-id="6c64e-194">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
