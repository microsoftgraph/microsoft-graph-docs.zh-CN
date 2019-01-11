---
title: notebook 资源类型
description: OneNote 笔记本。
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: c39ac85dcfacb332a72c81d1d5f075a7a5021047
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876557"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="c106a-103">notebook 资源类型</span><span class="sxs-lookup"><span data-stu-id="c106a-103">notebook resource type</span></span>

> <span data-ttu-id="c106a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c106a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c106a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c106a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c106a-106">OneNote 笔记本。</span><span class="sxs-lookup"><span data-stu-id="c106a-106">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c106a-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c106a-107">JSON representation</span></span>

<span data-ttu-id="c106a-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c106a-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
## <a name="properties"></a><span data-ttu-id="c106a-109">属性</span><span class="sxs-lookup"><span data-stu-id="c106a-109">Properties</span></span>
| <span data-ttu-id="c106a-110">属性</span><span class="sxs-lookup"><span data-stu-id="c106a-110">Property</span></span>     | <span data-ttu-id="c106a-111">类型</span><span class="sxs-lookup"><span data-stu-id="c106a-111">Type</span></span>   |<span data-ttu-id="c106a-112">说明</span><span class="sxs-lookup"><span data-stu-id="c106a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c106a-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="c106a-113">createdBy</span></span>|[<span data-ttu-id="c106a-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="c106a-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="c106a-p102">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="c106a-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="c106a-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c106a-117">createdDateTime</span></span>|<span data-ttu-id="c106a-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c106a-118">DateTimeOffset</span></span>|<span data-ttu-id="c106a-p103">笔记本的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="c106a-p103">The date and time when the notebook was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="c106a-123">id</span><span class="sxs-lookup"><span data-stu-id="c106a-123">id</span></span>|<span data-ttu-id="c106a-124">字符串</span><span class="sxs-lookup"><span data-stu-id="c106a-124">String</span></span>|<span data-ttu-id="c106a-p104">笔记本的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="c106a-p104">The unique identifier of the notebook. Read-only.</span></span>|
|<span data-ttu-id="c106a-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="c106a-127">isDefault</span></span>|<span data-ttu-id="c106a-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="c106a-128">Boolean</span></span>|<span data-ttu-id="c106a-p105">指示其是否是用户的默认笔记本。只读。</span><span class="sxs-lookup"><span data-stu-id="c106a-p105">Indicates whether this is the user's default notebook. Read-only.</span></span>|
|<span data-ttu-id="c106a-131">isShared</span><span class="sxs-lookup"><span data-stu-id="c106a-131">isShared</span></span>|<span data-ttu-id="c106a-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="c106a-132">Boolean</span></span>|<span data-ttu-id="c106a-p106">指示是否共享笔记本。如果为 true，则笔记本的内容可供除所有者之外的人员查看。只读。</span><span class="sxs-lookup"><span data-stu-id="c106a-p106">Indicates whether the notebook is shared. If true, the contents of the notebook can be seen by people other than the owner. Read-only.</span></span>|
|<span data-ttu-id="c106a-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c106a-136">lastModifiedBy</span></span>|[<span data-ttu-id="c106a-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="c106a-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="c106a-p107">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="c106a-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="c106a-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c106a-140">lastModifiedDateTime</span></span>|<span data-ttu-id="c106a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c106a-141">DateTimeOffset</span></span>|<span data-ttu-id="c106a-p108">上次修改笔记本的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="c106a-p108">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="c106a-146">links</span><span class="sxs-lookup"><span data-stu-id="c106a-146">links</span></span>|[<span data-ttu-id="c106a-147">NotebookLinks</span><span class="sxs-lookup"><span data-stu-id="c106a-147">NotebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="c106a-p109">用于打开笔记本的链接。如果安装了 OneNote 本机客户端，则 `oneNoteClientURL` 链接将在其中打开笔记本。`oneNoteWebURL` 链接将在 OneNote Online 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="c106a-p109">Links for opening the notebook. The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="c106a-151">displayName</span><span class="sxs-lookup"><span data-stu-id="c106a-151">displayName</span></span>|<span data-ttu-id="c106a-152">字符串</span><span class="sxs-lookup"><span data-stu-id="c106a-152">String</span></span>|<span data-ttu-id="c106a-153">笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="c106a-153">The name of the notebook.</span></span>|
|<span data-ttu-id="c106a-154">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="c106a-154">sectionGroupsUrl</span></span>|<span data-ttu-id="c106a-155">String</span><span class="sxs-lookup"><span data-stu-id="c106a-155">String</span></span>|<span data-ttu-id="c106a-p110">`sectionGroups` 导航属性的 URL，其将返回笔记本中的所有分区组。只读。</span><span class="sxs-lookup"><span data-stu-id="c106a-p110">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook. Read-only.</span></span>|
|<span data-ttu-id="c106a-158">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="c106a-158">sectionsUrl</span></span>|<span data-ttu-id="c106a-159">String</span><span class="sxs-lookup"><span data-stu-id="c106a-159">String</span></span>|<span data-ttu-id="c106a-p111">`sections` 导航属性的 URL，其将返回笔记本中的所有分区。只读。</span><span class="sxs-lookup"><span data-stu-id="c106a-p111">The URL for the `sections` navigation property, which returns all the sections in the notebook. Read-only.</span></span>|
|<span data-ttu-id="c106a-162">self</span><span class="sxs-lookup"><span data-stu-id="c106a-162">self</span></span>|<span data-ttu-id="c106a-163">字符串</span><span class="sxs-lookup"><span data-stu-id="c106a-163">String</span></span>|<span data-ttu-id="c106a-p112">可以在其中获取关于笔记本的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="c106a-p112">The endpoint where you can get details about the notebook. Read-only.</span></span>|
|<span data-ttu-id="c106a-166">userRole</span><span class="sxs-lookup"><span data-stu-id="c106a-166">userRole</span></span>|<span data-ttu-id="c106a-167">String</span><span class="sxs-lookup"><span data-stu-id="c106a-167">String</span></span>|<span data-ttu-id="c106a-p113">可能的值是：`Owner`、`Contributor`、`Reader`、`None`。“所有者”表示对笔记本的所有者级别访问权限。“参与者”表示对笔记本的读写访问权限。“读者”表示对笔记本的只读访问权限。只读。</span><span class="sxs-lookup"><span data-stu-id="c106a-p113">Possible values are: `Owner`, `Contributor`, `Reader`, `None`. Owner represents owner-level access to the notebook. Contributor represents read/write access to the notebook. Reader represents read-only access to the notebook. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c106a-173">Relationships</span><span class="sxs-lookup"><span data-stu-id="c106a-173">Relationships</span></span>
| <span data-ttu-id="c106a-174">关系</span><span class="sxs-lookup"><span data-stu-id="c106a-174">Relationship</span></span> | <span data-ttu-id="c106a-175">类型</span><span class="sxs-lookup"><span data-stu-id="c106a-175">Type</span></span>   |<span data-ttu-id="c106a-176">说明</span><span class="sxs-lookup"><span data-stu-id="c106a-176">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c106a-177">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="c106a-177">sectionGroups</span></span>|<span data-ttu-id="c106a-178">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="c106a-178">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="c106a-p114">笔记本中的分区组。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="c106a-p114">The section groups in the notebook. Read-only. Nullable.</span></span>|
|<span data-ttu-id="c106a-182">节</span><span class="sxs-lookup"><span data-stu-id="c106a-182">sections</span></span>|<span data-ttu-id="c106a-183">[Section](section.md) collection</span><span class="sxs-lookup"><span data-stu-id="c106a-183">[Section](section.md) collection</span></span>|<span data-ttu-id="c106a-p115">笔记本中的分区。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c106a-p115">The sections in the notebook. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="c106a-187">方法</span><span class="sxs-lookup"><span data-stu-id="c106a-187">Methods</span></span>

| <span data-ttu-id="c106a-188">方法</span><span class="sxs-lookup"><span data-stu-id="c106a-188">Method</span></span>           | <span data-ttu-id="c106a-189">返回类型</span><span class="sxs-lookup"><span data-stu-id="c106a-189">Return Type</span></span>    |<span data-ttu-id="c106a-190">说明</span><span class="sxs-lookup"><span data-stu-id="c106a-190">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c106a-191">Get notebook</span><span class="sxs-lookup"><span data-stu-id="c106a-191">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="c106a-192">Notebook</span><span class="sxs-lookup"><span data-stu-id="c106a-192">Notebook</span></span>](notebook.md) |<span data-ttu-id="c106a-193">读取笔记本的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c106a-193">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="c106a-194">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="c106a-194">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="c106a-195">[recentNotebook](recentnotebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c106a-195">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="c106a-196">获取用户最近访问过的笔记本的集合。</span><span class="sxs-lookup"><span data-stu-id="c106a-196">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="c106a-197">创建分区组</span><span class="sxs-lookup"><span data-stu-id="c106a-197">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="c106a-198">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="c106a-198">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="c106a-199">通过发布到指定笔记本中的 sectionGroups 集合创建分区组。</span><span class="sxs-lookup"><span data-stu-id="c106a-199">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="c106a-200">List section groups</span><span class="sxs-lookup"><span data-stu-id="c106a-200">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="c106a-201">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="c106a-201">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="c106a-202">获取指定笔记本中的分区组集合。</span><span class="sxs-lookup"><span data-stu-id="c106a-202">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="c106a-203">Create section</span><span class="sxs-lookup"><span data-stu-id="c106a-203">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="c106a-204">Section</span><span class="sxs-lookup"><span data-stu-id="c106a-204">Section</span></span>](section.md)| <span data-ttu-id="c106a-205">通过发布到指定笔记本中的分区集合创建分区。</span><span class="sxs-lookup"><span data-stu-id="c106a-205">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="c106a-206">List sections</span><span class="sxs-lookup"><span data-stu-id="c106a-206">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="c106a-207">[Section](section.md) collection</span><span class="sxs-lookup"><span data-stu-id="c106a-207">[Section](section.md) collection</span></span>| <span data-ttu-id="c106a-208">获取指定笔记本中的分区集合。</span><span class="sxs-lookup"><span data-stu-id="c106a-208">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="c106a-209">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="c106a-209">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="c106a-210">无</span><span class="sxs-lookup"><span data-stu-id="c106a-210">None</span></span> | <span data-ttu-id="c106a-211">复制笔记本。</span><span class="sxs-lookup"><span data-stu-id="c106a-211">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
