---
author: daspek
description: ContentType 资源代表 SharePoint 中的内容类型。
title: contentType
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: bcd888d01f47b98fa5a55a4b6da2fdfe2028e05b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962656"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="38829-103">contentType 资源类型</span><span class="sxs-lookup"><span data-stu-id="38829-103">contentType resource type</span></span>

<span data-ttu-id="38829-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38829-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38829-105">表示 SharePoint 中的内容类型。</span><span class="sxs-lookup"><span data-stu-id="38829-105">Represents a content type in SharePoint.</span></span>
<span data-ttu-id="38829-106">内容类型允许您定义一组列，这些列必须存在于列表中的每个 [**listItem**][listItem] [**上**][list]。</span><span class="sxs-lookup"><span data-stu-id="38829-106">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

## <a name="methods"></a><span data-ttu-id="38829-107">Methods</span><span class="sxs-lookup"><span data-stu-id="38829-107">Methods</span></span>
|<span data-ttu-id="38829-108">方法</span><span class="sxs-lookup"><span data-stu-id="38829-108">Method</span></span>|<span data-ttu-id="38829-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="38829-109">Return type</span></span>|<span data-ttu-id="38829-110">说明</span><span class="sxs-lookup"><span data-stu-id="38829-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="38829-111">列出网站中的 contentTypes</span><span class="sxs-lookup"><span data-stu-id="38829-111">List contentTypes in a site</span></span>](../api/site-list-contenttypes.md)|<span data-ttu-id="38829-112">[contentType](../resources/contenttype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="38829-112">[contentType](../resources/contenttype.md) collection</span></span>|<span data-ttu-id="38829-113">获取网站 中的 [contentType](../resources/contenttype.md) 对象及其属性 [的列表](../resources/site.md)。</span><span class="sxs-lookup"><span data-stu-id="38829-113">Get a list of the [contentType](../resources/contenttype.md) objects and their properties in a [site](../resources/site.md).</span></span>|
|[<span data-ttu-id="38829-114">列出列表中的 contentTypes</span><span class="sxs-lookup"><span data-stu-id="38829-114">List contentTypes in a list</span></span>](../api/list-list-contenttypes.md)|<span data-ttu-id="38829-115">[contentType](../resources/contenttype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="38829-115">[contentType](../resources/contenttype.md) collection</span></span>|<span data-ttu-id="38829-116">在列表中获取 [contentType](../resources/contenttype.md) 对象及其属性 [的列表](../resources/list.md)。</span><span class="sxs-lookup"><span data-stu-id="38829-116">Get a list of the [contentType](../resources/contenttype.md) objects and their properties in a [list](../resources/list.md).</span></span>|
|[<span data-ttu-id="38829-117">为网站创建 contentType</span><span class="sxs-lookup"><span data-stu-id="38829-117">Create contentType for a site</span></span>](../api/site-post-contenttypes.md)|[<span data-ttu-id="38829-118">contentType</span><span class="sxs-lookup"><span data-stu-id="38829-118">contentType</span></span>](../resources/contenttype.md)|<span data-ttu-id="38829-119">在网站 [中创建新的 contentType](../resources/contenttype.md) [对象](../resources/site.md)。</span><span class="sxs-lookup"><span data-stu-id="38829-119">Create a new [contentType](../resources/contenttype.md) object in a [site](../resources/site.md).</span></span>|
|[<span data-ttu-id="38829-120">获取 contentType</span><span class="sxs-lookup"><span data-stu-id="38829-120">Get contentType</span></span>](../api/contenttype-get.md)|[<span data-ttu-id="38829-121">contentType</span><span class="sxs-lookup"><span data-stu-id="38829-121">contentType</span></span>](../resources/contenttype.md)|<span data-ttu-id="38829-122">读取 [contentType](../resources/contenttype.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="38829-122">Read the properties and relationships of a [contentType](../resources/contenttype.md) object.</span></span>|
|[<span data-ttu-id="38829-123">更新 contentType</span><span class="sxs-lookup"><span data-stu-id="38829-123">Update contentType</span></span>](../api/contenttype-update.md)|[<span data-ttu-id="38829-124">contentType</span><span class="sxs-lookup"><span data-stu-id="38829-124">contentType</span></span>](../resources/contenttype.md)|<span data-ttu-id="38829-125">更新 [contentType 对象](../resources/contenttype.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="38829-125">Update the properties of a [contentType](../resources/contenttype.md) object.</span></span>|
|[<span data-ttu-id="38829-126">删除 contentType</span><span class="sxs-lookup"><span data-stu-id="38829-126">Delete contentType</span></span>](../api/contenttype-delete.md)|<span data-ttu-id="38829-127">无</span><span class="sxs-lookup"><span data-stu-id="38829-127">None</span></span>|<span data-ttu-id="38829-128">删除 [contentType](../resources/contenttype.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="38829-128">Deletes a [contentType](../resources/contenttype.md) object.</span></span>|
|[<span data-ttu-id="38829-129">isPublished</span><span class="sxs-lookup"><span data-stu-id="38829-129">isPublished</span></span>](../api/contenttype-ispublished.md)|<span data-ttu-id="38829-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="38829-130">Boolean</span></span>| <span data-ttu-id="38829-131">检查 [contentType 是否](../resources/contenttype.md) 发布。</span><span class="sxs-lookup"><span data-stu-id="38829-131">Checks if the [contentType](../resources/contenttype.md) is published.</span></span>|
|[<span data-ttu-id="38829-132">发布</span><span class="sxs-lookup"><span data-stu-id="38829-132">publish</span></span>](../api/contenttype-publish.md)|[<span data-ttu-id="38829-133">contentType</span><span class="sxs-lookup"><span data-stu-id="38829-133">contentType</span></span>](../resources/contenttype.md)| <span data-ttu-id="38829-134">发布 [contentType](../resources/contenttype.md)。</span><span class="sxs-lookup"><span data-stu-id="38829-134">Publish a [contentType](../resources/contenttype.md).</span></span>|
|[<span data-ttu-id="38829-135">取消发布</span><span class="sxs-lookup"><span data-stu-id="38829-135">unpublish</span></span>](../api/contenttype-unpublish.md)|[<span data-ttu-id="38829-136">contentType</span><span class="sxs-lookup"><span data-stu-id="38829-136">contentType</span></span>](../resources/contenttype.md)|<span data-ttu-id="38829-137">取消发布 [contentType](../resources/contenttype.md)。</span><span class="sxs-lookup"><span data-stu-id="38829-137">Unpublish a [contentType](../resources/contenttype.md).</span></span>|
|[<span data-ttu-id="38829-138">addCopy</span><span class="sxs-lookup"><span data-stu-id="38829-138">addCopy</span></span>](../api/contenttype-addcopy.md)|[<span data-ttu-id="38829-139">contentType</span><span class="sxs-lookup"><span data-stu-id="38829-139">contentType</span></span>](../resources/contenttype.md)|<span data-ttu-id="38829-140">将网站中的[contentType](../resources/contenttype.md) [副本添加到](../resources/site.md)[列表) 。](../resources/list.md)</span><span class="sxs-lookup"><span data-stu-id="38829-140">Add copy of a [contentType](../resources/contenttype.md) from a [site](../resources/site.md) to a [list](../resources/list.md)).</span></span>|
|[<span data-ttu-id="38829-141">associateWithHubSites</span><span class="sxs-lookup"><span data-stu-id="38829-141">associateWithHubSites</span></span>](../api/contenttype-associatewithhubsites.md)|[<span data-ttu-id="38829-142">contentType</span><span class="sxs-lookup"><span data-stu-id="38829-142">contentType</span></span>](../resources/contenttype.md)|<span data-ttu-id="38829-143">将 [contentType](../resources/contenttype.md) 与中心网站列表关联。</span><span class="sxs-lookup"><span data-stu-id="38829-143">Associates a [contentType](../resources/contenttype.md) with a list of hubsites.</span></span>|
|[<span data-ttu-id="38829-144">copyToDefaultContentLocation</span><span class="sxs-lookup"><span data-stu-id="38829-144">copyToDefaultContentLocation</span></span>](../api/contenttype-copytodefaultcontentlocation.md)|[<span data-ttu-id="38829-145">contentType</span><span class="sxs-lookup"><span data-stu-id="38829-145">contentType</span></span>](../resources/contenttype.md)| <span data-ttu-id="38829-146">将文件复制到 contentType 中的默认 [内容位置](../resources/contenttype.md)。</span><span class="sxs-lookup"><span data-stu-id="38829-146">Copy a file to default content location in a [contentType](../resources/contenttype.md).</span></span>|
|[<span data-ttu-id="38829-147">List columns</span><span class="sxs-lookup"><span data-stu-id="38829-147">List columns</span></span>](../api/contenttype-list-columns.md)|<span data-ttu-id="38829-148">[columnDefinition](../resources/columnDefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="38829-148">[columnDefinition](../resources/columnDefinition.md) collection</span></span>|<span data-ttu-id="38829-149">获取 **contentType** 中的列的集合，这些列表示为 [columnDefinition](../resources/columnDefinition.md)资源。</span><span class="sxs-lookup"><span data-stu-id="38829-149">Get a collection of columns, represented as [columnDefinition](../resources/columnDefinition.md) resources, in a **contentType**.</span></span>|
|[<span data-ttu-id="38829-150">创建列</span><span class="sxs-lookup"><span data-stu-id="38829-150">Create column</span></span>](../api/contenttype-post-columns.md)|[<span data-ttu-id="38829-151">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="38829-151">columnDefinition</span></span>](../resources/columnDefinition.md)|<span data-ttu-id="38829-152">向网站或 **列表中的内容** 类型添加列。</span><span class="sxs-lookup"><span data-stu-id="38829-152">Add a column to a **content type** in a site or list.</span></span>|


## <a name="properties"></a><span data-ttu-id="38829-153">属性</span><span class="sxs-lookup"><span data-stu-id="38829-153">Properties</span></span>

| <span data-ttu-id="38829-154">属性名称</span><span class="sxs-lookup"><span data-stu-id="38829-154">Property name</span></span>     | <span data-ttu-id="38829-155">类型</span><span class="sxs-lookup"><span data-stu-id="38829-155">Type</span></span>                 | <span data-ttu-id="38829-156">说明</span><span class="sxs-lookup"><span data-stu-id="38829-156">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="38829-157">**说明**</span><span class="sxs-lookup"><span data-stu-id="38829-157">**description**</span></span>   | <span data-ttu-id="38829-158">string</span><span class="sxs-lookup"><span data-stu-id="38829-158">string</span></span>               | <span data-ttu-id="38829-159">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="38829-159">The descriptive text for the item.</span></span>
| <span data-ttu-id="38829-160">**group**</span><span class="sxs-lookup"><span data-stu-id="38829-160">**group**</span></span>         | <span data-ttu-id="38829-161">string</span><span class="sxs-lookup"><span data-stu-id="38829-161">string</span></span>               | <span data-ttu-id="38829-162">此内容类型所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="38829-162">The name of the group this content type belongs to.</span></span> <span data-ttu-id="38829-163">可以帮助组织相关的内容类型。</span><span class="sxs-lookup"><span data-stu-id="38829-163">Helps organize related content types.</span></span>
| <span data-ttu-id="38829-164">**hidden**</span><span class="sxs-lookup"><span data-stu-id="38829-164">**hidden**</span></span>        | <span data-ttu-id="38829-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="38829-165">Boolean</span></span>              | <span data-ttu-id="38829-166">指示内容类型是否隐藏于此列表的“新建”菜单中。</span><span class="sxs-lookup"><span data-stu-id="38829-166">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="38829-167">**id**</span><span class="sxs-lookup"><span data-stu-id="38829-167">**id**</span></span>            | <span data-ttu-id="38829-168">string</span><span class="sxs-lookup"><span data-stu-id="38829-168">string</span></span>               | <span data-ttu-id="38829-169">内容类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="38829-169">The unique identifier of the content type.</span></span>
| <span data-ttu-id="38829-170">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="38829-170">**inheritedFrom**</span></span> | <span data-ttu-id="38829-171">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="38829-171">[itemReference][]</span></span>    | <span data-ttu-id="38829-172">如果此内容类型继承自另一个作用域（如某个站点），则会提供对在其中定义内容类型的项的引用。</span><span class="sxs-lookup"><span data-stu-id="38829-172">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="38829-173">**名称**</span><span class="sxs-lookup"><span data-stu-id="38829-173">**name**</span></span>          | <span data-ttu-id="38829-174">string</span><span class="sxs-lookup"><span data-stu-id="38829-174">string</span></span>               | <span data-ttu-id="38829-175">内容类型的名称。</span><span class="sxs-lookup"><span data-stu-id="38829-175">The name of the content type.</span></span>
| <span data-ttu-id="38829-176">**order**</span><span class="sxs-lookup"><span data-stu-id="38829-176">**order**</span></span>         | <span data-ttu-id="38829-177">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="38829-177">[contentTypeOrder][]</span></span> | <span data-ttu-id="38829-178">指定在选择 UI 中显示内容类型的顺序。</span><span class="sxs-lookup"><span data-stu-id="38829-178">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="38829-179">**parentId**</span><span class="sxs-lookup"><span data-stu-id="38829-179">**parentId**</span></span>      | <span data-ttu-id="38829-180">string</span><span class="sxs-lookup"><span data-stu-id="38829-180">string</span></span>               | <span data-ttu-id="38829-181">内容类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="38829-181">The unique identifier of the content type.</span></span>
| <span data-ttu-id="38829-182">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="38829-182">**readOnly**</span></span>      | <span data-ttu-id="38829-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="38829-183">Boolean</span></span>              | <span data-ttu-id="38829-184">如果为 `true`，则不能修改内容类型，除非此值首次设置为 `false`。</span><span class="sxs-lookup"><span data-stu-id="38829-184">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="38829-185">**sealed**</span><span class="sxs-lookup"><span data-stu-id="38829-185">**sealed**</span></span>        | <span data-ttu-id="38829-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="38829-186">Boolean</span></span>              | <span data-ttu-id="38829-187">如果为 `true`，则不能由用户或通过下推操作修改内容类型。</span><span class="sxs-lookup"><span data-stu-id="38829-187">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="38829-188">只有网站集管理员可以密封或解封内容类型。</span><span class="sxs-lookup"><span data-stu-id="38829-188">Only site collection administrators can seal or unseal content types.</span></span>
| <span data-ttu-id="38829-189">**isBuiltIn**</span><span class="sxs-lookup"><span data-stu-id="38829-189">**isBuiltIn**</span></span>            | <span data-ttu-id="38829-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="38829-190">Boolean</span></span>| <span data-ttu-id="38829-191">指定内容类型是否内置内容类型。</span><span class="sxs-lookup"><span data-stu-id="38829-191">Specifies if a content type is a built-in content type.</span></span> 
| <span data-ttu-id="38829-192">**documentSet**</span><span class="sxs-lookup"><span data-stu-id="38829-192">**documentSet**</span></span>       | <span data-ttu-id="38829-193">[documentSet][]</span><span class="sxs-lookup"><span data-stu-id="38829-193">[documentSet][]</span></span>      | <span data-ttu-id="38829-194">[文档集](https://docs.microsoft.com/sharepoint/governance/document-set-planning#about-document-sets) 元数据。</span><span class="sxs-lookup"><span data-stu-id="38829-194">[Document Set](https://docs.microsoft.com/sharepoint/governance/document-set-planning#about-document-sets) metadata.</span></span>
| <span data-ttu-id="38829-195">**documentTemplate**</span><span class="sxs-lookup"><span data-stu-id="38829-195">**documentTemplate**</span></span>  | <span data-ttu-id="38829-196">[documentSetContent][]</span><span class="sxs-lookup"><span data-stu-id="38829-196">[documentSetContent][]</span></span> | <span data-ttu-id="38829-197">文档模板元数据。</span><span class="sxs-lookup"><span data-stu-id="38829-197">Document template metadata.</span></span> <span data-ttu-id="38829-198">若要确保文档在网站及其子网站中具有一致的内容，您可以将 Word、Excel 或 PowerPoint 模板与网站内容类型关联。</span><span class="sxs-lookup"><span data-stu-id="38829-198">To make sure that documents have consistent content across a site and its subsites, you can associate a Word, Excel, or PowerPoint template with a site content type.</span></span>
| <span data-ttu-id="38829-199">**associatedHubsUrls**</span><span class="sxs-lookup"><span data-stu-id="38829-199">**associatedHubsUrls**</span></span>       | <span data-ttu-id="38829-200">集合 (字符串) </span><span class="sxs-lookup"><span data-stu-id="38829-200">Collection(string)</span></span> | <span data-ttu-id="38829-201">与此内容类型关联的中心网站的规范 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="38829-201">List of canonical URLs for hub sites with which this content type is associated to.</span></span> <span data-ttu-id="38829-202">这将包含此内容类型已排队以强制执行或已强制执行的所有中心网站。</span><span class="sxs-lookup"><span data-stu-id="38829-202">This will contain all hubsites where this content type is queued to be enforced or is already enforced.</span></span> <span data-ttu-id="38829-203">强制实施内容类型意味着内容类型将应用于强制网站中的列表。</span><span class="sxs-lookup"><span data-stu-id="38829-203">Enforcing a content type means that the content type will be applied to the lists in the enforced sites.</span></span>
| <span data-ttu-id="38829-204">**propagateChanges**</span><span class="sxs-lookup"><span data-stu-id="38829-204">**propagateChanges**</span></span>   | <span data-ttu-id="38829-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="38829-205">Boolean</span></span>              | <span data-ttu-id="38829-206">如果为 ，则对内容类型进行的任何更改都将推送到实现该内容类型的继承 `true` 内容类型和列表。</span><span class="sxs-lookup"><span data-stu-id="38829-206">If `true`, any changes made to the content type will be pushed to inherited content types and lists that implement the content type.</span></span>



## <a name="relationships"></a><span data-ttu-id="38829-207">关系</span><span class="sxs-lookup"><span data-stu-id="38829-207">Relationships</span></span>

| <span data-ttu-id="38829-208">属性名称</span><span class="sxs-lookup"><span data-stu-id="38829-208">Property name</span></span>   | <span data-ttu-id="38829-209">类型</span><span class="sxs-lookup"><span data-stu-id="38829-209">Type</span></span>                      | <span data-ttu-id="38829-210">说明</span><span class="sxs-lookup"><span data-stu-id="38829-210">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="38829-211">**base**</span><span class="sxs-lookup"><span data-stu-id="38829-211">**base**</span></span>   | <span data-ttu-id="38829-212">[contentType][]</span><span class="sxs-lookup"><span data-stu-id="38829-212">[contentType][]</span></span>  | <span data-ttu-id="38829-213">派生此内容类型的父 contentType。</span><span class="sxs-lookup"><span data-stu-id="38829-213">Parent contentType from which this content type is derived.</span></span> 
| <span data-ttu-id="38829-214">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="38829-214">**columnLinks**</span></span> | <span data-ttu-id="38829-215">[columnLink][] 集合</span><span class="sxs-lookup"><span data-stu-id="38829-215">[columnLink][] collection</span></span> | <span data-ttu-id="38829-216">此内容类型所需的列集合</span><span class="sxs-lookup"><span data-stu-id="38829-216">The collection of columns that are required by this content type</span></span>
| <span data-ttu-id="38829-217">**baseTypes**</span><span class="sxs-lookup"><span data-stu-id="38829-217">**baseTypes**</span></span>   | <span data-ttu-id="38829-218">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="38829-218">Collection([contentType][])</span></span>     | <span data-ttu-id="38829-219">作为此内容类型的上级的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="38829-219">The collection of content types that are ancestors of this content type.</span></span>
| <span data-ttu-id="38829-220">**columnPositions**</span><span class="sxs-lookup"><span data-stu-id="38829-220">**columnPositions**</span></span>       | <span data-ttu-id="38829-221">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="38829-221">Collection([columnDefinition][])</span></span> | <span data-ttu-id="38829-222">内容类型中的列顺序信息。</span><span class="sxs-lookup"><span data-stu-id="38829-222">Column order information in a content type.</span></span>
| <span data-ttu-id="38829-223">**columns**</span><span class="sxs-lookup"><span data-stu-id="38829-223">**columns**</span></span>     | <span data-ttu-id="38829-224">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="38829-224">Collection([columnDefinition][])</span></span>  | <span data-ttu-id="38829-225">此 contentType 的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="38829-225">The collection of column definitions for this contentType.</span></span>

<span data-ttu-id="38829-226">请参阅[内容类型和内容类型发布简介][contentTypeIntro]了解详细信息。</span><span class="sxs-lookup"><span data-stu-id="38829-226">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md
[columnDefinition]: columnDefinition.md
[contentType]: contentType.md
[documentSet]: documentSet.md
[documentSetContent]: documentSetContent.md

## <a name="json-representation"></a><span data-ttu-id="38829-234">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38829-234">JSON representation</span></span>

<span data-ttu-id="38829-235">下面是 **contentType** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38829-235">The following is a JSON representation of a **contentType** resource.</span></span>

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


