---
title: 标记资源类型
description: 表示电子数据展示标记，用于在审阅期间标记文档以分隔响应和非响应内容
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: dee53c5a7d8320822101addcf5764420456e703f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446655"
---
# <a name="tag-resource-type"></a><span data-ttu-id="eb5ed-103">标记资源类型</span><span class="sxs-lookup"><span data-stu-id="eb5ed-103">tag resource type</span></span>

<span data-ttu-id="eb5ed-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="eb5ed-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb5ed-105">表示电子数据展示标记，用于在审阅过程中标记文档，以分隔响应和非响应内容。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-105">Represents an eDiscovery tag, which is used to mark documents during review to separate responsive and non-responsive content.</span></span>

<span data-ttu-id="eb5ed-106">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="eb5ed-107">Methods</span><span class="sxs-lookup"><span data-stu-id="eb5ed-107">Methods</span></span>

|<span data-ttu-id="eb5ed-108">方法</span><span class="sxs-lookup"><span data-stu-id="eb5ed-108">Method</span></span>|<span data-ttu-id="eb5ed-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="eb5ed-109">Return type</span></span>|<span data-ttu-id="eb5ed-110">说明</span><span class="sxs-lookup"><span data-stu-id="eb5ed-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eb5ed-111">列表标记</span><span class="sxs-lookup"><span data-stu-id="eb5ed-111">List tags</span></span>](../api/ediscovery-case-list-tags.md)|<span data-ttu-id="eb5ed-112">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb5ed-112">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="eb5ed-113">获取标记对象 **及其** 属性的列表。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-113">Get a list of the **tag** objects and their properties.</span></span>|
|[<span data-ttu-id="eb5ed-114">创建标记</span><span class="sxs-lookup"><span data-stu-id="eb5ed-114">Create tag</span></span>](../api/ediscovery-case-post-tags.md)|[<span data-ttu-id="eb5ed-115">microsoft.graph.ediscovery.tag</span><span class="sxs-lookup"><span data-stu-id="eb5ed-115">microsoft.graph.ediscovery.tag</span></span>](../resources/ediscovery-tag.md)|<span data-ttu-id="eb5ed-116">创建新的 **标记** 对象。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-116">Create a new **tag** object.</span></span>|
|[<span data-ttu-id="eb5ed-117">获取标记</span><span class="sxs-lookup"><span data-stu-id="eb5ed-117">Get tag</span></span>](../api/ediscovery-tag-get.md)|[<span data-ttu-id="eb5ed-118">microsoft.graph.ediscovery.tag</span><span class="sxs-lookup"><span data-stu-id="eb5ed-118">microsoft.graph.ediscovery.tag</span></span>](../resources/ediscovery-tag.md)|<span data-ttu-id="eb5ed-119">读取标记对象 **的属性** 和关系。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-119">Read the properties and relationships of a **tag** object.</span></span>|
|[<span data-ttu-id="eb5ed-120">更新标记</span><span class="sxs-lookup"><span data-stu-id="eb5ed-120">Update tag</span></span>](../api/ediscovery-tag-update.md)|[<span data-ttu-id="eb5ed-121">microsoft.graph.ediscovery.tag</span><span class="sxs-lookup"><span data-stu-id="eb5ed-121">microsoft.graph.ediscovery.tag</span></span>](../resources/ediscovery-tag.md)|<span data-ttu-id="eb5ed-122">更新 **标记对象的属性** 。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-122">Update the properties of a **tag** object.</span></span>|
|[<span data-ttu-id="eb5ed-123">删除标记</span><span class="sxs-lookup"><span data-stu-id="eb5ed-123">Delete tag</span></span>](../api/ediscovery-tag-delete.md)|<span data-ttu-id="eb5ed-124">无</span><span class="sxs-lookup"><span data-stu-id="eb5ed-124">None</span></span>|<span data-ttu-id="eb5ed-125">删除 **标记** 对象。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-125">Delete a **tag** object.</span></span>|
|[<span data-ttu-id="eb5ed-126">asHierarchy</span><span class="sxs-lookup"><span data-stu-id="eb5ed-126">asHierarchy</span></span>](../api/ediscovery-tag-ashierarchy.md)|<span data-ttu-id="eb5ed-127">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb5ed-127">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="eb5ed-128">列出所有标记，包括其层次结构。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-128">Lists all tags, including their hierarchy.</span></span>|
|[<span data-ttu-id="eb5ed-129">列出 childTags</span><span class="sxs-lookup"><span data-stu-id="eb5ed-129">List childTags</span></span>](../api/ediscovery-tag-childtags.md)|<span data-ttu-id="eb5ed-130">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb5ed-130">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="eb5ed-131">获取与 **标记关联的** 子标记对象列表。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-131">Get a list of child **tag** objects associated with a tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="eb5ed-132">属性</span><span class="sxs-lookup"><span data-stu-id="eb5ed-132">Properties</span></span>

