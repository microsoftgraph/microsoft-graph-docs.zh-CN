---
title: 笔记本资源类型
description: OneNote 笔记本。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: c52108e415388d8e4e919709fd619660c531aef8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960376"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="92c44-103">笔记本资源类型</span><span class="sxs-lookup"><span data-stu-id="92c44-103">notebook resource type</span></span>

<span data-ttu-id="92c44-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92c44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92c44-105">OneNote 笔记本。</span><span class="sxs-lookup"><span data-stu-id="92c44-105">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="92c44-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92c44-106">JSON representation</span></span>

<span data-ttu-id="92c44-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92c44-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
## <a name="properties"></a><span data-ttu-id="92c44-108">属性</span><span class="sxs-lookup"><span data-stu-id="92c44-108">Properties</span></span>
| <span data-ttu-id="92c44-109">属性</span><span class="sxs-lookup"><span data-stu-id="92c44-109">Property</span></span>     | <span data-ttu-id="92c44-110">类型</span><span class="sxs-lookup"><span data-stu-id="92c44-110">Type</span></span>   |<span data-ttu-id="92c44-111">说明</span><span class="sxs-lookup"><span data-stu-id="92c44-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92c44-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="92c44-112">createdBy</span></span>|[<span data-ttu-id="92c44-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="92c44-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="92c44-p101">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="92c44-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="92c44-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92c44-116">createdDateTime</span></span>|<span data-ttu-id="92c44-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92c44-117">DateTimeOffset</span></span>|<span data-ttu-id="92c44-118">笔记本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="92c44-118">The date and time when the notebook was created.</span></span> <span data-ttu-id="92c44-119">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="92c44-119">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="92c44-120">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="92c44-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="92c44-121">只读。</span><span class="sxs-lookup"><span data-stu-id="92c44-121">Read-only.</span></span>|
|<span data-ttu-id="92c44-122">id</span><span class="sxs-lookup"><span data-stu-id="92c44-122">id</span></span>|<span data-ttu-id="92c44-123">String</span><span class="sxs-lookup"><span data-stu-id="92c44-123">String</span></span>|<span data-ttu-id="92c44-124">笔记本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="92c44-124">The unique identifier of the notebook.</span></span> <span data-ttu-id="92c44-125">只读。</span><span class="sxs-lookup"><span data-stu-id="92c44-125">Read-only.</span></span>|
|<span data-ttu-id="92c44-126">isDefault</span><span class="sxs-lookup"><span data-stu-id="92c44-126">isDefault</span></span>|<span data-ttu-id="92c44-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="92c44-127">Boolean</span></span>|<span data-ttu-id="92c44-128">指示这是否是用户的默认笔记本。</span><span class="sxs-lookup"><span data-stu-id="92c44-128">Indicates whether this is the user's default notebook.</span></span> <span data-ttu-id="92c44-129">只读。</span><span class="sxs-lookup"><span data-stu-id="92c44-129">Read-only.</span></span>|
|<span data-ttu-id="92c44-130">isShared</span><span class="sxs-lookup"><span data-stu-id="92c44-130">isShared</span></span>|<span data-ttu-id="92c44-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="92c44-131">Boolean</span></span>|<span data-ttu-id="92c44-132">指明笔记本是否为共享。</span><span class="sxs-lookup"><span data-stu-id="92c44-132">Indicates whether the notebook is shared.</span></span> <span data-ttu-id="92c44-133">如果是，笔记本的内容可供所有者以外的用户查看。</span><span class="sxs-lookup"><span data-stu-id="92c44-133">If true, the contents of the notebook can be seen by people other than the owner.</span></span> <span data-ttu-id="92c44-134">只读。</span><span class="sxs-lookup"><span data-stu-id="92c44-134">Read-only.</span></span>|
|<span data-ttu-id="92c44-135">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="92c44-135">lastModifiedBy</span></span>|[<span data-ttu-id="92c44-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="92c44-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="92c44-p106">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="92c44-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="92c44-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92c44-139">lastModifiedDateTime</span></span>|<span data-ttu-id="92c44-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92c44-140">DateTimeOffset</span></span>|<span data-ttu-id="92c44-141">上次修改笔记本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="92c44-141">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="92c44-142">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="92c44-142">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="92c44-143">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="92c44-143">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="92c44-144">只读。</span><span class="sxs-lookup"><span data-stu-id="92c44-144">Read-only.</span></span>|
|<span data-ttu-id="92c44-145">links</span><span class="sxs-lookup"><span data-stu-id="92c44-145">links</span></span>|[<span data-ttu-id="92c44-146">notebookLinks</span><span class="sxs-lookup"><span data-stu-id="92c44-146">notebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="92c44-147">用于打开笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="92c44-147">Links for opening the notebook.</span></span> <span data-ttu-id="92c44-148">链接 `oneNoteClientURL` 将在 OneNote 本机客户端中打开笔记本（如果已安装）。</span><span class="sxs-lookup"><span data-stu-id="92c44-148">The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed.</span></span> <span data-ttu-id="92c44-149">该 `oneNoteWebURL` 链接在 OneNote 网页中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="92c44-149">The `oneNoteWebURL` link opens the notebook in OneNote on the web.</span></span>|
|<span data-ttu-id="92c44-150">displayName</span><span class="sxs-lookup"><span data-stu-id="92c44-150">displayName</span></span>|<span data-ttu-id="92c44-151">String</span><span class="sxs-lookup"><span data-stu-id="92c44-151">String</span></span>|<span data-ttu-id="92c44-152">笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="92c44-152">The name of the notebook.</span></span>|
|<span data-ttu-id="92c44-153">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="92c44-153">sectionGroupsUrl</span></span>|<span data-ttu-id="92c44-154">String</span><span class="sxs-lookup"><span data-stu-id="92c44-154">String</span></span>|<span data-ttu-id="92c44-155">导航属性的 `sectionGroups` URL，可返回笔记本中所有节组。</span><span class="sxs-lookup"><span data-stu-id="92c44-155">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook.</span></span> <span data-ttu-id="92c44-156">只读。</span><span class="sxs-lookup"><span data-stu-id="92c44-156">Read-only.</span></span>|
|<span data-ttu-id="92c44-157">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="92c44-157">sectionsUrl</span></span>|<span data-ttu-id="92c44-158">String</span><span class="sxs-lookup"><span data-stu-id="92c44-158">String</span></span>|<span data-ttu-id="92c44-159">导航属性的 `sections` URL，可返回笔记本中所有节。</span><span class="sxs-lookup"><span data-stu-id="92c44-159">The URL for the `sections` navigation property, which returns all the sections in the notebook.</span></span> <span data-ttu-id="92c44-160">只读。</span><span class="sxs-lookup"><span data-stu-id="92c44-160">Read-only.</span></span>|
|<span data-ttu-id="92c44-161">self</span><span class="sxs-lookup"><span data-stu-id="92c44-161">self</span></span>|<span data-ttu-id="92c44-162">String</span><span class="sxs-lookup"><span data-stu-id="92c44-162">String</span></span>|<span data-ttu-id="92c44-163">终结点，您可在此处获取关于笔记本的详细信息。</span><span class="sxs-lookup"><span data-stu-id="92c44-163">The endpoint where you can get details about the notebook.</span></span> <span data-ttu-id="92c44-164">只读。</span><span class="sxs-lookup"><span data-stu-id="92c44-164">Read-only.</span></span>|
|<span data-ttu-id="92c44-165">userRole</span><span class="sxs-lookup"><span data-stu-id="92c44-165">userRole</span></span>|<span data-ttu-id="92c44-166">onenoteUserRole</span><span class="sxs-lookup"><span data-stu-id="92c44-166">onenoteUserRole</span></span>|<span data-ttu-id="92c44-167">可取值为：`Owner`、`Contributor`、`Reader`、`None`。</span><span class="sxs-lookup"><span data-stu-id="92c44-167">Possible values are: `Owner`, `Contributor`, `Reader`, `None`.</span></span> <span data-ttu-id="92c44-168">所有者表示对笔记本的所有者级别访问权限。</span><span class="sxs-lookup"><span data-stu-id="92c44-168">Owner represents owner-level access to the notebook.</span></span> <span data-ttu-id="92c44-169">参与者表示笔记本的读/写访问权限。</span><span class="sxs-lookup"><span data-stu-id="92c44-169">Contributor represents read/write access to the notebook.</span></span> <span data-ttu-id="92c44-170">Reader 表示对笔记本的只读访问权限。</span><span class="sxs-lookup"><span data-stu-id="92c44-170">Reader represents read-only access to the notebook.</span></span> <span data-ttu-id="92c44-171">只读。</span><span class="sxs-lookup"><span data-stu-id="92c44-171">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92c44-172">关系</span><span class="sxs-lookup"><span data-stu-id="92c44-172">Relationships</span></span>
| <span data-ttu-id="92c44-173">关系</span><span class="sxs-lookup"><span data-stu-id="92c44-173">Relationship</span></span> | <span data-ttu-id="92c44-174">类型</span><span class="sxs-lookup"><span data-stu-id="92c44-174">Type</span></span>   |<span data-ttu-id="92c44-175">说明</span><span class="sxs-lookup"><span data-stu-id="92c44-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92c44-176">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="92c44-176">sectionGroups</span></span>|<span data-ttu-id="92c44-177">[sectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92c44-177">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="92c44-178">笔记本中的分区组。</span><span class="sxs-lookup"><span data-stu-id="92c44-178">The section groups in the notebook.</span></span> <span data-ttu-id="92c44-179">只读。</span><span class="sxs-lookup"><span data-stu-id="92c44-179">Read-only.</span></span> <span data-ttu-id="92c44-180">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="92c44-180">Nullable.</span></span>|
|<span data-ttu-id="92c44-181">sections</span><span class="sxs-lookup"><span data-stu-id="92c44-181">sections</span></span>|<span data-ttu-id="92c44-182">[onenoteSection](onenotesection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92c44-182">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="92c44-183">笔记本中的节。</span><span class="sxs-lookup"><span data-stu-id="92c44-183">The sections in the notebook.</span></span> <span data-ttu-id="92c44-184">只读。</span><span class="sxs-lookup"><span data-stu-id="92c44-184">Read-only.</span></span> <span data-ttu-id="92c44-185">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="92c44-185">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="92c44-186">方法</span><span class="sxs-lookup"><span data-stu-id="92c44-186">Methods</span></span>

| <span data-ttu-id="92c44-187">方法</span><span class="sxs-lookup"><span data-stu-id="92c44-187">Method</span></span>           | <span data-ttu-id="92c44-188">返回类型</span><span class="sxs-lookup"><span data-stu-id="92c44-188">Return Type</span></span>    |<span data-ttu-id="92c44-189">说明</span><span class="sxs-lookup"><span data-stu-id="92c44-189">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92c44-190">获取笔记本</span><span class="sxs-lookup"><span data-stu-id="92c44-190">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="92c44-191">笔记本</span><span class="sxs-lookup"><span data-stu-id="92c44-191">notebook</span></span>](notebook.md) |<span data-ttu-id="92c44-192">读取笔记本的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="92c44-192">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="92c44-193">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="92c44-193">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="92c44-194">[recentNotebook](recentnotebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92c44-194">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="92c44-195">获取用户最近访问过的一组笔记本。</span><span class="sxs-lookup"><span data-stu-id="92c44-195">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="92c44-196">getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="92c44-196">getNotebookFromWebUrl</span></span>](../api/notebook-getnotebookfromweburl.md) | [<span data-ttu-id="92c44-197">笔记本</span><span class="sxs-lookup"><span data-stu-id="92c44-197">notebook</span></span>](notebook.md) | <span data-ttu-id="92c44-198">使用笔记本对象 URL 路径检索其属性和关系。</span><span class="sxs-lookup"><span data-stu-id="92c44-198">Retrieve the properties and relationships of a notebook object using its URL path.</span></span> |
|[<span data-ttu-id="92c44-199">创建分区组</span><span class="sxs-lookup"><span data-stu-id="92c44-199">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="92c44-200">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="92c44-200">sectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="92c44-201">通过发布到指定笔记本中的 sectionGroups 集合创建分区组。</span><span class="sxs-lookup"><span data-stu-id="92c44-201">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="92c44-202">列出分区组</span><span class="sxs-lookup"><span data-stu-id="92c44-202">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="92c44-203">[sectionGroup](sectiongroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92c44-203">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="92c44-204">获取指定笔记本中的分区组集合。</span><span class="sxs-lookup"><span data-stu-id="92c44-204">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="92c44-205">创建分区</span><span class="sxs-lookup"><span data-stu-id="92c44-205">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="92c44-206">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="92c44-206">onenoteSection</span></span>](onenotesection.md)| <span data-ttu-id="92c44-207">通过发布到指定笔记本中的节集合创建分区。</span><span class="sxs-lookup"><span data-stu-id="92c44-207">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="92c44-208">列出节</span><span class="sxs-lookup"><span data-stu-id="92c44-208">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="92c44-209">[onenoteSection](onenotesection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92c44-209">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="92c44-210">获取指定笔记本中的分区集合。</span><span class="sxs-lookup"><span data-stu-id="92c44-210">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="92c44-211">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="92c44-211">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="92c44-212">无</span><span class="sxs-lookup"><span data-stu-id="92c44-212">None</span></span> | <span data-ttu-id="92c44-213">复制笔记本。</span><span class="sxs-lookup"><span data-stu-id="92c44-213">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


