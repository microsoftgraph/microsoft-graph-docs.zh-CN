---
title: notebook 资源类型
description: OneNote 笔记本。
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 0a657ea6d5837674a7881bc9ef6095af5529355a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894444"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="19035-103">notebook 资源类型</span><span class="sxs-lookup"><span data-stu-id="19035-103">notebook resource type</span></span>

<span data-ttu-id="19035-104">OneNote 笔记本。</span><span class="sxs-lookup"><span data-stu-id="19035-104">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="19035-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19035-105">JSON representation</span></span>

<span data-ttu-id="19035-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19035-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="19035-107">属性</span><span class="sxs-lookup"><span data-stu-id="19035-107">Properties</span></span>
| <span data-ttu-id="19035-108">属性</span><span class="sxs-lookup"><span data-stu-id="19035-108">Property</span></span>     | <span data-ttu-id="19035-109">类型</span><span class="sxs-lookup"><span data-stu-id="19035-109">Type</span></span>   |<span data-ttu-id="19035-110">说明</span><span class="sxs-lookup"><span data-stu-id="19035-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19035-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="19035-111">createdBy</span></span>|[<span data-ttu-id="19035-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="19035-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="19035-p101">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="19035-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="19035-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19035-115">createdDateTime</span></span>|<span data-ttu-id="19035-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19035-116">DateTimeOffset</span></span>|<span data-ttu-id="19035-p102">笔记本的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="19035-p102">The date and time when the notebook was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="19035-121">id</span><span class="sxs-lookup"><span data-stu-id="19035-121">id</span></span>|<span data-ttu-id="19035-122">字符串</span><span class="sxs-lookup"><span data-stu-id="19035-122">String</span></span>|<span data-ttu-id="19035-p103">笔记本的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="19035-p103">The unique identifier of the notebook. Read-only.</span></span>|
|<span data-ttu-id="19035-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="19035-125">isDefault</span></span>|<span data-ttu-id="19035-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="19035-126">Boolean</span></span>|<span data-ttu-id="19035-p104">指示其是否是用户的默认笔记本。只读。</span><span class="sxs-lookup"><span data-stu-id="19035-p104">Indicates whether this is the user's default notebook. Read-only.</span></span>|
|<span data-ttu-id="19035-129">isShared</span><span class="sxs-lookup"><span data-stu-id="19035-129">isShared</span></span>|<span data-ttu-id="19035-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="19035-130">Boolean</span></span>|<span data-ttu-id="19035-p105">指示是否共享笔记本。如果为 true，则笔记本的内容可供除所有者之外的人员查看。只读。</span><span class="sxs-lookup"><span data-stu-id="19035-p105">Indicates whether the notebook is shared. If true, the contents of the notebook can be seen by people other than the owner. Read-only.</span></span>|
|<span data-ttu-id="19035-134">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="19035-134">lastModifiedBy</span></span>|[<span data-ttu-id="19035-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="19035-135">identitySet</span></span>](identityset.md)|<span data-ttu-id="19035-p106">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="19035-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="19035-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19035-138">lastModifiedDateTime</span></span>|<span data-ttu-id="19035-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19035-139">DateTimeOffset</span></span>|<span data-ttu-id="19035-p107">上次修改笔记本的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="19035-p107">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="19035-144">links</span><span class="sxs-lookup"><span data-stu-id="19035-144">links</span></span>|[<span data-ttu-id="19035-145">NotebookLinks</span><span class="sxs-lookup"><span data-stu-id="19035-145">NotebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="19035-p108">用于打开笔记本的链接。如果安装了 OneNote 本机客户端，则 `oneNoteClientURL` 链接将在其中打开笔记本。`oneNoteWebURL` 链接将在 OneNote Online 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="19035-p108">Links for opening the notebook. The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="19035-149">displayName</span><span class="sxs-lookup"><span data-stu-id="19035-149">displayName</span></span>|<span data-ttu-id="19035-150">字符串</span><span class="sxs-lookup"><span data-stu-id="19035-150">String</span></span>|<span data-ttu-id="19035-151">笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="19035-151">The name of the notebook.</span></span>|
|<span data-ttu-id="19035-152">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="19035-152">sectionGroupsUrl</span></span>|<span data-ttu-id="19035-153">String</span><span class="sxs-lookup"><span data-stu-id="19035-153">String</span></span>|<span data-ttu-id="19035-p109">`sectionGroups` 导航属性的 URL，其将返回笔记本中的所有分区组。只读。</span><span class="sxs-lookup"><span data-stu-id="19035-p109">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook. Read-only.</span></span>|
|<span data-ttu-id="19035-156">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="19035-156">sectionsUrl</span></span>|<span data-ttu-id="19035-157">String</span><span class="sxs-lookup"><span data-stu-id="19035-157">String</span></span>|<span data-ttu-id="19035-p110">`sections` 导航属性的 URL，其将返回笔记本中的所有分区。只读。</span><span class="sxs-lookup"><span data-stu-id="19035-p110">The URL for the `sections` navigation property, which returns all the sections in the notebook. Read-only.</span></span>|
|<span data-ttu-id="19035-160">self</span><span class="sxs-lookup"><span data-stu-id="19035-160">self</span></span>|<span data-ttu-id="19035-161">字符串</span><span class="sxs-lookup"><span data-stu-id="19035-161">String</span></span>|<span data-ttu-id="19035-p111">可以在其中获取关于笔记本的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="19035-p111">The endpoint where you can get details about the notebook. Read-only.</span></span>|
|<span data-ttu-id="19035-164">userRole</span><span class="sxs-lookup"><span data-stu-id="19035-164">userRole</span></span>|<span data-ttu-id="19035-165">onenoteUserRole</span><span class="sxs-lookup"><span data-stu-id="19035-165">onenoteUserRole</span></span>|<span data-ttu-id="19035-p112">可能的值是：`Owner`、`Contributor`、`Reader`、`None`。“所有者”表示对笔记本的所有者级别访问权限。“参与者”表示对笔记本的读写访问权限。“读者”表示对笔记本的只读访问权限。只读。</span><span class="sxs-lookup"><span data-stu-id="19035-p112">Possible values are: `Owner`, `Contributor`, `Reader`, `None`. Owner represents owner-level access to the notebook. Contributor represents read/write access to the notebook. Reader represents read-only access to the notebook. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19035-171">Relationships</span><span class="sxs-lookup"><span data-stu-id="19035-171">Relationships</span></span>
| <span data-ttu-id="19035-172">关系</span><span class="sxs-lookup"><span data-stu-id="19035-172">Relationship</span></span> | <span data-ttu-id="19035-173">类型</span><span class="sxs-lookup"><span data-stu-id="19035-173">Type</span></span>   |<span data-ttu-id="19035-174">说明</span><span class="sxs-lookup"><span data-stu-id="19035-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19035-175">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="19035-175">sectionGroups</span></span>|<span data-ttu-id="19035-176">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="19035-176">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="19035-p113">笔记本中的分区组。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="19035-p113">The section groups in the notebook. Read-only. Nullable.</span></span>|
|<span data-ttu-id="19035-180">sections</span><span class="sxs-lookup"><span data-stu-id="19035-180">sections</span></span>|<span data-ttu-id="19035-181">[OnenoteSection](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="19035-181">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="19035-p114">笔记本中的分区。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="19035-p114">The sections in the notebook. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="19035-185">方法</span><span class="sxs-lookup"><span data-stu-id="19035-185">Methods</span></span>

| <span data-ttu-id="19035-186">方法</span><span class="sxs-lookup"><span data-stu-id="19035-186">Method</span></span>           | <span data-ttu-id="19035-187">返回类型</span><span class="sxs-lookup"><span data-stu-id="19035-187">Return Type</span></span>    |<span data-ttu-id="19035-188">说明</span><span class="sxs-lookup"><span data-stu-id="19035-188">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="19035-189">Get notebook</span><span class="sxs-lookup"><span data-stu-id="19035-189">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="19035-190">Notebook</span><span class="sxs-lookup"><span data-stu-id="19035-190">Notebook</span></span>](notebook.md) |<span data-ttu-id="19035-191">读取笔记本的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="19035-191">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="19035-192">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="19035-192">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="19035-193">[recentNotebook](recentnotebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="19035-193">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="19035-194">获取用户最近访问过的笔记本的集合。</span><span class="sxs-lookup"><span data-stu-id="19035-194">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="19035-195">创建分区组</span><span class="sxs-lookup"><span data-stu-id="19035-195">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="19035-196">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="19035-196">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="19035-197">通过发布到指定笔记本中的 sectionGroups 集合创建分区组。</span><span class="sxs-lookup"><span data-stu-id="19035-197">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="19035-198">List section groups</span><span class="sxs-lookup"><span data-stu-id="19035-198">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="19035-199">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="19035-199">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="19035-200">获取指定笔记本中的分区组集合。</span><span class="sxs-lookup"><span data-stu-id="19035-200">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="19035-201">Create section</span><span class="sxs-lookup"><span data-stu-id="19035-201">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="19035-202">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="19035-202">OnenoteSection</span></span>](section.md)| <span data-ttu-id="19035-203">通过发布到指定笔记本中的分区集合创建分区。</span><span class="sxs-lookup"><span data-stu-id="19035-203">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="19035-204">List sections</span><span class="sxs-lookup"><span data-stu-id="19035-204">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="19035-205">[OnenoteSection](section.md)集合</span><span class="sxs-lookup"><span data-stu-id="19035-205">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="19035-206">获取指定笔记本中的分区集合。</span><span class="sxs-lookup"><span data-stu-id="19035-206">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="19035-207">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="19035-207">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="19035-208">无</span><span class="sxs-lookup"><span data-stu-id="19035-208">None</span></span> | <span data-ttu-id="19035-209">复制笔记本。</span><span class="sxs-lookup"><span data-stu-id="19035-209">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