|<span data-ttu-id="eb5ed-133">属性</span><span class="sxs-lookup"><span data-stu-id="eb5ed-133">Property</span></span>|<span data-ttu-id="eb5ed-134">类型</span><span class="sxs-lookup"><span data-stu-id="eb5ed-134">Type</span></span>|<span data-ttu-id="eb5ed-135">说明</span><span class="sxs-lookup"><span data-stu-id="eb5ed-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb5ed-136">childSelectability</span><span class="sxs-lookup"><span data-stu-id="eb5ed-136">childSelectability</span></span>|[<span data-ttu-id="eb5ed-137">microsoft.graph.ediscovery.childSelectability</span><span class="sxs-lookup"><span data-stu-id="eb5ed-137">microsoft.graph.ediscovery.childSelectability</span></span>](../resources/ediscovery-tag.md#childselectability-values)|<span data-ttu-id="eb5ed-138">指示单个或多个子标记是否可以与文档关联。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-138">Indicates whether a single or multiple child tags can be associated with a document.</span></span> <span data-ttu-id="eb5ed-139">可取值为：`One`、`Many`。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-139">Possible values are: `One`, `Many`.</span></span>  <span data-ttu-id="eb5ed-140">此值控制 UX 是作为复选框还是单选按钮组显示标记。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-140">This value controls whether the UX presents the tags as checkboxes or a radio button group.</span></span>|
|<span data-ttu-id="eb5ed-141">createdBy</span><span class="sxs-lookup"><span data-stu-id="eb5ed-141">createdBy</span></span>|[<span data-ttu-id="eb5ed-142">identitySet</span><span class="sxs-lookup"><span data-stu-id="eb5ed-142">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="eb5ed-143">创建标记的用户。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-143">The user who created the tag.</span></span>|
|<span data-ttu-id="eb5ed-144">说明</span><span class="sxs-lookup"><span data-stu-id="eb5ed-144">description</span></span>|<span data-ttu-id="eb5ed-145">String</span><span class="sxs-lookup"><span data-stu-id="eb5ed-145">String</span></span>|<span data-ttu-id="eb5ed-146">标记的说明。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-146">The description for the tag.</span></span>|
|<span data-ttu-id="eb5ed-147">displayName</span><span class="sxs-lookup"><span data-stu-id="eb5ed-147">displayName</span></span>|<span data-ttu-id="eb5ed-148">String</span><span class="sxs-lookup"><span data-stu-id="eb5ed-148">String</span></span>|<span data-ttu-id="eb5ed-149">标记的显示名称。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-149">Display name of the tag.</span></span>|
|<span data-ttu-id="eb5ed-150">id</span><span class="sxs-lookup"><span data-stu-id="eb5ed-150">id</span></span>|<span data-ttu-id="eb5ed-151">String</span><span class="sxs-lookup"><span data-stu-id="eb5ed-151">String</span></span>|<span data-ttu-id="eb5ed-152">标记的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-152">Unique identifier for the tag.</span></span>|
|<span data-ttu-id="eb5ed-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb5ed-153">lastModifiedDateTime</span></span>|<span data-ttu-id="eb5ed-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb5ed-154">DateTimeOffset</span></span>|<span data-ttu-id="eb5ed-155">上次修改标记的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-155">The date and time the tag was last modified.</span></span>|

### <a name="childselectability-values"></a><span data-ttu-id="eb5ed-156">childSelectability 值</span><span class="sxs-lookup"><span data-stu-id="eb5ed-156">childSelectability values</span></span>

|<span data-ttu-id="eb5ed-157">成员</span><span class="sxs-lookup"><span data-stu-id="eb5ed-157">Member</span></span>|<span data-ttu-id="eb5ed-158">说明</span><span class="sxs-lookup"><span data-stu-id="eb5ed-158">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="eb5ed-159">一个</span><span class="sxs-lookup"><span data-stu-id="eb5ed-159">One</span></span>|<span data-ttu-id="eb5ed-160">只能选择一个子级。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-160">Only one child can be selected.</span></span> <span data-ttu-id="eb5ed-161">这与显示具有单选按钮的标记的 UI 相对应。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-161">This corresponds to a UI that presents the tags with radio buttons.</span></span>|
|<span data-ttu-id="eb5ed-162">许多</span><span class="sxs-lookup"><span data-stu-id="eb5ed-162">Many</span></span>|<span data-ttu-id="eb5ed-163">可以选择零个或多个子级。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-163">Zero or many children can be selected.</span></span> <span data-ttu-id="eb5ed-164">这与显示带复选框的标记的 UI 相对应。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-164">This corresponds to a UI that presents the tags with checkboxes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb5ed-165">关系</span><span class="sxs-lookup"><span data-stu-id="eb5ed-165">Relationships</span></span>

|<span data-ttu-id="eb5ed-166">关系</span><span class="sxs-lookup"><span data-stu-id="eb5ed-166">Relationship</span></span>|<span data-ttu-id="eb5ed-167">类型</span><span class="sxs-lookup"><span data-stu-id="eb5ed-167">Type</span></span>|<span data-ttu-id="eb5ed-168">说明</span><span class="sxs-lookup"><span data-stu-id="eb5ed-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb5ed-169">childTags</span><span class="sxs-lookup"><span data-stu-id="eb5ed-169">childTags</span></span>|<span data-ttu-id="eb5ed-170">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb5ed-170">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="eb5ed-171">返回标记的子级标记。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-171">Returns the tags that are a child of a tag.</span></span>|
|<span data-ttu-id="eb5ed-172">父级</span><span class="sxs-lookup"><span data-stu-id="eb5ed-172">parent</span></span>|[<span data-ttu-id="eb5ed-173">microsoft.graph.ediscovery.tag</span><span class="sxs-lookup"><span data-stu-id="eb5ed-173">microsoft.graph.ediscovery.tag</span></span>](../resources/ediscovery-tag.md)|<span data-ttu-id="eb5ed-174">返回指定标记的父标记。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-174">Returns the parent tag of the specified tag.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb5ed-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb5ed-175">JSON representation</span></span>

<span data-ttu-id="eb5ed-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb5ed-176">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.tag",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.tag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "childSelectability": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```
