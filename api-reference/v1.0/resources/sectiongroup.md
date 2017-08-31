# <a name="sectiongroup-resource-type"></a><span data-ttu-id="6a05d-101">sectionGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a05d-101">sectionGroup resource type</span></span>

<span data-ttu-id="6a05d-p101">OneNote 笔记本中的分区组。分区组可以包含分区和分区组。</span><span class="sxs-lookup"><span data-stu-id="6a05d-p101">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a05d-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a05d-104">JSON representation</span></span>

<span data-ttu-id="6a05d-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a05d-105">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="6a05d-106">属性</span><span class="sxs-lookup"><span data-stu-id="6a05d-106">Properties</span></span>
| <span data-ttu-id="6a05d-107">属性</span><span class="sxs-lookup"><span data-stu-id="6a05d-107">Property</span></span>     | <span data-ttu-id="6a05d-108">类型</span><span class="sxs-lookup"><span data-stu-id="6a05d-108">Type</span></span>   |<span data-ttu-id="6a05d-109">说明</span><span class="sxs-lookup"><span data-stu-id="6a05d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a05d-110">createdBy</span><span class="sxs-lookup"><span data-stu-id="6a05d-110">createdBy</span></span>|[<span data-ttu-id="6a05d-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="6a05d-111">identitySet</span></span>](identityset.md)|<span data-ttu-id="6a05d-p102">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="6a05d-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="6a05d-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a05d-114">createdDateTime</span></span>|<span data-ttu-id="6a05d-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a05d-115">DateTimeOffset</span></span>|<span data-ttu-id="6a05d-p103">分区组的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="6a05d-p103">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="6a05d-120">id</span><span class="sxs-lookup"><span data-stu-id="6a05d-120">id</span></span>|<span data-ttu-id="6a05d-121">字符串</span><span class="sxs-lookup"><span data-stu-id="6a05d-121">String</span></span>|<span data-ttu-id="6a05d-p104">分区组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="6a05d-p104">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="6a05d-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6a05d-124">lastModifiedBy</span></span>|[<span data-ttu-id="6a05d-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="6a05d-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="6a05d-p105">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="6a05d-p105">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="6a05d-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a05d-128">lastModifiedDateTime</span></span>|<span data-ttu-id="6a05d-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a05d-129">DateTimeOffset</span></span>|<span data-ttu-id="6a05d-p106">上次修改分区组的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="6a05d-p106">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="6a05d-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6a05d-134">displayName</span></span>|<span data-ttu-id="6a05d-135">String</span><span class="sxs-lookup"><span data-stu-id="6a05d-135">String</span></span>|<span data-ttu-id="6a05d-136">分区组的名称。</span><span class="sxs-lookup"><span data-stu-id="6a05d-136">The name of the section group.</span></span>|
|<span data-ttu-id="6a05d-137">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="6a05d-137">sectionGroupsUrl</span></span>|<span data-ttu-id="6a05d-138">String</span><span class="sxs-lookup"><span data-stu-id="6a05d-138">String</span></span>|<span data-ttu-id="6a05d-p107">`sectionGroups` 导航属性的 URL，其将返回分区组中的所有分区组。只读。</span><span class="sxs-lookup"><span data-stu-id="6a05d-p107">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="6a05d-141">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="6a05d-141">sectionsUrl</span></span>|<span data-ttu-id="6a05d-142">String</span><span class="sxs-lookup"><span data-stu-id="6a05d-142">String</span></span>|<span data-ttu-id="6a05d-p108">`sections` 导航属性的 URL，其将返回分区组中的所有分区。只读。</span><span class="sxs-lookup"><span data-stu-id="6a05d-p108">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="6a05d-145">self</span><span class="sxs-lookup"><span data-stu-id="6a05d-145">self</span></span>|<span data-ttu-id="6a05d-146">字符串</span><span class="sxs-lookup"><span data-stu-id="6a05d-146">String</span></span>|<span data-ttu-id="6a05d-p109">可以在其中获取关于分区阻的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="6a05d-p109">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a05d-149">关系</span><span class="sxs-lookup"><span data-stu-id="6a05d-149">Relationships</span></span>
| <span data-ttu-id="6a05d-150">关系</span><span class="sxs-lookup"><span data-stu-id="6a05d-150">Relationship</span></span> | <span data-ttu-id="6a05d-151">类型</span><span class="sxs-lookup"><span data-stu-id="6a05d-151">Type</span></span>   |<span data-ttu-id="6a05d-152">说明</span><span class="sxs-lookup"><span data-stu-id="6a05d-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a05d-153">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="6a05d-153">parentNotebook</span></span>|[<span data-ttu-id="6a05d-154">Notebook</span><span class="sxs-lookup"><span data-stu-id="6a05d-154">Notebook</span></span>](notebook.md)|<span data-ttu-id="6a05d-p110">包含分区组的笔记本。只读。</span><span class="sxs-lookup"><span data-stu-id="6a05d-p110">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="6a05d-157">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="6a05d-157">parentSectionGroup</span></span>|[<span data-ttu-id="6a05d-158">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="6a05d-158">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="6a05d-p111">包含分区组的分区组。只读。</span><span class="sxs-lookup"><span data-stu-id="6a05d-p111">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="6a05d-161">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="6a05d-161">sectionGroups</span></span>|<span data-ttu-id="6a05d-162">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="6a05d-162">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="6a05d-p112">分区中的分区组。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="6a05d-p112">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6a05d-166">节</span><span class="sxs-lookup"><span data-stu-id="6a05d-166">sections</span></span>|<span data-ttu-id="6a05d-167">[Section](section.md) collection</span><span class="sxs-lookup"><span data-stu-id="6a05d-167">[Section](section.md) collection</span></span>|<span data-ttu-id="6a05d-p113">分区组中的分区。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="6a05d-p113">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="6a05d-171">方法</span><span class="sxs-lookup"><span data-stu-id="6a05d-171">Methods</span></span>

| <span data-ttu-id="6a05d-172">方法</span><span class="sxs-lookup"><span data-stu-id="6a05d-172">Method</span></span>           | <span data-ttu-id="6a05d-173">返回类型</span><span class="sxs-lookup"><span data-stu-id="6a05d-173">Return Type</span></span>    |<span data-ttu-id="6a05d-174">说明</span><span class="sxs-lookup"><span data-stu-id="6a05d-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6a05d-175">Get section group</span><span class="sxs-lookup"><span data-stu-id="6a05d-175">Get section group</span></span>](../api/sectiongroup_get.md) | [<span data-ttu-id="6a05d-176">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="6a05d-176">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="6a05d-177">读取分区组的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6a05d-177">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="6a05d-178">Create section group</span><span class="sxs-lookup"><span data-stu-id="6a05d-178">Create section group</span></span>](../api/sectiongroup_post_sectiongroups.md) |[<span data-ttu-id="6a05d-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="6a05d-179">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="6a05d-180">通过发布到指定分区组中的 sectionGroups 集合创建分区组。</span><span class="sxs-lookup"><span data-stu-id="6a05d-180">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="6a05d-181">List section groups</span><span class="sxs-lookup"><span data-stu-id="6a05d-181">List section groups</span></span>](../api/sectiongroup_list_sectiongroups.md) |<span data-ttu-id="6a05d-182">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="6a05d-182">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="6a05d-183">获取指定分区组中的分区组集合。</span><span class="sxs-lookup"><span data-stu-id="6a05d-183">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="6a05d-184">Create section</span><span class="sxs-lookup"><span data-stu-id="6a05d-184">Create section</span></span>](../api/sectiongroup_post_sections.md) |[<span data-ttu-id="6a05d-185">Section</span><span class="sxs-lookup"><span data-stu-id="6a05d-185">Section</span></span>](section.md)| <span data-ttu-id="6a05d-186">通过发布到指定分区组中的分区集合创建分区。</span><span class="sxs-lookup"><span data-stu-id="6a05d-186">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="6a05d-187">List sections</span><span class="sxs-lookup"><span data-stu-id="6a05d-187">List sections</span></span>](../api/sectiongroup_list_sections.md) |<span data-ttu-id="6a05d-188">[Section](section.md) collection</span><span class="sxs-lookup"><span data-stu-id="6a05d-188">[Section](section.md) collection</span></span>| <span data-ttu-id="6a05d-189">获取指定分区组中的分区集合。</span><span class="sxs-lookup"><span data-stu-id="6a05d-189">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
