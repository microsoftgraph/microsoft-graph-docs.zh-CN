---
title: section 资源类型
description: OneNote 笔记本中的分区。分区可包含页面。
localization_priority: Normal
ms.openlocfilehash: 181fa3399f13d0490d9cd7d4599d8208633107b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831849"
---
# <a name="section-resource-type"></a><span data-ttu-id="e2578-104">section 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2578-104">section resource type</span></span>

> <span data-ttu-id="e2578-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e2578-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2578-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e2578-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2578-p103">OneNote 笔记本中的分区。分区可包含页面。</span><span class="sxs-lookup"><span data-stu-id="e2578-p103">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2578-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2578-109">JSON representation</span></span>

<span data-ttu-id="e2578-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2578-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="e2578-111">属性</span><span class="sxs-lookup"><span data-stu-id="e2578-111">Properties</span></span>
| <span data-ttu-id="e2578-112">属性</span><span class="sxs-lookup"><span data-stu-id="e2578-112">Property</span></span>     | <span data-ttu-id="e2578-113">类型</span><span class="sxs-lookup"><span data-stu-id="e2578-113">Type</span></span>   |<span data-ttu-id="e2578-114">说明</span><span class="sxs-lookup"><span data-stu-id="e2578-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2578-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="e2578-115">createdBy</span></span>|[<span data-ttu-id="e2578-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="e2578-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="e2578-p104">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="e2578-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="e2578-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2578-119">createdDateTime</span></span>|<span data-ttu-id="e2578-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2578-120">DateTimeOffset</span></span>|<span data-ttu-id="e2578-p105">分区的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="e2578-p105">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="e2578-125">id</span><span class="sxs-lookup"><span data-stu-id="e2578-125">id</span></span>|<span data-ttu-id="e2578-126">字符串</span><span class="sxs-lookup"><span data-stu-id="e2578-126">String</span></span>|<span data-ttu-id="e2578-p106">分区的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="e2578-p106">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="e2578-129">isDefault</span><span class="sxs-lookup"><span data-stu-id="e2578-129">isDefault</span></span>|<span data-ttu-id="e2578-130">布尔</span><span class="sxs-lookup"><span data-stu-id="e2578-130">Boolean</span></span>|<span data-ttu-id="e2578-p107">指示其是否是用户的默认分区。只读。</span><span class="sxs-lookup"><span data-stu-id="e2578-p107">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="e2578-133">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e2578-133">lastModifiedBy</span></span>|[<span data-ttu-id="e2578-134">identitySet</span><span class="sxs-lookup"><span data-stu-id="e2578-134">identitySet</span></span>](identityset.md)|<span data-ttu-id="e2578-p108">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="e2578-p108">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="e2578-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2578-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e2578-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2578-138">DateTimeOffset</span></span>|<span data-ttu-id="e2578-p109">上次修改分区的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="e2578-p109">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="e2578-143">links</span><span class="sxs-lookup"><span data-stu-id="e2578-143">links</span></span>|[<span data-ttu-id="e2578-144">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="e2578-144">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="e2578-p110">用于打开分区的链接。如果安装了 OneNote 本机客户端，则 `oneNoteClientURL` 链接将在其中打开分区。`oneNoteWebURL` 将在 OneNote Online 中打开分区。</span><span class="sxs-lookup"><span data-stu-id="e2578-p110">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="e2578-148">displayName</span><span class="sxs-lookup"><span data-stu-id="e2578-148">displayName</span></span>|<span data-ttu-id="e2578-149">String</span><span class="sxs-lookup"><span data-stu-id="e2578-149">String</span></span>|<span data-ttu-id="e2578-150">分区名称。</span><span class="sxs-lookup"><span data-stu-id="e2578-150">The name of the section.</span></span> |
|<span data-ttu-id="e2578-151">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="e2578-151">pagesUrl</span></span>|<span data-ttu-id="e2578-152">String</span><span class="sxs-lookup"><span data-stu-id="e2578-152">String</span></span>|<span data-ttu-id="e2578-p111">可以在其中获取分区中所有页面的详细信息的 `pages` 终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="e2578-p111">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="e2578-155">self</span><span class="sxs-lookup"><span data-stu-id="e2578-155">self</span></span>|<span data-ttu-id="e2578-156">字符串</span><span class="sxs-lookup"><span data-stu-id="e2578-156">String</span></span>|<span data-ttu-id="e2578-p112">可以在其中获取关于分区的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="e2578-p112">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2578-159">关系</span><span class="sxs-lookup"><span data-stu-id="e2578-159">Relationships</span></span>
| <span data-ttu-id="e2578-160">关系</span><span class="sxs-lookup"><span data-stu-id="e2578-160">Relationship</span></span> | <span data-ttu-id="e2578-161">类型</span><span class="sxs-lookup"><span data-stu-id="e2578-161">Type</span></span>   |<span data-ttu-id="e2578-162">说明</span><span class="sxs-lookup"><span data-stu-id="e2578-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2578-163">pages</span><span class="sxs-lookup"><span data-stu-id="e2578-163">pages</span></span>|<span data-ttu-id="e2578-164">[Page](page.md) collection</span><span class="sxs-lookup"><span data-stu-id="e2578-164">[Page](page.md) collection</span></span>|<span data-ttu-id="e2578-p113">分区中的页面集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e2578-p113">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="e2578-168">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="e2578-168">parentNotebook</span></span>|[<span data-ttu-id="e2578-169">Notebook</span><span class="sxs-lookup"><span data-stu-id="e2578-169">Notebook</span></span>](notebook.md)|<span data-ttu-id="e2578-p114">包含分区的笔记本。只读。</span><span class="sxs-lookup"><span data-stu-id="e2578-p114">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="e2578-172">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="e2578-172">parentSectionGroup</span></span>|[<span data-ttu-id="e2578-173">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="e2578-173">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="e2578-p115">包含分区的分区组。只读。</span><span class="sxs-lookup"><span data-stu-id="e2578-p115">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="e2578-176">方法</span><span class="sxs-lookup"><span data-stu-id="e2578-176">Methods</span></span>

