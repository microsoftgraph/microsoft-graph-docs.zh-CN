---
title: onenoteSection 资源类型
description: OneNote 笔记本中的分区。 分区可包含页面。
localization_priority: Normal
ms.openlocfilehash: b07ea378a4338e22896d40065e35aa599db42832
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236627"
---
# <a name="onenotesection-resource-type"></a><span data-ttu-id="a1a93-104">onenoteSection 资源类型</span><span class="sxs-lookup"><span data-stu-id="a1a93-104">onenoteSection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1a93-105">OneNote 笔记本中的分区。</span><span class="sxs-lookup"><span data-stu-id="a1a93-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="a1a93-106">分区可包含页面。</span><span class="sxs-lookup"><span data-stu-id="a1a93-106">Sections can contain pages.</span></span>

## <a name="properties"></a><span data-ttu-id="a1a93-107">属性</span><span class="sxs-lookup"><span data-stu-id="a1a93-107">Properties</span></span>
| <span data-ttu-id="a1a93-108">属性</span><span class="sxs-lookup"><span data-stu-id="a1a93-108">Property</span></span>     | <span data-ttu-id="a1a93-109">类型</span><span class="sxs-lookup"><span data-stu-id="a1a93-109">Type</span></span>   |<span data-ttu-id="a1a93-110">说明</span><span class="sxs-lookup"><span data-stu-id="a1a93-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1a93-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="a1a93-111">createdBy</span></span>|[<span data-ttu-id="a1a93-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="a1a93-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="a1a93-p103">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="a1a93-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="a1a93-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1a93-115">createdDateTime</span></span>|<span data-ttu-id="a1a93-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1a93-116">DateTimeOffset</span></span>|<span data-ttu-id="a1a93-117">节的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a1a93-117">The date and time when the section was created.</span></span> <span data-ttu-id="a1a93-118">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="a1a93-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a1a93-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="a1a93-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a1a93-120">只读。</span><span class="sxs-lookup"><span data-stu-id="a1a93-120">Read-only.</span></span>|
|<span data-ttu-id="a1a93-121">id</span><span class="sxs-lookup"><span data-stu-id="a1a93-121">id</span></span>|<span data-ttu-id="a1a93-122">String</span><span class="sxs-lookup"><span data-stu-id="a1a93-122">String</span></span>|<span data-ttu-id="a1a93-123">节的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a1a93-123">The unique identifier of the section.</span></span>  <span data-ttu-id="a1a93-124">只读。</span><span class="sxs-lookup"><span data-stu-id="a1a93-124">Read-only.</span></span>|
|<span data-ttu-id="a1a93-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="a1a93-125">isDefault</span></span>|<span data-ttu-id="a1a93-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1a93-126">Boolean</span></span>|<span data-ttu-id="a1a93-127">指示是否为用户的默认节。</span><span class="sxs-lookup"><span data-stu-id="a1a93-127">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="a1a93-128">只读。</span><span class="sxs-lookup"><span data-stu-id="a1a93-128">Read-only.</span></span>|
|<span data-ttu-id="a1a93-129">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a1a93-129">lastModifiedBy</span></span>|[<span data-ttu-id="a1a93-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="a1a93-130">identitySet</span></span>](identityset.md)|<span data-ttu-id="a1a93-p107">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="a1a93-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="a1a93-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1a93-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a1a93-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1a93-134">DateTimeOffset</span></span>|<span data-ttu-id="a1a93-135">上次修改节的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a1a93-135">The date and time when the section was last modified.</span></span> <span data-ttu-id="a1a93-136">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="a1a93-136">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a1a93-137">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="a1a93-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a1a93-138">只读。</span><span class="sxs-lookup"><span data-stu-id="a1a93-138">Read-only.</span></span>|
|<span data-ttu-id="a1a93-139">links</span><span class="sxs-lookup"><span data-stu-id="a1a93-139">links</span></span>|[<span data-ttu-id="a1a93-140">sectionLinks</span><span class="sxs-lookup"><span data-stu-id="a1a93-140">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="a1a93-141">用于打开分区的链接。</span><span class="sxs-lookup"><span data-stu-id="a1a93-141">Links for opening the section.</span></span> <span data-ttu-id="a1a93-142">如果`oneNoteClientURL`安装了 OneNote 本机客户端, 则链接将在其中打开分区。</span><span class="sxs-lookup"><span data-stu-id="a1a93-142">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="a1a93-143">`oneNoteWebURL`链接将打开 web 上的 OneNote 中的分区。</span><span class="sxs-lookup"><span data-stu-id="a1a93-143">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="a1a93-144">displayName</span><span class="sxs-lookup"><span data-stu-id="a1a93-144">displayName</span></span>|<span data-ttu-id="a1a93-145">String</span><span class="sxs-lookup"><span data-stu-id="a1a93-145">String</span></span>|<span data-ttu-id="a1a93-146">节的名称。</span><span class="sxs-lookup"><span data-stu-id="a1a93-146">The name of the section.</span></span> |
|<span data-ttu-id="a1a93-147">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="a1a93-147">pagesUrl</span></span>|<span data-ttu-id="a1a93-148">String</span><span class="sxs-lookup"><span data-stu-id="a1a93-148">String</span></span>|<span data-ttu-id="a1a93-149">`pages`终结点, 您可在其中获取该部分中所有页面的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a1a93-149">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="a1a93-150">只读。</span><span class="sxs-lookup"><span data-stu-id="a1a93-150">Read-only.</span></span>|
|<span data-ttu-id="a1a93-151">自学</span><span class="sxs-lookup"><span data-stu-id="a1a93-151">self</span></span>|<span data-ttu-id="a1a93-152">String</span><span class="sxs-lookup"><span data-stu-id="a1a93-152">String</span></span>|<span data-ttu-id="a1a93-153">终结点，您可在此处获取关于节的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a1a93-153">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="a1a93-154">只读。</span><span class="sxs-lookup"><span data-stu-id="a1a93-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1a93-155">关系</span><span class="sxs-lookup"><span data-stu-id="a1a93-155">Relationships</span></span>
| <span data-ttu-id="a1a93-156">关系</span><span class="sxs-lookup"><span data-stu-id="a1a93-156">Relationship</span></span> | <span data-ttu-id="a1a93-157">类型</span><span class="sxs-lookup"><span data-stu-id="a1a93-157">Type</span></span>   |<span data-ttu-id="a1a93-158">说明</span><span class="sxs-lookup"><span data-stu-id="a1a93-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1a93-159">pages</span><span class="sxs-lookup"><span data-stu-id="a1a93-159">pages</span></span>|<span data-ttu-id="a1a93-160">[onenotePage](onenotepage.md)集合</span><span class="sxs-lookup"><span data-stu-id="a1a93-160">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="a1a93-161">分区中的一组页面。</span><span class="sxs-lookup"><span data-stu-id="a1a93-161">The collection of pages in the section.</span></span>  <span data-ttu-id="a1a93-162">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="a1a93-162">Read-only.</span></span> <span data-ttu-id="a1a93-163">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a1a93-163">Nullable.</span></span>|
|<span data-ttu-id="a1a93-164">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="a1a93-164">parentNotebook</span></span>|[<span data-ttu-id="a1a93-165">笔记</span><span class="sxs-lookup"><span data-stu-id="a1a93-165">notebook</span></span>](notebook.md)|<span data-ttu-id="a1a93-166">包含该部分的笔记本。</span><span class="sxs-lookup"><span data-stu-id="a1a93-166">The notebook that contains the section.</span></span>  <span data-ttu-id="a1a93-167">只读。</span><span class="sxs-lookup"><span data-stu-id="a1a93-167">Read-only.</span></span>|
|<span data-ttu-id="a1a93-168">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="a1a93-168">parentSectionGroup</span></span>|[<span data-ttu-id="a1a93-169">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="a1a93-169">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="a1a93-170">包含节的节组。</span><span class="sxs-lookup"><span data-stu-id="a1a93-170">The section group that contains the section.</span></span>  <span data-ttu-id="a1a93-171">只读的。</span><span class="sxs-lookup"><span data-stu-id="a1a93-171">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="a1a93-172">方法</span><span class="sxs-lookup"><span data-stu-id="a1a93-172">Methods</span></span>

| <span data-ttu-id="a1a93-173">方法</span><span class="sxs-lookup"><span data-stu-id="a1a93-173">Method</span></span>           | <span data-ttu-id="a1a93-174">返回类型</span><span class="sxs-lookup"><span data-stu-id="a1a93-174">Return Type</span></span>    |<span data-ttu-id="a1a93-175">说明</span><span class="sxs-lookup"><span data-stu-id="a1a93-175">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a1a93-176">获取分区</span><span class="sxs-lookup"><span data-stu-id="a1a93-176">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="a1a93-177">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="a1a93-177">onenoteSection</span></span>](onenotesection.md) |<span data-ttu-id="a1a93-178">读取节的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a1a93-178">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="a1a93-179">创建页面</span><span class="sxs-lookup"><span data-stu-id="a1a93-179">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="a1a93-180">onenotePage</span><span class="sxs-lookup"><span data-stu-id="a1a93-180">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="a1a93-181">通过发布到指定分区中的 pages 集合来创建页面。</span><span class="sxs-lookup"><span data-stu-id="a1a93-181">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="a1a93-182">列出页面</span><span class="sxs-lookup"><span data-stu-id="a1a93-182">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="a1a93-183">[onenotePage](onenotepage.md)集合</span><span class="sxs-lookup"><span data-stu-id="a1a93-183">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="a1a93-184">获取指定节中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="a1a93-184">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="a1a93-185">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="a1a93-185">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="a1a93-186">无</span><span class="sxs-lookup"><span data-stu-id="a1a93-186">None</span></span>|<span data-ttu-id="a1a93-187">将分区复制到特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="a1a93-187">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="a1a93-188">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="a1a93-188">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="a1a93-189">无</span><span class="sxs-lookup"><span data-stu-id="a1a93-189">None</span></span>|<span data-ttu-id="a1a93-190">将分区复制到特定分区组。</span><span class="sxs-lookup"><span data-stu-id="a1a93-190">Copy the section to a specific section group.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a1a93-191">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1a93-191">JSON representation</span></span>

<span data-ttu-id="a1a93-192">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1a93-192">Here is a JSON representation of the resource.</span></span>

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
