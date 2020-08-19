---
title: onenoteSection 资源类型
description: OneNote 笔记本中的分区。 分区可包含页面。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 2ec9ea6b30443b0dfc25ce8ac5ccc4ff4ab0516d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809369"
---
# <a name="onenotesection-resource-type"></a><span data-ttu-id="23f9e-104">onenoteSection 资源类型</span><span class="sxs-lookup"><span data-stu-id="23f9e-104">onenoteSection resource type</span></span>

<span data-ttu-id="23f9e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23f9e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23f9e-106">OneNote 笔记本中的分区。</span><span class="sxs-lookup"><span data-stu-id="23f9e-106">A section in a OneNote notebook.</span></span> <span data-ttu-id="23f9e-107">分区可包含页面。</span><span class="sxs-lookup"><span data-stu-id="23f9e-107">Sections can contain pages.</span></span>

## <a name="properties"></a><span data-ttu-id="23f9e-108">属性</span><span class="sxs-lookup"><span data-stu-id="23f9e-108">Properties</span></span>
| <span data-ttu-id="23f9e-109">属性</span><span class="sxs-lookup"><span data-stu-id="23f9e-109">Property</span></span>     | <span data-ttu-id="23f9e-110">类型</span><span class="sxs-lookup"><span data-stu-id="23f9e-110">Type</span></span>   |<span data-ttu-id="23f9e-111">说明</span><span class="sxs-lookup"><span data-stu-id="23f9e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23f9e-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="23f9e-112">createdBy</span></span>|[<span data-ttu-id="23f9e-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="23f9e-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="23f9e-p103">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="23f9e-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="23f9e-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23f9e-116">createdDateTime</span></span>|<span data-ttu-id="23f9e-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23f9e-117">DateTimeOffset</span></span>|<span data-ttu-id="23f9e-118">节的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="23f9e-118">The date and time when the section was created.</span></span> <span data-ttu-id="23f9e-119">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="23f9e-119">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="23f9e-120">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="23f9e-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="23f9e-121">只读。</span><span class="sxs-lookup"><span data-stu-id="23f9e-121">Read-only.</span></span>|
|<span data-ttu-id="23f9e-122">id</span><span class="sxs-lookup"><span data-stu-id="23f9e-122">id</span></span>|<span data-ttu-id="23f9e-123">String</span><span class="sxs-lookup"><span data-stu-id="23f9e-123">String</span></span>|<span data-ttu-id="23f9e-124">节的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="23f9e-124">The unique identifier of the section.</span></span>  <span data-ttu-id="23f9e-125">只读。</span><span class="sxs-lookup"><span data-stu-id="23f9e-125">Read-only.</span></span>|
|<span data-ttu-id="23f9e-126">isDefault</span><span class="sxs-lookup"><span data-stu-id="23f9e-126">isDefault</span></span>|<span data-ttu-id="23f9e-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="23f9e-127">Boolean</span></span>|<span data-ttu-id="23f9e-128">指示是否为用户的默认节。</span><span class="sxs-lookup"><span data-stu-id="23f9e-128">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="23f9e-129">只读。</span><span class="sxs-lookup"><span data-stu-id="23f9e-129">Read-only.</span></span>|
|<span data-ttu-id="23f9e-130">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="23f9e-130">lastModifiedBy</span></span>|[<span data-ttu-id="23f9e-131">identitySet</span><span class="sxs-lookup"><span data-stu-id="23f9e-131">identitySet</span></span>](identityset.md)|<span data-ttu-id="23f9e-p107">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="23f9e-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="23f9e-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23f9e-134">lastModifiedDateTime</span></span>|<span data-ttu-id="23f9e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23f9e-135">DateTimeOffset</span></span>|<span data-ttu-id="23f9e-136">上次修改节的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="23f9e-136">The date and time when the section was last modified.</span></span> <span data-ttu-id="23f9e-137">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="23f9e-137">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="23f9e-138">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="23f9e-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="23f9e-139">只读。</span><span class="sxs-lookup"><span data-stu-id="23f9e-139">Read-only.</span></span>|
|<span data-ttu-id="23f9e-140">links</span><span class="sxs-lookup"><span data-stu-id="23f9e-140">links</span></span>|[<span data-ttu-id="23f9e-141">sectionLinks</span><span class="sxs-lookup"><span data-stu-id="23f9e-141">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="23f9e-142">用于打开分区的链接。</span><span class="sxs-lookup"><span data-stu-id="23f9e-142">Links for opening the section.</span></span> <span data-ttu-id="23f9e-143">`oneNoteClientURL`如果安装了 OneNote 本机客户端，则链接将在其中打开分区。</span><span class="sxs-lookup"><span data-stu-id="23f9e-143">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="23f9e-144">`oneNoteWebURL`链接将打开 web 上的 OneNote 中的分区。</span><span class="sxs-lookup"><span data-stu-id="23f9e-144">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="23f9e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="23f9e-145">displayName</span></span>|<span data-ttu-id="23f9e-146">String</span><span class="sxs-lookup"><span data-stu-id="23f9e-146">String</span></span>|<span data-ttu-id="23f9e-147">节的名称。</span><span class="sxs-lookup"><span data-stu-id="23f9e-147">The name of the section.</span></span> |
|<span data-ttu-id="23f9e-148">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="23f9e-148">pagesUrl</span></span>|<span data-ttu-id="23f9e-149">String</span><span class="sxs-lookup"><span data-stu-id="23f9e-149">String</span></span>|<span data-ttu-id="23f9e-150">`pages`终结点，您可在其中获取该部分中所有页面的详细信息。</span><span class="sxs-lookup"><span data-stu-id="23f9e-150">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="23f9e-151">只读。</span><span class="sxs-lookup"><span data-stu-id="23f9e-151">Read-only.</span></span>|
|<span data-ttu-id="23f9e-152">自学</span><span class="sxs-lookup"><span data-stu-id="23f9e-152">self</span></span>|<span data-ttu-id="23f9e-153">String</span><span class="sxs-lookup"><span data-stu-id="23f9e-153">String</span></span>|<span data-ttu-id="23f9e-154">终结点，您可在此处获取关于节的详细信息。</span><span class="sxs-lookup"><span data-stu-id="23f9e-154">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="23f9e-155">只读。</span><span class="sxs-lookup"><span data-stu-id="23f9e-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23f9e-156">关系</span><span class="sxs-lookup"><span data-stu-id="23f9e-156">Relationships</span></span>
| <span data-ttu-id="23f9e-157">关系</span><span class="sxs-lookup"><span data-stu-id="23f9e-157">Relationship</span></span> | <span data-ttu-id="23f9e-158">类型</span><span class="sxs-lookup"><span data-stu-id="23f9e-158">Type</span></span>   |<span data-ttu-id="23f9e-159">说明</span><span class="sxs-lookup"><span data-stu-id="23f9e-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23f9e-160">pages</span><span class="sxs-lookup"><span data-stu-id="23f9e-160">pages</span></span>|<span data-ttu-id="23f9e-161">[onenotePage](onenotepage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="23f9e-161">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="23f9e-162">分区中的一组页面。</span><span class="sxs-lookup"><span data-stu-id="23f9e-162">The collection of pages in the section.</span></span>  <span data-ttu-id="23f9e-163">只读。</span><span class="sxs-lookup"><span data-stu-id="23f9e-163">Read-only.</span></span> <span data-ttu-id="23f9e-164">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="23f9e-164">Nullable.</span></span>|
|<span data-ttu-id="23f9e-165">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="23f9e-165">parentNotebook</span></span>|[<span data-ttu-id="23f9e-166">笔记本</span><span class="sxs-lookup"><span data-stu-id="23f9e-166">notebook</span></span>](notebook.md)|<span data-ttu-id="23f9e-167">包含该部分的笔记本。</span><span class="sxs-lookup"><span data-stu-id="23f9e-167">The notebook that contains the section.</span></span>  <span data-ttu-id="23f9e-168">只读。</span><span class="sxs-lookup"><span data-stu-id="23f9e-168">Read-only.</span></span>|
|<span data-ttu-id="23f9e-169">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="23f9e-169">parentSectionGroup</span></span>|[<span data-ttu-id="23f9e-170">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="23f9e-170">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="23f9e-171">包含节的节组。</span><span class="sxs-lookup"><span data-stu-id="23f9e-171">The section group that contains the section.</span></span>  <span data-ttu-id="23f9e-172">只读的。</span><span class="sxs-lookup"><span data-stu-id="23f9e-172">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="23f9e-173">方法</span><span class="sxs-lookup"><span data-stu-id="23f9e-173">Methods</span></span>

| <span data-ttu-id="23f9e-174">方法</span><span class="sxs-lookup"><span data-stu-id="23f9e-174">Method</span></span>           | <span data-ttu-id="23f9e-175">返回类型</span><span class="sxs-lookup"><span data-stu-id="23f9e-175">Return Type</span></span>    |<span data-ttu-id="23f9e-176">说明</span><span class="sxs-lookup"><span data-stu-id="23f9e-176">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="23f9e-177">获取分区</span><span class="sxs-lookup"><span data-stu-id="23f9e-177">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="23f9e-178">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="23f9e-178">onenoteSection</span></span>](onenotesection.md) |<span data-ttu-id="23f9e-179">读取节的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="23f9e-179">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="23f9e-180">创建页面</span><span class="sxs-lookup"><span data-stu-id="23f9e-180">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="23f9e-181">onenotePage</span><span class="sxs-lookup"><span data-stu-id="23f9e-181">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="23f9e-182">通过发布到指定分区中的 pages 集合来创建页面。</span><span class="sxs-lookup"><span data-stu-id="23f9e-182">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="23f9e-183">列出页面</span><span class="sxs-lookup"><span data-stu-id="23f9e-183">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="23f9e-184">[onenotePage](onenotepage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="23f9e-184">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="23f9e-185">获取指定节中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="23f9e-185">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="23f9e-186">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="23f9e-186">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="23f9e-187">无</span><span class="sxs-lookup"><span data-stu-id="23f9e-187">None</span></span>|<span data-ttu-id="23f9e-188">将分区复制到特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="23f9e-188">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="23f9e-189">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="23f9e-189">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="23f9e-190">无</span><span class="sxs-lookup"><span data-stu-id="23f9e-190">None</span></span>|<span data-ttu-id="23f9e-191">将分区复制到特定分区组。</span><span class="sxs-lookup"><span data-stu-id="23f9e-191">Copy the section to a specific section group.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="23f9e-192">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23f9e-192">JSON representation</span></span>

<span data-ttu-id="23f9e-193">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23f9e-193">Here is a JSON representation of the resource.</span></span>

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