| <span data-ttu-id="e2578-177">方法</span><span class="sxs-lookup"><span data-stu-id="e2578-177">Method</span></span>           | <span data-ttu-id="e2578-178">返回类型</span><span class="sxs-lookup"><span data-stu-id="e2578-178">Return Type</span></span>    |<span data-ttu-id="e2578-179">说明</span><span class="sxs-lookup"><span data-stu-id="e2578-179">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e2578-180">Get section</span><span class="sxs-lookup"><span data-stu-id="e2578-180">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="e2578-181">Section</span><span class="sxs-lookup"><span data-stu-id="e2578-181">Section</span></span>](section.md) |<span data-ttu-id="e2578-182">读取分区的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2578-182">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="e2578-183">Create page</span><span class="sxs-lookup"><span data-stu-id="e2578-183">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="e2578-184">页面</span><span class="sxs-lookup"><span data-stu-id="e2578-184">Page</span></span>](page.md)| <span data-ttu-id="e2578-185">通过发布到指定分区中的页面集合创建页面。</span><span class="sxs-lookup"><span data-stu-id="e2578-185">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="e2578-186">List pages</span><span class="sxs-lookup"><span data-stu-id="e2578-186">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="e2578-187">[Page](page.md) collection</span><span class="sxs-lookup"><span data-stu-id="e2578-187">[Page](page.md) collection</span></span>| <span data-ttu-id="e2578-188">获取指定分区中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="e2578-188">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="e2578-189">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="e2578-189">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="e2578-190">无</span><span class="sxs-lookup"><span data-stu-id="e2578-190">None</span></span>|<span data-ttu-id="e2578-191">将分区复制到特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="e2578-191">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="e2578-192">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="e2578-192">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="e2578-193">无</span><span class="sxs-lookup"><span data-stu-id="e2578-193">None</span></span>|<span data-ttu-id="e2578-194">将分区复制到特定分区组。</span><span class="sxs-lookup"><span data-stu-id="e2578-194">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
