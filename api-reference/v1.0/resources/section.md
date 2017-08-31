# <a name="section-resource-type"></a><span data-ttu-id="0ac1b-101">section 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ac1b-101">section resource type</span></span>

<span data-ttu-id="0ac1b-p101">OneNote 笔记本中的分区。分区可包含页面。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-p101">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ac1b-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ac1b-104">JSON representation</span></span>

<span data-ttu-id="0ac1b-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
## <a name="properties"></a><span data-ttu-id="0ac1b-106">属性</span><span class="sxs-lookup"><span data-stu-id="0ac1b-106">Properties</span></span>
| <span data-ttu-id="0ac1b-107">属性</span><span class="sxs-lookup"><span data-stu-id="0ac1b-107">Property</span></span>     | <span data-ttu-id="0ac1b-108">类型</span><span class="sxs-lookup"><span data-stu-id="0ac1b-108">Type</span></span>   |<span data-ttu-id="0ac1b-109">说明</span><span class="sxs-lookup"><span data-stu-id="0ac1b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ac1b-110">createdBy</span><span class="sxs-lookup"><span data-stu-id="0ac1b-110">createdBy</span></span>|[<span data-ttu-id="0ac1b-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="0ac1b-111">identitySet</span></span>](identityset.md)|<span data-ttu-id="0ac1b-p102">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="0ac1b-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ac1b-114">createdDateTime</span></span>|<span data-ttu-id="0ac1b-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ac1b-115">DateTimeOffset</span></span>|<span data-ttu-id="0ac1b-p103">分区的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-p103">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="0ac1b-120">id</span><span class="sxs-lookup"><span data-stu-id="0ac1b-120">id</span></span>|<span data-ttu-id="0ac1b-121">字符串</span><span class="sxs-lookup"><span data-stu-id="0ac1b-121">String</span></span>|<span data-ttu-id="0ac1b-p104">分区的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-p104">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="0ac1b-124">isDefault</span><span class="sxs-lookup"><span data-stu-id="0ac1b-124">isDefault</span></span>|<span data-ttu-id="0ac1b-125">布尔</span><span class="sxs-lookup"><span data-stu-id="0ac1b-125">Boolean</span></span>|<span data-ttu-id="0ac1b-p105">指示其是否是用户的默认分区。只读。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-p105">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="0ac1b-128">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="0ac1b-128">lastModifiedBy</span></span>|[<span data-ttu-id="0ac1b-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="0ac1b-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="0ac1b-p106">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="0ac1b-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ac1b-132">lastModifiedDateTime</span></span>|<span data-ttu-id="0ac1b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ac1b-133">DateTimeOffset</span></span>|<span data-ttu-id="0ac1b-p107">上次修改分区的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-p107">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="0ac1b-138">links</span><span class="sxs-lookup"><span data-stu-id="0ac1b-138">links</span></span>|[<span data-ttu-id="0ac1b-139">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="0ac1b-139">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="0ac1b-p108">用于打开分区的链接。如果安装了 OneNote 本机客户端，则 `oneNoteClientURL` 链接将在其中打开分区。`oneNoteWebURL` 将在 OneNote Online 中打开分区。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-p108">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="0ac1b-143">displayName</span><span class="sxs-lookup"><span data-stu-id="0ac1b-143">displayName</span></span>|<span data-ttu-id="0ac1b-144">String</span><span class="sxs-lookup"><span data-stu-id="0ac1b-144">String</span></span>|<span data-ttu-id="0ac1b-145">分区名称。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-145">The name of the section.</span></span> |
|<span data-ttu-id="0ac1b-146">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="0ac1b-146">pagesUrl</span></span>|<span data-ttu-id="0ac1b-147">String</span><span class="sxs-lookup"><span data-stu-id="0ac1b-147">String</span></span>|<span data-ttu-id="0ac1b-p109">可以在其中获取分区中所有页面的详细信息的 `pages` 终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-p109">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="0ac1b-150">self</span><span class="sxs-lookup"><span data-stu-id="0ac1b-150">self</span></span>|<span data-ttu-id="0ac1b-151">字符串</span><span class="sxs-lookup"><span data-stu-id="0ac1b-151">String</span></span>|<span data-ttu-id="0ac1b-p110">可以在其中获取关于分区的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-p110">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ac1b-154">关系</span><span class="sxs-lookup"><span data-stu-id="0ac1b-154">Relationships</span></span>
| <span data-ttu-id="0ac1b-155">关系</span><span class="sxs-lookup"><span data-stu-id="0ac1b-155">Relationship</span></span> | <span data-ttu-id="0ac1b-156">类型</span><span class="sxs-lookup"><span data-stu-id="0ac1b-156">Type</span></span>   |<span data-ttu-id="0ac1b-157">说明</span><span class="sxs-lookup"><span data-stu-id="0ac1b-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ac1b-158">pages</span><span class="sxs-lookup"><span data-stu-id="0ac1b-158">pages</span></span>|<span data-ttu-id="0ac1b-159">[Page](page.md) collection</span><span class="sxs-lookup"><span data-stu-id="0ac1b-159">[Page](page.md) collection</span></span>|<span data-ttu-id="0ac1b-p111">分区中的页面集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-p111">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="0ac1b-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="0ac1b-163">parentNotebook</span></span>|[<span data-ttu-id="0ac1b-164">Notebook</span><span class="sxs-lookup"><span data-stu-id="0ac1b-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="0ac1b-p112">包含分区的笔记本。只读。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-p112">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="0ac1b-167">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="0ac1b-167">parentSectionGroup</span></span>|[<span data-ttu-id="0ac1b-168">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="0ac1b-168">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="0ac1b-p113">包含分区的分区组。只读。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-p113">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="0ac1b-171">方法</span><span class="sxs-lookup"><span data-stu-id="0ac1b-171">Methods</span></span>

| <span data-ttu-id="0ac1b-172">方法</span><span class="sxs-lookup"><span data-stu-id="0ac1b-172">Method</span></span>           | <span data-ttu-id="0ac1b-173">返回类型</span><span class="sxs-lookup"><span data-stu-id="0ac1b-173">Return Type</span></span>    |<span data-ttu-id="0ac1b-174">说明</span><span class="sxs-lookup"><span data-stu-id="0ac1b-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0ac1b-175">Get section</span><span class="sxs-lookup"><span data-stu-id="0ac1b-175">Get section</span></span>](../api/section_get.md) | [<span data-ttu-id="0ac1b-176">Section</span><span class="sxs-lookup"><span data-stu-id="0ac1b-176">Section</span></span>](section.md) |<span data-ttu-id="0ac1b-177">读取分区的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-177">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="0ac1b-178">Create page</span><span class="sxs-lookup"><span data-stu-id="0ac1b-178">Create page</span></span>](../api/section_post_pages.md) |[<span data-ttu-id="0ac1b-179">Page</span><span class="sxs-lookup"><span data-stu-id="0ac1b-179">Page</span></span>](page.md)| <span data-ttu-id="0ac1b-180">通过发布到指定分区中的页面集合创建页面。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-180">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="0ac1b-181">List pages</span><span class="sxs-lookup"><span data-stu-id="0ac1b-181">List pages</span></span>](../api/section_list_pages.md) |<span data-ttu-id="0ac1b-182">[Page](page.md) collection</span><span class="sxs-lookup"><span data-stu-id="0ac1b-182">[Page](page.md) collection</span></span>| <span data-ttu-id="0ac1b-183">获取指定分区中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-183">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="0ac1b-184">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="0ac1b-184">copyToNotebook</span></span>](../api/section_copytonotebook.md)|<span data-ttu-id="0ac1b-185">无</span><span class="sxs-lookup"><span data-stu-id="0ac1b-185">None</span></span>|<span data-ttu-id="0ac1b-186">将分区复制到特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-186">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="0ac1b-187">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="0ac1b-187">copyToSectionGroup</span></span>](../api/section_copytosectiongroup.md)|<span data-ttu-id="0ac1b-188">无</span><span class="sxs-lookup"><span data-stu-id="0ac1b-188">None</span></span>|<span data-ttu-id="0ac1b-189">将分区复制到特定分区组。</span><span class="sxs-lookup"><span data-stu-id="0ac1b-189">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
