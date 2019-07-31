---
title: 笔记本资源类型
description: OneNote 笔记本。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 76d4d8daf17fa6c953ad7bf727c8b6481f7dc8b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009592"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="44bbb-103">笔记本资源类型</span><span class="sxs-lookup"><span data-stu-id="44bbb-103">notebook resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44bbb-104">OneNote 笔记本。</span><span class="sxs-lookup"><span data-stu-id="44bbb-104">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="44bbb-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44bbb-105">JSON representation</span></span>

<span data-ttu-id="44bbb-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44bbb-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="44bbb-107">属性</span><span class="sxs-lookup"><span data-stu-id="44bbb-107">Properties</span></span>
| <span data-ttu-id="44bbb-108">属性</span><span class="sxs-lookup"><span data-stu-id="44bbb-108">Property</span></span>     | <span data-ttu-id="44bbb-109">类型</span><span class="sxs-lookup"><span data-stu-id="44bbb-109">Type</span></span>   |<span data-ttu-id="44bbb-110">说明</span><span class="sxs-lookup"><span data-stu-id="44bbb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44bbb-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="44bbb-111">createdBy</span></span>|[<span data-ttu-id="44bbb-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="44bbb-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="44bbb-p101">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="44bbb-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="44bbb-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44bbb-115">createdDateTime</span></span>|<span data-ttu-id="44bbb-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44bbb-116">DateTimeOffset</span></span>|<span data-ttu-id="44bbb-117">笔记本的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="44bbb-117">The date and time when the notebook was created.</span></span> <span data-ttu-id="44bbb-118">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="44bbb-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="44bbb-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="44bbb-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="44bbb-120">只读。</span><span class="sxs-lookup"><span data-stu-id="44bbb-120">Read-only.</span></span>|
|<span data-ttu-id="44bbb-121">id</span><span class="sxs-lookup"><span data-stu-id="44bbb-121">id</span></span>|<span data-ttu-id="44bbb-122">String</span><span class="sxs-lookup"><span data-stu-id="44bbb-122">String</span></span>|<span data-ttu-id="44bbb-123">笔记本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="44bbb-123">The unique identifier of the notebook.</span></span> <span data-ttu-id="44bbb-124">只读。</span><span class="sxs-lookup"><span data-stu-id="44bbb-124">Read-only.</span></span>|
|<span data-ttu-id="44bbb-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="44bbb-125">isDefault</span></span>|<span data-ttu-id="44bbb-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="44bbb-126">Boolean</span></span>|<span data-ttu-id="44bbb-127">指示这是否是用户的默认笔记本。</span><span class="sxs-lookup"><span data-stu-id="44bbb-127">Indicates whether this is the user's default notebook.</span></span> <span data-ttu-id="44bbb-128">只读。</span><span class="sxs-lookup"><span data-stu-id="44bbb-128">Read-only.</span></span>|
|<span data-ttu-id="44bbb-129">isShared</span><span class="sxs-lookup"><span data-stu-id="44bbb-129">isShared</span></span>|<span data-ttu-id="44bbb-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="44bbb-130">Boolean</span></span>|<span data-ttu-id="44bbb-131">指明笔记本是否为共享。</span><span class="sxs-lookup"><span data-stu-id="44bbb-131">Indicates whether the notebook is shared.</span></span> <span data-ttu-id="44bbb-132">如果是，笔记本的内容可供所有者以外的用户查看。</span><span class="sxs-lookup"><span data-stu-id="44bbb-132">If true, the contents of the notebook can be seen by people other than the owner.</span></span> <span data-ttu-id="44bbb-133">只读。</span><span class="sxs-lookup"><span data-stu-id="44bbb-133">Read-only.</span></span>|
|<span data-ttu-id="44bbb-134">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="44bbb-134">lastModifiedBy</span></span>|[<span data-ttu-id="44bbb-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="44bbb-135">identitySet</span></span>](identityset.md)|<span data-ttu-id="44bbb-p106">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="44bbb-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="44bbb-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44bbb-138">lastModifiedDateTime</span></span>|<span data-ttu-id="44bbb-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44bbb-139">DateTimeOffset</span></span>|<span data-ttu-id="44bbb-140">上次修改笔记本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="44bbb-140">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="44bbb-141">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="44bbb-141">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="44bbb-142">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="44bbb-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="44bbb-143">只读。</span><span class="sxs-lookup"><span data-stu-id="44bbb-143">Read-only.</span></span>|
|<span data-ttu-id="44bbb-144">links</span><span class="sxs-lookup"><span data-stu-id="44bbb-144">links</span></span>|[<span data-ttu-id="44bbb-145">notebookLinks</span><span class="sxs-lookup"><span data-stu-id="44bbb-145">notebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="44bbb-146">用于打开笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="44bbb-146">Links for opening the notebook.</span></span> <span data-ttu-id="44bbb-147">如果`oneNoteClientURL`安装了 OneNote 本机客户端, 则链接将在其中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="44bbb-147">The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed.</span></span> <span data-ttu-id="44bbb-148">该`oneNoteWebURL`链接将在 web 上的 OneNote 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="44bbb-148">The `oneNoteWebURL` link opens the notebook in OneNote on the web.</span></span>|
|<span data-ttu-id="44bbb-149">displayName</span><span class="sxs-lookup"><span data-stu-id="44bbb-149">displayName</span></span>|<span data-ttu-id="44bbb-150">字符串</span><span class="sxs-lookup"><span data-stu-id="44bbb-150">String</span></span>|<span data-ttu-id="44bbb-151">笔记本的名称。</span><span class="sxs-lookup"><span data-stu-id="44bbb-151">The name of the notebook.</span></span>|
|<span data-ttu-id="44bbb-152">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="44bbb-152">sectionGroupsUrl</span></span>|<span data-ttu-id="44bbb-153">String</span><span class="sxs-lookup"><span data-stu-id="44bbb-153">String</span></span>|<span data-ttu-id="44bbb-154">`sectionGroups`导航属性的 URL, 该 URL 将返回笔记本中的所有分区组。</span><span class="sxs-lookup"><span data-stu-id="44bbb-154">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook.</span></span> <span data-ttu-id="44bbb-155">只读。</span><span class="sxs-lookup"><span data-stu-id="44bbb-155">Read-only.</span></span>|
|<span data-ttu-id="44bbb-156">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="44bbb-156">sectionsUrl</span></span>|<span data-ttu-id="44bbb-157">String</span><span class="sxs-lookup"><span data-stu-id="44bbb-157">String</span></span>|<span data-ttu-id="44bbb-158">`sections`导航属性的 URL, 该 URL 将返回笔记本中的所有分区。</span><span class="sxs-lookup"><span data-stu-id="44bbb-158">The URL for the `sections` navigation property, which returns all the sections in the notebook.</span></span> <span data-ttu-id="44bbb-159">只读。</span><span class="sxs-lookup"><span data-stu-id="44bbb-159">Read-only.</span></span>|
|<span data-ttu-id="44bbb-160">自学</span><span class="sxs-lookup"><span data-stu-id="44bbb-160">self</span></span>|<span data-ttu-id="44bbb-161">String</span><span class="sxs-lookup"><span data-stu-id="44bbb-161">String</span></span>|<span data-ttu-id="44bbb-162">终结点，您可在此处获取关于笔记本的详细信息。</span><span class="sxs-lookup"><span data-stu-id="44bbb-162">The endpoint where you can get details about the notebook.</span></span> <span data-ttu-id="44bbb-163">只读。</span><span class="sxs-lookup"><span data-stu-id="44bbb-163">Read-only.</span></span>|
|<span data-ttu-id="44bbb-164">userRole</span><span class="sxs-lookup"><span data-stu-id="44bbb-164">userRole</span></span>|<span data-ttu-id="44bbb-165">String</span><span class="sxs-lookup"><span data-stu-id="44bbb-165">String</span></span>|<span data-ttu-id="44bbb-166">可能的值是：`Owner`、`Contributor`、`Reader`、`None`。</span><span class="sxs-lookup"><span data-stu-id="44bbb-166">Possible values are: `Owner`, `Contributor`, `Reader`, `None`.</span></span> <span data-ttu-id="44bbb-167">Owner 表示对笔记本的所有者级别访问。</span><span class="sxs-lookup"><span data-stu-id="44bbb-167">Owner represents owner-level access to the notebook.</span></span> <span data-ttu-id="44bbb-168">参与者表示对笔记本的读/写访问权限。</span><span class="sxs-lookup"><span data-stu-id="44bbb-168">Contributor represents read/write access to the notebook.</span></span> <span data-ttu-id="44bbb-169">读取器表示对笔记本的只读访问。</span><span class="sxs-lookup"><span data-stu-id="44bbb-169">Reader represents read-only access to the notebook.</span></span> <span data-ttu-id="44bbb-170">只读。</span><span class="sxs-lookup"><span data-stu-id="44bbb-170">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44bbb-171">关系</span><span class="sxs-lookup"><span data-stu-id="44bbb-171">Relationships</span></span>
| <span data-ttu-id="44bbb-172">关系</span><span class="sxs-lookup"><span data-stu-id="44bbb-172">Relationship</span></span> | <span data-ttu-id="44bbb-173">类型</span><span class="sxs-lookup"><span data-stu-id="44bbb-173">Type</span></span>   |<span data-ttu-id="44bbb-174">说明</span><span class="sxs-lookup"><span data-stu-id="44bbb-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44bbb-175">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="44bbb-175">sectionGroups</span></span>|<span data-ttu-id="44bbb-176">[sectionGroup](sectiongroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="44bbb-176">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="44bbb-177">笔记本中的分区组。</span><span class="sxs-lookup"><span data-stu-id="44bbb-177">The section groups in the notebook.</span></span> <span data-ttu-id="44bbb-178">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="44bbb-178">Read-only.</span></span> <span data-ttu-id="44bbb-179">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="44bbb-179">Nullable.</span></span>|
|<span data-ttu-id="44bbb-180">sections</span><span class="sxs-lookup"><span data-stu-id="44bbb-180">sections</span></span>|<span data-ttu-id="44bbb-181">[onenoteSection](onenotesection.md)集合</span><span class="sxs-lookup"><span data-stu-id="44bbb-181">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="44bbb-182">笔记本中的分区。</span><span class="sxs-lookup"><span data-stu-id="44bbb-182">The sections in the notebook.</span></span> <span data-ttu-id="44bbb-183">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="44bbb-183">Read-only.</span></span> <span data-ttu-id="44bbb-184">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="44bbb-184">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="44bbb-185">方法</span><span class="sxs-lookup"><span data-stu-id="44bbb-185">Methods</span></span>

| <span data-ttu-id="44bbb-186">方法</span><span class="sxs-lookup"><span data-stu-id="44bbb-186">Method</span></span>           | <span data-ttu-id="44bbb-187">返回类型</span><span class="sxs-lookup"><span data-stu-id="44bbb-187">Return Type</span></span>    |<span data-ttu-id="44bbb-188">说明</span><span class="sxs-lookup"><span data-stu-id="44bbb-188">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="44bbb-189">获取笔记本</span><span class="sxs-lookup"><span data-stu-id="44bbb-189">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="44bbb-190">笔记</span><span class="sxs-lookup"><span data-stu-id="44bbb-190">notebook</span></span>](notebook.md) |<span data-ttu-id="44bbb-191">读取笔记本的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="44bbb-191">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="44bbb-192">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="44bbb-192">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="44bbb-193">[recentNotebook](recentnotebook.md)集合</span><span class="sxs-lookup"><span data-stu-id="44bbb-193">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="44bbb-194">获取用户最近访问过的一组笔记本。</span><span class="sxs-lookup"><span data-stu-id="44bbb-194">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="44bbb-195">getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="44bbb-195">getNotebookFromWebUrl</span></span>](../api/notebook-getnotebookfromweburl.md) | [<span data-ttu-id="44bbb-196">笔记</span><span class="sxs-lookup"><span data-stu-id="44bbb-196">notebook</span></span>](notebook.md) | <span data-ttu-id="44bbb-197">使用 URL 路径检索笔记本对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="44bbb-197">Retrieve the properties and relationships of a notebook object using its URL path.</span></span> |
|[<span data-ttu-id="44bbb-198">创建分区组</span><span class="sxs-lookup"><span data-stu-id="44bbb-198">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="44bbb-199">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="44bbb-199">sectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="44bbb-200">通过发布到指定笔记本中的 sectionGroups 集合创建分区组。</span><span class="sxs-lookup"><span data-stu-id="44bbb-200">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="44bbb-201">列出分区组</span><span class="sxs-lookup"><span data-stu-id="44bbb-201">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="44bbb-202">[sectionGroup](sectiongroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="44bbb-202">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="44bbb-203">获取指定笔记本中的分区组的集合。</span><span class="sxs-lookup"><span data-stu-id="44bbb-203">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="44bbb-204">创建分区</span><span class="sxs-lookup"><span data-stu-id="44bbb-204">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="44bbb-205">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="44bbb-205">onenoteSection</span></span>](onenotesection.md)| <span data-ttu-id="44bbb-206">通过发布到指定笔记本中的 section 集合来创建一个分区。</span><span class="sxs-lookup"><span data-stu-id="44bbb-206">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="44bbb-207">列出节</span><span class="sxs-lookup"><span data-stu-id="44bbb-207">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="44bbb-208">[onenoteSection](onenotesection.md)集合</span><span class="sxs-lookup"><span data-stu-id="44bbb-208">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="44bbb-209">获取指定笔记本中的分区集合。</span><span class="sxs-lookup"><span data-stu-id="44bbb-209">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="44bbb-210">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="44bbb-210">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="44bbb-211">无</span><span class="sxs-lookup"><span data-stu-id="44bbb-211">None</span></span> | <span data-ttu-id="44bbb-212">复制笔记本。</span><span class="sxs-lookup"><span data-stu-id="44bbb-212">Copies a notebook.</span></span>|

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
