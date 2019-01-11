---
title: section 资源类型
description: OneNote 笔记本中的分区。分区可包含页面。
localization_priority: Normal
ms.openlocfilehash: f9cb5a8e3ddf9cf4a045103e4ecc7909653d797c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853233"
---
# <a name="section-resource-type"></a><span data-ttu-id="612ed-104">section 资源类型</span><span class="sxs-lookup"><span data-stu-id="612ed-104">section resource type</span></span>

<span data-ttu-id="612ed-p102">OneNote 笔记本中的分区。分区可包含页面。</span><span class="sxs-lookup"><span data-stu-id="612ed-p102">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="612ed-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="612ed-107">JSON representation</span></span>

<span data-ttu-id="612ed-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="612ed-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
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
## <a name="properties"></a><span data-ttu-id="612ed-109">属性</span><span class="sxs-lookup"><span data-stu-id="612ed-109">Properties</span></span>
| <span data-ttu-id="612ed-110">属性</span><span class="sxs-lookup"><span data-stu-id="612ed-110">Property</span></span>     | <span data-ttu-id="612ed-111">类型</span><span class="sxs-lookup"><span data-stu-id="612ed-111">Type</span></span>   |<span data-ttu-id="612ed-112">说明</span><span class="sxs-lookup"><span data-stu-id="612ed-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="612ed-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="612ed-113">createdBy</span></span>|[<span data-ttu-id="612ed-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="612ed-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="612ed-p103">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="612ed-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="612ed-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="612ed-117">createdDateTime</span></span>|<span data-ttu-id="612ed-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="612ed-118">DateTimeOffset</span></span>|<span data-ttu-id="612ed-p104">分区的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="612ed-p104">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="612ed-123">id</span><span class="sxs-lookup"><span data-stu-id="612ed-123">id</span></span>|<span data-ttu-id="612ed-124">字符串</span><span class="sxs-lookup"><span data-stu-id="612ed-124">String</span></span>|<span data-ttu-id="612ed-p105">分区的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="612ed-p105">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="612ed-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="612ed-127">isDefault</span></span>|<span data-ttu-id="612ed-128">布尔</span><span class="sxs-lookup"><span data-stu-id="612ed-128">Boolean</span></span>|<span data-ttu-id="612ed-p106">指示其是否是用户的默认分区。只读。</span><span class="sxs-lookup"><span data-stu-id="612ed-p106">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="612ed-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="612ed-131">lastModifiedBy</span></span>|[<span data-ttu-id="612ed-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="612ed-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="612ed-p107">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="612ed-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="612ed-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="612ed-135">lastModifiedDateTime</span></span>|<span data-ttu-id="612ed-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="612ed-136">DateTimeOffset</span></span>|<span data-ttu-id="612ed-p108">上次修改分区的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="612ed-p108">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="612ed-141">links</span><span class="sxs-lookup"><span data-stu-id="612ed-141">links</span></span>|[<span data-ttu-id="612ed-142">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="612ed-142">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="612ed-p109">用于打开分区的链接。如果安装了 OneNote 本机客户端，则 `oneNoteClientURL` 链接将在其中打开分区。`oneNoteWebURL` 将在 OneNote Online 中打开分区。</span><span class="sxs-lookup"><span data-stu-id="612ed-p109">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="612ed-146">displayName</span><span class="sxs-lookup"><span data-stu-id="612ed-146">displayName</span></span>|<span data-ttu-id="612ed-147">String</span><span class="sxs-lookup"><span data-stu-id="612ed-147">String</span></span>|<span data-ttu-id="612ed-148">分区名称。</span><span class="sxs-lookup"><span data-stu-id="612ed-148">The name of the section.</span></span> |
|<span data-ttu-id="612ed-149">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="612ed-149">pagesUrl</span></span>|<span data-ttu-id="612ed-150">String</span><span class="sxs-lookup"><span data-stu-id="612ed-150">String</span></span>|<span data-ttu-id="612ed-p110">可以在其中获取分区中所有页面的详细信息的 `pages` 终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="612ed-p110">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="612ed-153">self</span><span class="sxs-lookup"><span data-stu-id="612ed-153">self</span></span>|<span data-ttu-id="612ed-154">字符串</span><span class="sxs-lookup"><span data-stu-id="612ed-154">String</span></span>|<span data-ttu-id="612ed-p111">可以在其中获取关于分区的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="612ed-p111">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="612ed-157">关系</span><span class="sxs-lookup"><span data-stu-id="612ed-157">Relationships</span></span>
| <span data-ttu-id="612ed-158">关系</span><span class="sxs-lookup"><span data-stu-id="612ed-158">Relationship</span></span> | <span data-ttu-id="612ed-159">类型</span><span class="sxs-lookup"><span data-stu-id="612ed-159">Type</span></span>   |<span data-ttu-id="612ed-160">说明</span><span class="sxs-lookup"><span data-stu-id="612ed-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="612ed-161">pages</span><span class="sxs-lookup"><span data-stu-id="612ed-161">pages</span></span>|<span data-ttu-id="612ed-162">[OnenotePage](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="612ed-162">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="612ed-p112">分区中的页面集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="612ed-p112">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="612ed-166">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="612ed-166">parentNotebook</span></span>|[<span data-ttu-id="612ed-167">Notebook</span><span class="sxs-lookup"><span data-stu-id="612ed-167">Notebook</span></span>](notebook.md)|<span data-ttu-id="612ed-p113">包含分区的笔记本。只读。</span><span class="sxs-lookup"><span data-stu-id="612ed-p113">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="612ed-170">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="612ed-170">parentSectionGroup</span></span>|[<span data-ttu-id="612ed-171">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="612ed-171">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="612ed-p114">包含分区的分区组。只读。</span><span class="sxs-lookup"><span data-stu-id="612ed-p114">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="612ed-174">方法</span><span class="sxs-lookup"><span data-stu-id="612ed-174">Methods</span></span>

| <span data-ttu-id="612ed-175">方法</span><span class="sxs-lookup"><span data-stu-id="612ed-175">Method</span></span>           | <span data-ttu-id="612ed-176">返回类型</span><span class="sxs-lookup"><span data-stu-id="612ed-176">Return Type</span></span>    |<span data-ttu-id="612ed-177">说明</span><span class="sxs-lookup"><span data-stu-id="612ed-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="612ed-178">Get section</span><span class="sxs-lookup"><span data-stu-id="612ed-178">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="612ed-179">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="612ed-179">OnenoteSection</span></span>](section.md) |<span data-ttu-id="612ed-180">读取分区的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="612ed-180">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="612ed-181">Create page</span><span class="sxs-lookup"><span data-stu-id="612ed-181">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="612ed-182">页面</span><span class="sxs-lookup"><span data-stu-id="612ed-182">Page</span></span>](page.md)| <span data-ttu-id="612ed-183">通过发布到指定分区中的页面集合创建页面。</span><span class="sxs-lookup"><span data-stu-id="612ed-183">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="612ed-184">List pages</span><span class="sxs-lookup"><span data-stu-id="612ed-184">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="612ed-185">[Page](page.md) collection</span><span class="sxs-lookup"><span data-stu-id="612ed-185">[Page](page.md) collection</span></span>| <span data-ttu-id="612ed-186">获取指定分区中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="612ed-186">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="612ed-187">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="612ed-187">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="612ed-188">无</span><span class="sxs-lookup"><span data-stu-id="612ed-188">None</span></span>|<span data-ttu-id="612ed-189">将分区复制到特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="612ed-189">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="612ed-190">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="612ed-190">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="612ed-191">无</span><span class="sxs-lookup"><span data-stu-id="612ed-191">None</span></span>|<span data-ttu-id="612ed-192">将分区复制到特定分区组。</span><span class="sxs-lookup"><span data-stu-id="612ed-192">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
