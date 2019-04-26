---
title: 部分资源类型
description: OneNote 笔记本中的分区。 分区可包含页面。
localization_priority: Normal
ms.openlocfilehash: faecf31ad09f3ea3b5614480fc051ad1054d442b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562942"
---
# <a name="section-resource-type"></a><span data-ttu-id="e53c4-104">部分资源类型</span><span class="sxs-lookup"><span data-stu-id="e53c4-104">section resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e53c4-105">OneNote 笔记本中的分区。</span><span class="sxs-lookup"><span data-stu-id="e53c4-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="e53c4-106">分区可包含页面。</span><span class="sxs-lookup"><span data-stu-id="e53c4-106">Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e53c4-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e53c4-107">JSON representation</span></span>

<span data-ttu-id="e53c4-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e53c4-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="e53c4-109">属性</span><span class="sxs-lookup"><span data-stu-id="e53c4-109">Properties</span></span>
| <span data-ttu-id="e53c4-110">属性</span><span class="sxs-lookup"><span data-stu-id="e53c4-110">Property</span></span>     | <span data-ttu-id="e53c4-111">类型</span><span class="sxs-lookup"><span data-stu-id="e53c4-111">Type</span></span>   |<span data-ttu-id="e53c4-112">说明</span><span class="sxs-lookup"><span data-stu-id="e53c4-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e53c4-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="e53c4-113">createdBy</span></span>|[<span data-ttu-id="e53c4-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="e53c4-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="e53c4-p103">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="e53c4-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="e53c4-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e53c4-117">createdDateTime</span></span>|<span data-ttu-id="e53c4-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e53c4-118">DateTimeOffset</span></span>|<span data-ttu-id="e53c4-119">节的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e53c4-119">The date and time when the section was created.</span></span> <span data-ttu-id="e53c4-120">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e53c4-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e53c4-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="e53c4-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e53c4-122">只读。</span><span class="sxs-lookup"><span data-stu-id="e53c4-122">Read-only.</span></span>|
|<span data-ttu-id="e53c4-123">id</span><span class="sxs-lookup"><span data-stu-id="e53c4-123">id</span></span>|<span data-ttu-id="e53c4-124">String</span><span class="sxs-lookup"><span data-stu-id="e53c4-124">String</span></span>|<span data-ttu-id="e53c4-125">节的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e53c4-125">The unique identifier of the section.</span></span>  <span data-ttu-id="e53c4-126">只读。</span><span class="sxs-lookup"><span data-stu-id="e53c4-126">Read-only.</span></span>|
|<span data-ttu-id="e53c4-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="e53c4-127">isDefault</span></span>|<span data-ttu-id="e53c4-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="e53c4-128">Boolean</span></span>|<span data-ttu-id="e53c4-129">指示是否为用户的默认节。</span><span class="sxs-lookup"><span data-stu-id="e53c4-129">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="e53c4-130">只读。</span><span class="sxs-lookup"><span data-stu-id="e53c4-130">Read-only.</span></span>|
|<span data-ttu-id="e53c4-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e53c4-131">lastModifiedBy</span></span>|[<span data-ttu-id="e53c4-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="e53c4-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="e53c4-p107">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="e53c4-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="e53c4-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e53c4-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e53c4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e53c4-136">DateTimeOffset</span></span>|<span data-ttu-id="e53c4-137">上次修改节的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e53c4-137">The date and time when the section was last modified.</span></span> <span data-ttu-id="e53c4-138">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e53c4-138">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e53c4-139">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="e53c4-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e53c4-140">只读。</span><span class="sxs-lookup"><span data-stu-id="e53c4-140">Read-only.</span></span>|
|<span data-ttu-id="e53c4-141">links</span><span class="sxs-lookup"><span data-stu-id="e53c4-141">links</span></span>|[<span data-ttu-id="e53c4-142">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="e53c4-142">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="e53c4-143">用于打开分区的链接。</span><span class="sxs-lookup"><span data-stu-id="e53c4-143">Links for opening the section.</span></span> <span data-ttu-id="e53c4-144">如果`oneNoteClientURL`安装了 OneNote 本机客户端, 则链接将在其中打开分区。</span><span class="sxs-lookup"><span data-stu-id="e53c4-144">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="e53c4-145">`oneNoteWebURL`链接将在 OneNote Online 中打开分区。</span><span class="sxs-lookup"><span data-stu-id="e53c4-145">The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="e53c4-146">displayName</span><span class="sxs-lookup"><span data-stu-id="e53c4-146">displayName</span></span>|<span data-ttu-id="e53c4-147">String</span><span class="sxs-lookup"><span data-stu-id="e53c4-147">String</span></span>|<span data-ttu-id="e53c4-148">节的名称。</span><span class="sxs-lookup"><span data-stu-id="e53c4-148">The name of the section.</span></span> |
|<span data-ttu-id="e53c4-149">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="e53c4-149">pagesUrl</span></span>|<span data-ttu-id="e53c4-150">String</span><span class="sxs-lookup"><span data-stu-id="e53c4-150">String</span></span>|<span data-ttu-id="e53c4-151">`pages`终结点, 您可在其中获取该部分中所有页面的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e53c4-151">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="e53c4-152">只读。</span><span class="sxs-lookup"><span data-stu-id="e53c4-152">Read-only.</span></span>|
|<span data-ttu-id="e53c4-153">自学</span><span class="sxs-lookup"><span data-stu-id="e53c4-153">self</span></span>|<span data-ttu-id="e53c4-154">String</span><span class="sxs-lookup"><span data-stu-id="e53c4-154">String</span></span>|<span data-ttu-id="e53c4-155">终结点，您可在此处获取关于节的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e53c4-155">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="e53c4-156">只读。</span><span class="sxs-lookup"><span data-stu-id="e53c4-156">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e53c4-157">关系</span><span class="sxs-lookup"><span data-stu-id="e53c4-157">Relationships</span></span>
| <span data-ttu-id="e53c4-158">关系</span><span class="sxs-lookup"><span data-stu-id="e53c4-158">Relationship</span></span> | <span data-ttu-id="e53c4-159">类型</span><span class="sxs-lookup"><span data-stu-id="e53c4-159">Type</span></span>   |<span data-ttu-id="e53c4-160">说明</span><span class="sxs-lookup"><span data-stu-id="e53c4-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e53c4-161">pages</span><span class="sxs-lookup"><span data-stu-id="e53c4-161">pages</span></span>|<span data-ttu-id="e53c4-162">[页面](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="e53c4-162">[Page](page.md) collection</span></span>|<span data-ttu-id="e53c4-163">分区中的一组页面。</span><span class="sxs-lookup"><span data-stu-id="e53c4-163">The collection of pages in the section.</span></span>  <span data-ttu-id="e53c4-164">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="e53c4-164">Read-only.</span></span> <span data-ttu-id="e53c4-165">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e53c4-165">Nullable.</span></span>|
|<span data-ttu-id="e53c4-166">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="e53c4-166">parentNotebook</span></span>|[<span data-ttu-id="e53c4-167">Notebook</span><span class="sxs-lookup"><span data-stu-id="e53c4-167">Notebook</span></span>](notebook.md)|<span data-ttu-id="e53c4-168">包含该部分的笔记本。</span><span class="sxs-lookup"><span data-stu-id="e53c4-168">The notebook that contains the section.</span></span>  <span data-ttu-id="e53c4-169">只读。</span><span class="sxs-lookup"><span data-stu-id="e53c4-169">Read-only.</span></span>|
|<span data-ttu-id="e53c4-170">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="e53c4-170">parentSectionGroup</span></span>|[<span data-ttu-id="e53c4-171">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="e53c4-171">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="e53c4-172">包含节的节组。</span><span class="sxs-lookup"><span data-stu-id="e53c4-172">The section group that contains the section.</span></span>  <span data-ttu-id="e53c4-173">只读的。</span><span class="sxs-lookup"><span data-stu-id="e53c4-173">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="e53c4-174">方法</span><span class="sxs-lookup"><span data-stu-id="e53c4-174">Methods</span></span>

| <span data-ttu-id="e53c4-175">方法</span><span class="sxs-lookup"><span data-stu-id="e53c4-175">Method</span></span>           | <span data-ttu-id="e53c4-176">返回类型</span><span class="sxs-lookup"><span data-stu-id="e53c4-176">Return Type</span></span>    |<span data-ttu-id="e53c4-177">说明</span><span class="sxs-lookup"><span data-stu-id="e53c4-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e53c4-178">获取分区</span><span class="sxs-lookup"><span data-stu-id="e53c4-178">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="e53c4-179">Section</span><span class="sxs-lookup"><span data-stu-id="e53c4-179">Section</span></span>](section.md) |<span data-ttu-id="e53c4-180">读取节的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e53c4-180">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="e53c4-181">创建页面</span><span class="sxs-lookup"><span data-stu-id="e53c4-181">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="e53c4-182">Page</span><span class="sxs-lookup"><span data-stu-id="e53c4-182">Page</span></span>](page.md)| <span data-ttu-id="e53c4-183">通过发布到指定分区中的 pages 集合来创建页面。</span><span class="sxs-lookup"><span data-stu-id="e53c4-183">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="e53c4-184">列出页面</span><span class="sxs-lookup"><span data-stu-id="e53c4-184">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="e53c4-185">[页面](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="e53c4-185">[Page](page.md) collection</span></span>| <span data-ttu-id="e53c4-186">获取指定节中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="e53c4-186">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="e53c4-187">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="e53c4-187">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="e53c4-188">无</span><span class="sxs-lookup"><span data-stu-id="e53c4-188">None</span></span>|<span data-ttu-id="e53c4-189">将分区复制到特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="e53c4-189">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="e53c4-190">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="e53c4-190">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="e53c4-191">无</span><span class="sxs-lookup"><span data-stu-id="e53c4-191">None</span></span>|<span data-ttu-id="e53c4-192">将分区复制到特定分区组。</span><span class="sxs-lookup"><span data-stu-id="e53c4-192">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/section.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
