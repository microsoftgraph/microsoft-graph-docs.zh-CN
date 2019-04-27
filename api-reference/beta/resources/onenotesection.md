---
title: onenoteSection 资源类型
description: OneNote 笔记本中的分区。 分区可包含页面。
localization_priority: Normal
ms.openlocfilehash: d262065f46052c1cae55b42babaa91a2e065d3ef
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348565"
---
# <a name="onenotesection-resource-type"></a><span data-ttu-id="8c975-104">onenoteSection 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c975-104">onenoteSection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c975-105">OneNote 笔记本中的分区。</span><span class="sxs-lookup"><span data-stu-id="8c975-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="8c975-106">分区可包含页面。</span><span class="sxs-lookup"><span data-stu-id="8c975-106">Sections can contain pages.</span></span>

## <a name="properties"></a><span data-ttu-id="8c975-107">属性</span><span class="sxs-lookup"><span data-stu-id="8c975-107">Properties</span></span>
| <span data-ttu-id="8c975-108">属性</span><span class="sxs-lookup"><span data-stu-id="8c975-108">Property</span></span>     | <span data-ttu-id="8c975-109">类型</span><span class="sxs-lookup"><span data-stu-id="8c975-109">Type</span></span>   |<span data-ttu-id="8c975-110">说明</span><span class="sxs-lookup"><span data-stu-id="8c975-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c975-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="8c975-111">createdBy</span></span>|[<span data-ttu-id="8c975-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="8c975-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="8c975-p103">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="8c975-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="8c975-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c975-115">createdDateTime</span></span>|<span data-ttu-id="8c975-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c975-116">DateTimeOffset</span></span>|<span data-ttu-id="8c975-117">节的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8c975-117">The date and time when the section was created.</span></span> <span data-ttu-id="8c975-118">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="8c975-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8c975-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="8c975-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="8c975-120">只读。</span><span class="sxs-lookup"><span data-stu-id="8c975-120">Read-only.</span></span>|
|<span data-ttu-id="8c975-121">id</span><span class="sxs-lookup"><span data-stu-id="8c975-121">id</span></span>|<span data-ttu-id="8c975-122">String</span><span class="sxs-lookup"><span data-stu-id="8c975-122">String</span></span>|<span data-ttu-id="8c975-123">节的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8c975-123">The unique identifier of the section.</span></span>  <span data-ttu-id="8c975-124">只读。</span><span class="sxs-lookup"><span data-stu-id="8c975-124">Read-only.</span></span>|
|<span data-ttu-id="8c975-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="8c975-125">isDefault</span></span>|<span data-ttu-id="8c975-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c975-126">Boolean</span></span>|<span data-ttu-id="8c975-127">指示是否为用户的默认节。</span><span class="sxs-lookup"><span data-stu-id="8c975-127">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="8c975-128">只读。</span><span class="sxs-lookup"><span data-stu-id="8c975-128">Read-only.</span></span>|
|<span data-ttu-id="8c975-129">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8c975-129">lastModifiedBy</span></span>|[<span data-ttu-id="8c975-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="8c975-130">identitySet</span></span>](identityset.md)|<span data-ttu-id="8c975-p107">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="8c975-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="8c975-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c975-133">lastModifiedDateTime</span></span>|<span data-ttu-id="8c975-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c975-134">DateTimeOffset</span></span>|<span data-ttu-id="8c975-135">上次修改节的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8c975-135">The date and time when the section was last modified.</span></span> <span data-ttu-id="8c975-136">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="8c975-136">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8c975-137">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="8c975-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="8c975-138">只读。</span><span class="sxs-lookup"><span data-stu-id="8c975-138">Read-only.</span></span>|
|<span data-ttu-id="8c975-139">links</span><span class="sxs-lookup"><span data-stu-id="8c975-139">links</span></span>|[<span data-ttu-id="8c975-140">sectionLinks</span><span class="sxs-lookup"><span data-stu-id="8c975-140">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="8c975-141">用于打开分区的链接。</span><span class="sxs-lookup"><span data-stu-id="8c975-141">Links for opening the section.</span></span> <span data-ttu-id="8c975-142">如果`oneNoteClientURL`安装了 OneNote 本机客户端, 则链接将在其中打开分区。</span><span class="sxs-lookup"><span data-stu-id="8c975-142">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="8c975-143">`oneNoteWebURL`链接将在 OneNote Online 中打开分区。</span><span class="sxs-lookup"><span data-stu-id="8c975-143">The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="8c975-144">displayName</span><span class="sxs-lookup"><span data-stu-id="8c975-144">displayName</span></span>|<span data-ttu-id="8c975-145">String</span><span class="sxs-lookup"><span data-stu-id="8c975-145">String</span></span>|<span data-ttu-id="8c975-146">节的名称。</span><span class="sxs-lookup"><span data-stu-id="8c975-146">The name of the section.</span></span> |
|<span data-ttu-id="8c975-147">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="8c975-147">pagesUrl</span></span>|<span data-ttu-id="8c975-148">String</span><span class="sxs-lookup"><span data-stu-id="8c975-148">String</span></span>|<span data-ttu-id="8c975-149">`pages`终结点, 您可在其中获取该部分中所有页面的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8c975-149">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="8c975-150">只读。</span><span class="sxs-lookup"><span data-stu-id="8c975-150">Read-only.</span></span>|
|<span data-ttu-id="8c975-151">自学</span><span class="sxs-lookup"><span data-stu-id="8c975-151">self</span></span>|<span data-ttu-id="8c975-152">String</span><span class="sxs-lookup"><span data-stu-id="8c975-152">String</span></span>|<span data-ttu-id="8c975-153">终结点，您可在此处获取关于节的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8c975-153">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="8c975-154">只读。</span><span class="sxs-lookup"><span data-stu-id="8c975-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c975-155">关系</span><span class="sxs-lookup"><span data-stu-id="8c975-155">Relationships</span></span>
| <span data-ttu-id="8c975-156">关系</span><span class="sxs-lookup"><span data-stu-id="8c975-156">Relationship</span></span> | <span data-ttu-id="8c975-157">类型</span><span class="sxs-lookup"><span data-stu-id="8c975-157">Type</span></span>   |<span data-ttu-id="8c975-158">说明</span><span class="sxs-lookup"><span data-stu-id="8c975-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c975-159">pages</span><span class="sxs-lookup"><span data-stu-id="8c975-159">pages</span></span>|<span data-ttu-id="8c975-160">[onenotePage](onenotepage.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c975-160">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="8c975-161">分区中的一组页面。</span><span class="sxs-lookup"><span data-stu-id="8c975-161">The collection of pages in the section.</span></span>  <span data-ttu-id="8c975-162">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="8c975-162">Read-only.</span></span> <span data-ttu-id="8c975-163">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8c975-163">Nullable.</span></span>|
|<span data-ttu-id="8c975-164">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="8c975-164">parentNotebook</span></span>|[<span data-ttu-id="8c975-165">笔记</span><span class="sxs-lookup"><span data-stu-id="8c975-165">notebook</span></span>](notebook.md)|<span data-ttu-id="8c975-166">包含该部分的笔记本。</span><span class="sxs-lookup"><span data-stu-id="8c975-166">The notebook that contains the section.</span></span>  <span data-ttu-id="8c975-167">只读。</span><span class="sxs-lookup"><span data-stu-id="8c975-167">Read-only.</span></span>|
|<span data-ttu-id="8c975-168">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="8c975-168">parentSectionGroup</span></span>|[<span data-ttu-id="8c975-169">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="8c975-169">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="8c975-170">包含节的节组。</span><span class="sxs-lookup"><span data-stu-id="8c975-170">The section group that contains the section.</span></span>  <span data-ttu-id="8c975-171">只读的。</span><span class="sxs-lookup"><span data-stu-id="8c975-171">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="8c975-172">方法</span><span class="sxs-lookup"><span data-stu-id="8c975-172">Methods</span></span>

| <span data-ttu-id="8c975-173">方法</span><span class="sxs-lookup"><span data-stu-id="8c975-173">Method</span></span>           | <span data-ttu-id="8c975-174">返回类型</span><span class="sxs-lookup"><span data-stu-id="8c975-174">Return Type</span></span>    |<span data-ttu-id="8c975-175">说明</span><span class="sxs-lookup"><span data-stu-id="8c975-175">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8c975-176">获取分区</span><span class="sxs-lookup"><span data-stu-id="8c975-176">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="8c975-177">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="8c975-177">onenoteSection</span></span>](onenotesection.md) |<span data-ttu-id="8c975-178">读取节的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8c975-178">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="8c975-179">创建页面</span><span class="sxs-lookup"><span data-stu-id="8c975-179">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="8c975-180">onenotePage</span><span class="sxs-lookup"><span data-stu-id="8c975-180">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="8c975-181">通过发布到指定分区中的 pages 集合来创建页面。</span><span class="sxs-lookup"><span data-stu-id="8c975-181">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="8c975-182">列出页面</span><span class="sxs-lookup"><span data-stu-id="8c975-182">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="8c975-183">[onenotePage](onenotepage.md)集合</span><span class="sxs-lookup"><span data-stu-id="8c975-183">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="8c975-184">获取指定节中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="8c975-184">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="8c975-185">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="8c975-185">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="8c975-186">无</span><span class="sxs-lookup"><span data-stu-id="8c975-186">None</span></span>|<span data-ttu-id="8c975-187">将分区复制到特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="8c975-187">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="8c975-188">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="8c975-188">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="8c975-189">无</span><span class="sxs-lookup"><span data-stu-id="8c975-189">None</span></span>|<span data-ttu-id="8c975-190">将分区复制到特定分区组。</span><span class="sxs-lookup"><span data-stu-id="8c975-190">Copy the section to a specific section group.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8c975-191">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c975-191">JSON representation</span></span>

<span data-ttu-id="8c975-192">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c975-192">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
