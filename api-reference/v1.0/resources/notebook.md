# <a name="notebook-resource-type"></a><span data-ttu-id="b3548-101">notebook 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3548-101">notebook resource type</span></span>

<span data-ttu-id="b3548-102">OneNote 笔记本。</span><span class="sxs-lookup"><span data-stu-id="b3548-102">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3548-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3548-103">JSON representation</span></span>

<span data-ttu-id="b3548-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3548-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.notebook"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "isShared": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.notebookLinks"},
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string",
  "userRole": "String"
}

```
## <a name="properties"></a><span data-ttu-id="b3548-105">属性</span><span class="sxs-lookup"><span data-stu-id="b3548-105">Properties</span></span>
| <span data-ttu-id="b3548-106">属性</span><span class="sxs-lookup"><span data-stu-id="b3548-106">Property</span></span>     | <span data-ttu-id="b3548-107">类型</span><span class="sxs-lookup"><span data-stu-id="b3548-107">Type</span></span>   |<span data-ttu-id="b3548-108">说明</span><span class="sxs-lookup"><span data-stu-id="b3548-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3548-109">createdBy</span><span class="sxs-lookup"><span data-stu-id="b3548-109">createdBy</span></span>|[<span data-ttu-id="b3548-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="b3548-110">identitySet</span></span>](identityset.md)|<span data-ttu-id="b3548-p101">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="b3548-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="b3548-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3548-113">createdDateTime</span></span>|<span data-ttu-id="b3548-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3548-114">DateTimeOffset</span></span>|<span data-ttu-id="b3548-p102">笔记本的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="b3548-p102">The date and time when the notebook was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="b3548-119">id</span><span class="sxs-lookup"><span data-stu-id="b3548-119">id</span></span>|<span data-ttu-id="b3548-120">字符串</span><span class="sxs-lookup"><span data-stu-id="b3548-120">String</span></span>|<span data-ttu-id="b3548-p103">笔记本的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="b3548-p103">The unique identifier of the notebook. Read-only.</span></span>|
|<span data-ttu-id="b3548-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="b3548-123">isDefault</span></span>|<span data-ttu-id="b3548-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="b3548-124">Boolean</span></span>|<span data-ttu-id="b3548-p104">指示其是否是用户的默认笔记本。只读。</span><span class="sxs-lookup"><span data-stu-id="b3548-p104">Indicates whether this is the user's default notebook. Read-only.</span></span>|
|<span data-ttu-id="b3548-127">isShared</span><span class="sxs-lookup"><span data-stu-id="b3548-127">isShared</span></span>|<span data-ttu-id="b3548-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="b3548-128">Boolean</span></span>|<span data-ttu-id="b3548-p105">指示是否共享笔记本。如果为 true，则笔记本的内容可供除所有者之外的人员查看。只读。</span><span class="sxs-lookup"><span data-stu-id="b3548-p105">Indicates whether the notebook is shared. If true, the contents of the notebook can be seen by people other than the owner. Read-only.</span></span>|
|<span data-ttu-id="b3548-132">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b3548-132">lastModifiedBy</span></span>|[<span data-ttu-id="b3548-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="b3548-133">identitySet</span></span>](identityset.md)|<span data-ttu-id="b3548-p106">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="b3548-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="b3548-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3548-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b3548-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3548-137">DateTimeOffset</span></span>|<span data-ttu-id="b3548-p107">上次修改笔记本的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="b3548-p107">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="b3548-142">links</span><span class="sxs-lookup"><span data-stu-id="b3548-142">links</span></span>|[<span data-ttu-id="b3548-143">NotebookLinks</span><span class="sxs-lookup"><span data-stu-id="b3548-143">NotebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="b3548-p108">用于打开笔记本的链接。如果安装了 OneNote 本机客户端，则 `oneNoteClientURL` 链接将在其中打开笔记本。`oneNoteWebURL` 链接将在 OneNote Online 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="b3548-p108">Links for opening the notebook. The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="b3548-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b3548-147">displayName</span></span>|<span data-ttu-id="b3548-148">字符串</span><span class="sxs-lookup"><span data-stu-id="b3548-148">String</span></span>|<span data-ttu-id="b3548-149">笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="b3548-149">The name of the notebook.</span></span>|
|<span data-ttu-id="b3548-150">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="b3548-150">sectionGroupsUrl</span></span>|<span data-ttu-id="b3548-151">字符串</span><span class="sxs-lookup"><span data-stu-id="b3548-151">String</span></span>|<span data-ttu-id="b3548-p109">|||UNTRANSLATED_CONTENT_START|||The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook. Read-only.|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="b3548-p109">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook. Read-only.</span></span>|
|<span data-ttu-id="b3548-154">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="b3548-154">sectionsUrl</span></span>|<span data-ttu-id="b3548-155">字符串</span><span class="sxs-lookup"><span data-stu-id="b3548-155">String</span></span>|<span data-ttu-id="b3548-p110">|||UNTRANSLATED_CONTENT_START|||The URL for the `sections` navigation property, which returns all the sections in the notebook. Read-only.|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="b3548-p110">The URL for the `sections` navigation property, which returns all the sections in the notebook. Read-only.</span></span>|
|<span data-ttu-id="b3548-158">self</span><span class="sxs-lookup"><span data-stu-id="b3548-158">self</span></span>|<span data-ttu-id="b3548-159">字符串</span><span class="sxs-lookup"><span data-stu-id="b3548-159">String</span></span>|<span data-ttu-id="b3548-p111">可以在其中获取关于笔记本的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="b3548-p111">The endpoint where you can get details about the notebook. Read-only.</span></span>|
|<span data-ttu-id="b3548-162">userRole</span><span class="sxs-lookup"><span data-stu-id="b3548-162">userRole</span></span>|<span data-ttu-id="b3548-163">onenoteUserRole</span><span class="sxs-lookup"><span data-stu-id="b3548-163">onenoteUserRole values</span></span>|<span data-ttu-id="b3548-p112">可能的值是：`Owner`、`Contributor`、`Reader`、`None`。“所有者”表示对笔记本的所有者级别访问权限。“参与者”表示对笔记本的读写访问权限。“读者”表示对笔记本的只读访问权限。只读。</span><span class="sxs-lookup"><span data-stu-id="b3548-p112">Possible values are: `Owner`, `Contributor`, `Reader`, `None`. Owner represents owner-level access to the notebook. Contributor represents read/write access to the notebook. Reader represents read-only access to the notebook. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3548-169">关系</span><span class="sxs-lookup"><span data-stu-id="b3548-169">Relationships</span></span>
| <span data-ttu-id="b3548-170">关系</span><span class="sxs-lookup"><span data-stu-id="b3548-170">Relationship</span></span> | <span data-ttu-id="b3548-171">类型</span><span class="sxs-lookup"><span data-stu-id="b3548-171">Type</span></span>   |<span data-ttu-id="b3548-172">说明</span><span class="sxs-lookup"><span data-stu-id="b3548-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3548-173">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="b3548-173">sectionGroups</span></span>|<span data-ttu-id="b3548-174">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="b3548-174">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="b3548-p113">笔记本中的分区组。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="b3548-p113">The section groups in the notebook. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b3548-178">sections</span><span class="sxs-lookup"><span data-stu-id="b3548-178">sections</span></span>|<span data-ttu-id="b3548-179">[OnenoteSection](section.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b3548-179">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="b3548-p114">笔记本中的分区。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b3548-p114">The sections in the notebook. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="b3548-183">方法</span><span class="sxs-lookup"><span data-stu-id="b3548-183">Methods</span></span>

| <span data-ttu-id="b3548-184">方法</span><span class="sxs-lookup"><span data-stu-id="b3548-184">Method</span></span>           | <span data-ttu-id="b3548-185">返回类型</span><span class="sxs-lookup"><span data-stu-id="b3548-185">Return Type</span></span>    |<span data-ttu-id="b3548-186">说明</span><span class="sxs-lookup"><span data-stu-id="b3548-186">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b3548-187">Get notebook</span><span class="sxs-lookup"><span data-stu-id="b3548-187">Get notebook</span></span>](../api/notebook_get.md) | [<span data-ttu-id="b3548-188">Notebook</span><span class="sxs-lookup"><span data-stu-id="b3548-188">Notebook</span></span>](notebook.md) |<span data-ttu-id="b3548-189">读取笔记本的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b3548-189">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="b3548-190">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="b3548-190">getRecentNotebooks</span></span>](../api/notebook_getrecentnotebooks.md) | <span data-ttu-id="b3548-191">[recentNotebook](recentnotebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b3548-191">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="b3548-192">获取用户最近访问过的笔记本的集合。</span><span class="sxs-lookup"><span data-stu-id="b3548-192">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="b3548-193">创建分区组</span><span class="sxs-lookup"><span data-stu-id="b3548-193">Create section group</span></span>](../api/notebook_post_sectiongroups.md) |[<span data-ttu-id="b3548-194">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="b3548-194">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="b3548-195">通过发布到指定笔记本中的 sectionGroups 集合创建分区组。</span><span class="sxs-lookup"><span data-stu-id="b3548-195">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="b3548-196">List section groups</span><span class="sxs-lookup"><span data-stu-id="b3548-196">List section groups</span></span>](../api/notebook_list_sectiongroups.md) |<span data-ttu-id="b3548-197">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="b3548-197">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="b3548-198">获取指定笔记本中的分区组集合。</span><span class="sxs-lookup"><span data-stu-id="b3548-198">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="b3548-199">创建分区</span><span class="sxs-lookup"><span data-stu-id="b3548-199">Create section</span></span>](../api/notebook_post_sections.md) |[<span data-ttu-id="b3548-200">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="b3548-200">OnenoteSection</span></span>](section.md)| <span data-ttu-id="b3548-201">通过发布到指定笔记本中的分区集合创建分区。</span><span class="sxs-lookup"><span data-stu-id="b3548-201">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="b3548-202">列出分区</span><span class="sxs-lookup"><span data-stu-id="b3548-202">List sections</span></span>](../api/notebook_list_sections.md) |<span data-ttu-id="b3548-203">[OnenoteSection](section.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b3548-203">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="b3548-204">获取指定笔记本中的分区集合。</span><span class="sxs-lookup"><span data-stu-id="b3548-204">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="b3548-205">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="b3548-205">copyNotebook</span></span>](../api/notebook_copynotebook.md)| <span data-ttu-id="b3548-206">无</span><span class="sxs-lookup"><span data-stu-id="b3548-206">None</span></span> | <span data-ttu-id="b3548-207">复制笔记本。</span><span class="sxs-lookup"><span data-stu-id="b3548-207">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
