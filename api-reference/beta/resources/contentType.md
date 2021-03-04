---
author: daspek
description: ContentType 资源代表 SharePoint 中的内容类型。
title: contentType
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 2af8291f33f62517e33349fb66408131f576e89a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444292"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="10a04-103">contentType 资源类型</span><span class="sxs-lookup"><span data-stu-id="10a04-103">contentType resource type</span></span>

<span data-ttu-id="10a04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10a04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10a04-105">表示 SharePoint _中_ 的内容类型。</span><span class="sxs-lookup"><span data-stu-id="10a04-105">Represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="10a04-106">内容类型允许您定义一组列，这些列必须存在于列表中的每个 [**listItem**][listItem] [**上**][list]。</span><span class="sxs-lookup"><span data-stu-id="10a04-106">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

## <a name="properties"></a><span data-ttu-id="10a04-107">属性</span><span class="sxs-lookup"><span data-stu-id="10a04-107">Properties</span></span>

| <span data-ttu-id="10a04-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="10a04-108">Property name</span></span>     | <span data-ttu-id="10a04-109">类型</span><span class="sxs-lookup"><span data-stu-id="10a04-109">Type</span></span>                 | <span data-ttu-id="10a04-110">说明</span><span class="sxs-lookup"><span data-stu-id="10a04-110">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="10a04-111">**说明**</span><span class="sxs-lookup"><span data-stu-id="10a04-111">**description**</span></span>   | <span data-ttu-id="10a04-112">string</span><span class="sxs-lookup"><span data-stu-id="10a04-112">string</span></span>               | <span data-ttu-id="10a04-113">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="10a04-113">The descriptive text for the item.</span></span>
| <span data-ttu-id="10a04-114">**group**</span><span class="sxs-lookup"><span data-stu-id="10a04-114">**group**</span></span>         | <span data-ttu-id="10a04-115">string</span><span class="sxs-lookup"><span data-stu-id="10a04-115">string</span></span>               | <span data-ttu-id="10a04-116">此内容类型所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="10a04-116">The name of the group this content type belongs to.</span></span> <span data-ttu-id="10a04-117">可以帮助组织相关的内容类型。</span><span class="sxs-lookup"><span data-stu-id="10a04-117">Helps organize related content types.</span></span>
| <span data-ttu-id="10a04-118">**hidden**</span><span class="sxs-lookup"><span data-stu-id="10a04-118">**hidden**</span></span>        | <span data-ttu-id="10a04-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="10a04-119">Boolean</span></span>              | <span data-ttu-id="10a04-120">指示内容类型是否隐藏于此列表的“新建”菜单中。</span><span class="sxs-lookup"><span data-stu-id="10a04-120">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="10a04-121">**id**</span><span class="sxs-lookup"><span data-stu-id="10a04-121">**id**</span></span>            | <span data-ttu-id="10a04-122">string</span><span class="sxs-lookup"><span data-stu-id="10a04-122">string</span></span>               | <span data-ttu-id="10a04-123">内容类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="10a04-123">The unique identifier of the content type.</span></span>
| <span data-ttu-id="10a04-124">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="10a04-124">**inheritedFrom**</span></span> | <span data-ttu-id="10a04-125">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="10a04-125">[itemReference][]</span></span>    | <span data-ttu-id="10a04-126">如果此内容类型继承自另一个作用域（如某个站点），则会提供对在其中定义内容类型的项的引用。</span><span class="sxs-lookup"><span data-stu-id="10a04-126">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="10a04-127">**名称**</span><span class="sxs-lookup"><span data-stu-id="10a04-127">**name**</span></span>          | <span data-ttu-id="10a04-128">string</span><span class="sxs-lookup"><span data-stu-id="10a04-128">string</span></span>               | <span data-ttu-id="10a04-129">内容类型的名称。</span><span class="sxs-lookup"><span data-stu-id="10a04-129">The name of the content type.</span></span>
| <span data-ttu-id="10a04-130">**order**</span><span class="sxs-lookup"><span data-stu-id="10a04-130">**order**</span></span>         | <span data-ttu-id="10a04-131">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="10a04-131">[contentTypeOrder][]</span></span> | <span data-ttu-id="10a04-132">指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="10a04-132">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="10a04-133">**parentId**</span><span class="sxs-lookup"><span data-stu-id="10a04-133">**parentId**</span></span>      | <span data-ttu-id="10a04-134">string</span><span class="sxs-lookup"><span data-stu-id="10a04-134">string</span></span>               | <span data-ttu-id="10a04-135">内容类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="10a04-135">The unique identifier of the content type.</span></span>
| <span data-ttu-id="10a04-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="10a04-136">**readOnly**</span></span>      | <span data-ttu-id="10a04-137">布尔</span><span class="sxs-lookup"><span data-stu-id="10a04-137">Boolean</span></span>              | <span data-ttu-id="10a04-138">如果为 `true`，则不能修改内容类型，除非此值首次设置为 `false`。</span><span class="sxs-lookup"><span data-stu-id="10a04-138">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="10a04-139">**sealed**</span><span class="sxs-lookup"><span data-stu-id="10a04-139">**sealed**</span></span>        | <span data-ttu-id="10a04-140">布尔</span><span class="sxs-lookup"><span data-stu-id="10a04-140">Boolean</span></span>              | <span data-ttu-id="10a04-141">如果为 `true`，则不能由用户或通过下推操作修改内容类型。</span><span class="sxs-lookup"><span data-stu-id="10a04-141">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="10a04-142">只有网站集管理员可以密封或解封内容类型。</span><span class="sxs-lookup"><span data-stu-id="10a04-142">Only site collection administrators can seal or unseal content types.</span></span>
| <span data-ttu-id="10a04-143">**isBuiltIn**</span><span class="sxs-lookup"><span data-stu-id="10a04-143">**isBuiltIn**</span></span>            | <span data-ttu-id="10a04-144">布尔</span><span class="sxs-lookup"><span data-stu-id="10a04-144">Boolean</span></span>| <span data-ttu-id="10a04-145">指定内容类型是内置内容类型。</span><span class="sxs-lookup"><span data-stu-id="10a04-145">Specifies if a content type is a built-in content type.</span></span> 
| <span data-ttu-id="10a04-146">**documentSet**</span><span class="sxs-lookup"><span data-stu-id="10a04-146">**documentSet**</span></span>       | <span data-ttu-id="10a04-147">[documentSet][]</span><span class="sxs-lookup"><span data-stu-id="10a04-147">[documentSet][]</span></span>      | <span data-ttu-id="10a04-148">[文档集](https://docs.microsoft.com/sharepoint/governance/document-set-planning#about-document-sets) 元数据。</span><span class="sxs-lookup"><span data-stu-id="10a04-148">[Document Set](https://docs.microsoft.com/sharepoint/governance/document-set-planning#about-document-sets) metadata.</span></span>
| <span data-ttu-id="10a04-149">**documentTemplate**</span><span class="sxs-lookup"><span data-stu-id="10a04-149">**documentTemplate**</span></span>  | <span data-ttu-id="10a04-150">[documentSetContent][]</span><span class="sxs-lookup"><span data-stu-id="10a04-150">[documentSetContent][]</span></span> | <span data-ttu-id="10a04-151">文档模板元数据。</span><span class="sxs-lookup"><span data-stu-id="10a04-151">Document template metadata.</span></span> <span data-ttu-id="10a04-152">若要确保文档在网站及其子网站中具有一致的内容，可以将 Word、Excel 或 PowerPoint 模板与网站内容类型关联。</span><span class="sxs-lookup"><span data-stu-id="10a04-152">To make sure that documents have consistent content across a site and its subsites, you can associate a Word, Excel, or PowerPoint template with a site content type.</span></span>
| <span data-ttu-id="10a04-153">**associatedHubsUrls**</span><span class="sxs-lookup"><span data-stu-id="10a04-153">**associatedHubsUrls**</span></span>       | <span data-ttu-id="10a04-154">集合 (字符串) </span><span class="sxs-lookup"><span data-stu-id="10a04-154">Collection(string)</span></span> | <span data-ttu-id="10a04-155">与此内容类型关联的中心网站的规范 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="10a04-155">List of canonical URLs for hub sites with which this content type is associated to.</span></span> <span data-ttu-id="10a04-156">这将包含此内容类型已排入队列以强制执行或已强制执行的所有中心网站。</span><span class="sxs-lookup"><span data-stu-id="10a04-156">This will contain all hubsites where this content type is queued to be enforced or is already enforced.</span></span> <span data-ttu-id="10a04-157">强制执行内容类型意味着内容类型将应用于强制网站中的列表。</span><span class="sxs-lookup"><span data-stu-id="10a04-157">Enforcing a content type means that the content type will be applied to the lists in the enforced sites.</span></span>
| <span data-ttu-id="10a04-158">**propagateChanges**</span><span class="sxs-lookup"><span data-stu-id="10a04-158">**propagateChanges**</span></span>   | <span data-ttu-id="10a04-159">布尔</span><span class="sxs-lookup"><span data-stu-id="10a04-159">Boolean</span></span>              | <span data-ttu-id="10a04-160">如果 `true` ，对内容类型进行的任何更改都将推送到实现内容类型的继承内容类型和列表。</span><span class="sxs-lookup"><span data-stu-id="10a04-160">If `true`, any changes made to the content type will be pushed to inherited content types and lists that implement the content type.</span></span>



## <a name="relationships"></a><span data-ttu-id="10a04-161">关系</span><span class="sxs-lookup"><span data-stu-id="10a04-161">Relationships</span></span>

| <span data-ttu-id="10a04-162">属性名称</span><span class="sxs-lookup"><span data-stu-id="10a04-162">Property name</span></span>   | <span data-ttu-id="10a04-163">类型</span><span class="sxs-lookup"><span data-stu-id="10a04-163">Type</span></span>                      | <span data-ttu-id="10a04-164">说明</span><span class="sxs-lookup"><span data-stu-id="10a04-164">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="10a04-165">**base**</span><span class="sxs-lookup"><span data-stu-id="10a04-165">**base**</span></span>   | <span data-ttu-id="10a04-166">[contentType][]</span><span class="sxs-lookup"><span data-stu-id="10a04-166">[contentType][]</span></span>  | <span data-ttu-id="10a04-167">派生此内容类型的父 contentType。</span><span class="sxs-lookup"><span data-stu-id="10a04-167">Parent contentType from which this content type is derived.</span></span> 
| <span data-ttu-id="10a04-168">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="10a04-168">**columnLinks**</span></span> | <span data-ttu-id="10a04-169">[columnLink][] 集合</span><span class="sxs-lookup"><span data-stu-id="10a04-169">[columnLink][] collection</span></span> | <span data-ttu-id="10a04-170">此内容类型所需的列集合</span><span class="sxs-lookup"><span data-stu-id="10a04-170">The collection of columns that are required by this content type</span></span>
| <span data-ttu-id="10a04-171">**baseTypes**</span><span class="sxs-lookup"><span data-stu-id="10a04-171">**baseTypes**</span></span>   | <span data-ttu-id="10a04-172">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="10a04-172">Collection([contentType][])</span></span>     | <span data-ttu-id="10a04-173">作为此内容类型的上级的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="10a04-173">The collection of content types that are ancestors of this content type.</span></span>
| <span data-ttu-id="10a04-174">**columnPositions**</span><span class="sxs-lookup"><span data-stu-id="10a04-174">**columnPositions**</span></span>       | <span data-ttu-id="10a04-175">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="10a04-175">Collection([columnDefinition][])</span></span> | <span data-ttu-id="10a04-176">内容类型中的列顺序信息。</span><span class="sxs-lookup"><span data-stu-id="10a04-176">Column order information in a content type.</span></span>
| <span data-ttu-id="10a04-177">**columns**</span><span class="sxs-lookup"><span data-stu-id="10a04-177">**columns**</span></span>     | <span data-ttu-id="10a04-178">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="10a04-178">Collection([columnDefinition][])</span></span>  | <span data-ttu-id="10a04-179">此 contentType 的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="10a04-179">The collection of column definitions for this contentType.</span></span>

<span data-ttu-id="10a04-180">请参阅[内容类型和内容类型发布简介][contentTypeIntro]了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="10a04-180">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md
[columnDefinition]: columnDefinition.md
[contentType]: contentType.md
[documentSet]: documentSet.md
[documentSetContent]: documentSetContent.md

## <a name="json-representation"></a><span data-ttu-id="10a04-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10a04-188">JSON representation</span></span>

<span data-ttu-id="10a04-189">下面是 **contentType** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10a04-189">The following is a JSON representation of a **contentType** resource.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType","keyProperty":"id" } -->

```json
{
  "description": "string",
  "group": "string",
  "hidden": false,
  "id": "string",
  "inheritedFrom": { "@type": "microsoft.graph.itemReference" },
  "name": "string",
  "order": { "@type": "microsoft.graph.contentTypeOrder" },
  "parentId": "string",
  "readOnly": false,
  "sealed": false,
  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }],
  "base": { "@type": "microsoft.graph.contentType" },
  "columnPositions" : [{ "@type": "microsoft.graph.columnDefinition" }],
  "isBuiltIn" : false,
  "documentSet" : { "@type": "microsoft.graph.documentSet" },
  "documentTemplate" : { "@type": "microsoft.graph.documentSetContent" },
  "associatedHubsUrls" : ["string"],
  "propagateChanges" : false,
  "baseTypes" : [{ "@type": "microsoft.graph.contentType" }],
  "columns" : [{ "@type": "microsoft.graph.columnDefinition" }]
}
```

[list]: list.md
[listItem]: listitem.md
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType",
  "suppressions": []
}
-->


