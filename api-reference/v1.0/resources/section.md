---
title: 部分资源类型
description: OneNote 笔记本中的分区。 分区可包含页面。
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6cc87845b14b45dbe84377f1be917fe4b9f873ff
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812244"
---
# <a name="section-resource-type"></a><span data-ttu-id="b0c60-104">部分资源类型</span><span class="sxs-lookup"><span data-stu-id="b0c60-104">section resource type</span></span>

<span data-ttu-id="b0c60-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0c60-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b0c60-106">OneNote 笔记本中的分区。</span><span class="sxs-lookup"><span data-stu-id="b0c60-106">A section in a OneNote notebook.</span></span> <span data-ttu-id="b0c60-107">分区可包含页面。</span><span class="sxs-lookup"><span data-stu-id="b0c60-107">Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0c60-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0c60-108">JSON representation</span></span>

<span data-ttu-id="b0c60-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0c60-109">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="b0c60-110">属性</span><span class="sxs-lookup"><span data-stu-id="b0c60-110">Properties</span></span>
| <span data-ttu-id="b0c60-111">属性</span><span class="sxs-lookup"><span data-stu-id="b0c60-111">Property</span></span>     | <span data-ttu-id="b0c60-112">类型</span><span class="sxs-lookup"><span data-stu-id="b0c60-112">Type</span></span>   |<span data-ttu-id="b0c60-113">说明</span><span class="sxs-lookup"><span data-stu-id="b0c60-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0c60-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="b0c60-114">createdBy</span></span>|[<span data-ttu-id="b0c60-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="b0c60-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="b0c60-p103">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="b0c60-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="b0c60-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0c60-118">createdDateTime</span></span>|<span data-ttu-id="b0c60-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0c60-119">DateTimeOffset</span></span>|<span data-ttu-id="b0c60-120">节的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b0c60-120">The date and time when the section was created.</span></span> <span data-ttu-id="b0c60-121">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="b0c60-121">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b0c60-122">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="b0c60-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b0c60-123">只读。</span><span class="sxs-lookup"><span data-stu-id="b0c60-123">Read-only.</span></span>|
|<span data-ttu-id="b0c60-124">id</span><span class="sxs-lookup"><span data-stu-id="b0c60-124">id</span></span>|<span data-ttu-id="b0c60-125">String</span><span class="sxs-lookup"><span data-stu-id="b0c60-125">String</span></span>|<span data-ttu-id="b0c60-126">节的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b0c60-126">The unique identifier of the section.</span></span>  <span data-ttu-id="b0c60-127">只读。</span><span class="sxs-lookup"><span data-stu-id="b0c60-127">Read-only.</span></span>|
|<span data-ttu-id="b0c60-128">isDefault</span><span class="sxs-lookup"><span data-stu-id="b0c60-128">isDefault</span></span>|<span data-ttu-id="b0c60-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0c60-129">Boolean</span></span>|<span data-ttu-id="b0c60-130">指示是否为用户的默认节。</span><span class="sxs-lookup"><span data-stu-id="b0c60-130">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="b0c60-131">只读。</span><span class="sxs-lookup"><span data-stu-id="b0c60-131">Read-only.</span></span>|
|<span data-ttu-id="b0c60-132">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b0c60-132">lastModifiedBy</span></span>|[<span data-ttu-id="b0c60-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="b0c60-133">identitySet</span></span>](identityset.md)|<span data-ttu-id="b0c60-p107">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="b0c60-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="b0c60-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0c60-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b0c60-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0c60-137">DateTimeOffset</span></span>|<span data-ttu-id="b0c60-138">上次修改节的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b0c60-138">The date and time when the section was last modified.</span></span> <span data-ttu-id="b0c60-139">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="b0c60-139">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b0c60-140">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="b0c60-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b0c60-141">只读。</span><span class="sxs-lookup"><span data-stu-id="b0c60-141">Read-only.</span></span>|
|<span data-ttu-id="b0c60-142">links</span><span class="sxs-lookup"><span data-stu-id="b0c60-142">links</span></span>|[<span data-ttu-id="b0c60-143">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="b0c60-143">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="b0c60-144">用于打开分区的链接。</span><span class="sxs-lookup"><span data-stu-id="b0c60-144">Links for opening the section.</span></span> <span data-ttu-id="b0c60-145">`oneNoteClientURL`如果安装了 OneNote 本机客户端，则链接将在其中打开分区。</span><span class="sxs-lookup"><span data-stu-id="b0c60-145">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="b0c60-146">`oneNoteWebURL`链接将打开 web 上的 OneNote 中的分区。</span><span class="sxs-lookup"><span data-stu-id="b0c60-146">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="b0c60-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b0c60-147">displayName</span></span>|<span data-ttu-id="b0c60-148">String</span><span class="sxs-lookup"><span data-stu-id="b0c60-148">String</span></span>|<span data-ttu-id="b0c60-149">节的名称。</span><span class="sxs-lookup"><span data-stu-id="b0c60-149">The name of the section.</span></span> |
|<span data-ttu-id="b0c60-150">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="b0c60-150">pagesUrl</span></span>|<span data-ttu-id="b0c60-151">String</span><span class="sxs-lookup"><span data-stu-id="b0c60-151">String</span></span>|<span data-ttu-id="b0c60-152">`pages`终结点，您可在其中获取该部分中所有页面的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b0c60-152">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="b0c60-153">只读。</span><span class="sxs-lookup"><span data-stu-id="b0c60-153">Read-only.</span></span>|
|<span data-ttu-id="b0c60-154">自学</span><span class="sxs-lookup"><span data-stu-id="b0c60-154">self</span></span>|<span data-ttu-id="b0c60-155">String</span><span class="sxs-lookup"><span data-stu-id="b0c60-155">String</span></span>|<span data-ttu-id="b0c60-156">终结点，您可在此处获取关于节的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b0c60-156">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="b0c60-157">只读。</span><span class="sxs-lookup"><span data-stu-id="b0c60-157">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0c60-158">关系</span><span class="sxs-lookup"><span data-stu-id="b0c60-158">Relationships</span></span>
| <span data-ttu-id="b0c60-159">关系</span><span class="sxs-lookup"><span data-stu-id="b0c60-159">Relationship</span></span> | <span data-ttu-id="b0c60-160">类型</span><span class="sxs-lookup"><span data-stu-id="b0c60-160">Type</span></span>   |<span data-ttu-id="b0c60-161">说明</span><span class="sxs-lookup"><span data-stu-id="b0c60-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0c60-162">pages</span><span class="sxs-lookup"><span data-stu-id="b0c60-162">pages</span></span>|<span data-ttu-id="b0c60-163">[OnenotePage](page.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b0c60-163">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="b0c60-164">分区中的一组页面。</span><span class="sxs-lookup"><span data-stu-id="b0c60-164">The collection of pages in the section.</span></span>  <span data-ttu-id="b0c60-165">只读。</span><span class="sxs-lookup"><span data-stu-id="b0c60-165">Read-only.</span></span> <span data-ttu-id="b0c60-166">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b0c60-166">Nullable.</span></span>|
|<span data-ttu-id="b0c60-167">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="b0c60-167">parentNotebook</span></span>|[<span data-ttu-id="b0c60-168">笔记本</span><span class="sxs-lookup"><span data-stu-id="b0c60-168">Notebook</span></span>](notebook.md)|<span data-ttu-id="b0c60-169">包含该部分的笔记本。</span><span class="sxs-lookup"><span data-stu-id="b0c60-169">The notebook that contains the section.</span></span>  <span data-ttu-id="b0c60-170">只读。</span><span class="sxs-lookup"><span data-stu-id="b0c60-170">Read-only.</span></span>|
|<span data-ttu-id="b0c60-171">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="b0c60-171">parentSectionGroup</span></span>|[<span data-ttu-id="b0c60-172">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="b0c60-172">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="b0c60-173">包含节的节组。</span><span class="sxs-lookup"><span data-stu-id="b0c60-173">The section group that contains the section.</span></span>  <span data-ttu-id="b0c60-174">只读的。</span><span class="sxs-lookup"><span data-stu-id="b0c60-174">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="b0c60-175">方法</span><span class="sxs-lookup"><span data-stu-id="b0c60-175">Methods</span></span>

| <span data-ttu-id="b0c60-176">方法</span><span class="sxs-lookup"><span data-stu-id="b0c60-176">Method</span></span>           | <span data-ttu-id="b0c60-177">返回类型</span><span class="sxs-lookup"><span data-stu-id="b0c60-177">Return Type</span></span>    |<span data-ttu-id="b0c60-178">说明</span><span class="sxs-lookup"><span data-stu-id="b0c60-178">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0c60-179">获取分区</span><span class="sxs-lookup"><span data-stu-id="b0c60-179">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="b0c60-180">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="b0c60-180">OnenoteSection</span></span>](section.md) |<span data-ttu-id="b0c60-181">读取节的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b0c60-181">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="b0c60-182">创建页面</span><span class="sxs-lookup"><span data-stu-id="b0c60-182">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="b0c60-183">页面</span><span class="sxs-lookup"><span data-stu-id="b0c60-183">Page</span></span>](page.md)| <span data-ttu-id="b0c60-184">通过发布到指定分区中的 pages 集合来创建页面。</span><span class="sxs-lookup"><span data-stu-id="b0c60-184">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="b0c60-185">列出页面</span><span class="sxs-lookup"><span data-stu-id="b0c60-185">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="b0c60-186">[页面](page.md)集合</span><span class="sxs-lookup"><span data-stu-id="b0c60-186">[Page](page.md) collection</span></span>| <span data-ttu-id="b0c60-187">获取指定节中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="b0c60-187">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="b0c60-188">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="b0c60-188">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="b0c60-189">无</span><span class="sxs-lookup"><span data-stu-id="b0c60-189">None</span></span>|<span data-ttu-id="b0c60-190">将分区复制到特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="b0c60-190">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="b0c60-191">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="b0c60-191">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="b0c60-192">无</span><span class="sxs-lookup"><span data-stu-id="b0c60-192">None</span></span>|<span data-ttu-id="b0c60-193">将分区复制到特定分区组。</span><span class="sxs-lookup"><span data-stu-id="b0c60-193">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
