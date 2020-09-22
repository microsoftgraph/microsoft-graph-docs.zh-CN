---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
description: FolderView 资源提供或设置关于文件夹的用户体验建议。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 749b66b50545b6bc7de66647c47153227cb54fa7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018275"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="10fd3-103">FolderView 资源类型</span><span class="sxs-lookup"><span data-stu-id="10fd3-103">FolderView resource type</span></span>

<span data-ttu-id="10fd3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10fd3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="10fd3-105">**FolderView** 资源提供或设置关于文件夹的用户体验建议。</span><span class="sxs-lookup"><span data-stu-id="10fd3-105">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="10fd3-106">它可从[driveItem][item-resource]资源的[folder][folder-facet]属性中获取。</span><span class="sxs-lookup"><span data-stu-id="10fd3-106">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="10fd3-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10fd3-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortOrder": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="10fd3-108">属性</span><span class="sxs-lookup"><span data-stu-id="10fd3-108">Properties</span></span>

| <span data-ttu-id="10fd3-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="10fd3-109">Property name</span></span>         | <span data-ttu-id="10fd3-110">类型</span><span class="sxs-lookup"><span data-stu-id="10fd3-110">Type</span></span>   | <span data-ttu-id="10fd3-111">说明</span><span class="sxs-lookup"><span data-stu-id="10fd3-111">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="10fd3-112">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="10fd3-112">**sortBy**</span></span>            | <span data-ttu-id="10fd3-113">string</span><span class="sxs-lookup"><span data-stu-id="10fd3-113">string</span></span> | <span data-ttu-id="10fd3-114">文件夹应采用的排序方法。</span><span class="sxs-lookup"><span data-stu-id="10fd3-114">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="10fd3-115">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="10fd3-115">**sortOrder**</span></span>         | <span data-ttu-id="10fd3-116">string</span><span class="sxs-lookup"><span data-stu-id="10fd3-116">string</span></span> | <span data-ttu-id="10fd3-p101">如果为 true，表明应按降序排列项。 否则，应按升序排列项。</span><span class="sxs-lookup"><span data-stu-id="10fd3-p101">If true, indicates that items should be sorted in descending order. Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="10fd3-119">**viewType**</span><span class="sxs-lookup"><span data-stu-id="10fd3-119">**viewType**</span></span>          | <span data-ttu-id="10fd3-120">string</span><span class="sxs-lookup"><span data-stu-id="10fd3-120">string</span></span> | <span data-ttu-id="10fd3-121">应用于表示文件夹的视图类型。</span><span class="sxs-lookup"><span data-stu-id="10fd3-121">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="10fd3-122">可以使用 _sortBy_ 属性控制遵循 **viewType** Facet 的应用中项的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="10fd3-122">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-options"></a><span data-ttu-id="10fd3-123">sortBy 选项</span><span class="sxs-lookup"><span data-stu-id="10fd3-123">sortBy options</span></span>

<span data-ttu-id="10fd3-124">以下值是针对 **sortBy** 属性进行定义。</span><span class="sxs-lookup"><span data-stu-id="10fd3-124">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="10fd3-125">值</span><span class="sxs-lookup"><span data-stu-id="10fd3-125">Value</span></span>                    | <span data-ttu-id="10fd3-126">说明</span><span class="sxs-lookup"><span data-stu-id="10fd3-126">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="10fd3-127">应用的默认排序顺序。</span><span class="sxs-lookup"><span data-stu-id="10fd3-127">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="10fd3-128">应按项的 **name** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="10fd3-128">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="10fd3-129">应按项类型排列项。</span><span class="sxs-lookup"><span data-stu-id="10fd3-129">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="10fd3-130">应按项的 **size** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="10fd3-130">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="10fd3-p102">应按 **Photo** Facet 的 **takenDateTime** 属性排列项。 如果此属性不可用，应按 **createdDateTime** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="10fd3-p102">Items should be arranged by the **takenDateTime** property of the **photo** facet. If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="10fd3-133">应按项的 **lastModifiedDateTime** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="10fd3-133">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="10fd3-134">这些项按照用户指定的自定义序列排列。</span><span class="sxs-lookup"><span data-stu-id="10fd3-134">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-options"></a><span data-ttu-id="10fd3-135">sortOrder 选项</span><span class="sxs-lookup"><span data-stu-id="10fd3-135">sortOrder options</span></span>

<span data-ttu-id="10fd3-136">以下值是针对 **sortOrder** 属性进行定义。</span><span class="sxs-lookup"><span data-stu-id="10fd3-136">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="10fd3-137">值</span><span class="sxs-lookup"><span data-stu-id="10fd3-137">Value</span></span>        | <span data-ttu-id="10fd3-138">说明</span><span class="sxs-lookup"><span data-stu-id="10fd3-138">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="10fd3-139">应按升序排列项。</span><span class="sxs-lookup"><span data-stu-id="10fd3-139">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="10fd3-140">应按降序排列项。</span><span class="sxs-lookup"><span data-stu-id="10fd3-140">Items should be arranged in descending order.</span></span>


### <a name="viewtype-options"></a><span data-ttu-id="10fd3-141">viewType 选项</span><span class="sxs-lookup"><span data-stu-id="10fd3-141">viewType options</span></span>

<span data-ttu-id="10fd3-142">以下值是针对 **viewType** 属性进行定义。</span><span class="sxs-lookup"><span data-stu-id="10fd3-142">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="10fd3-143">值</span><span class="sxs-lookup"><span data-stu-id="10fd3-143">Value</span></span>        | <span data-ttu-id="10fd3-144">说明</span><span class="sxs-lookup"><span data-stu-id="10fd3-144">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="10fd3-145">应用的默认视图类型。</span><span class="sxs-lookup"><span data-stu-id="10fd3-145">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="10fd3-146">使用图标表示 driveItem 的视图。</span><span class="sxs-lookup"><span data-stu-id="10fd3-146">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="10fd3-147">使用多个列提供每一项的其他详细信息的视图。</span><span class="sxs-lookup"><span data-stu-id="10fd3-147">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="10fd3-148">使用 driveItem 的大缩略图表示项的视图。</span><span class="sxs-lookup"><span data-stu-id="10fd3-148">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- {
  "type": "#page.annotation",
  "description": "The FolderView facet provides or sets recommendations on the user-experience of a folder.",
  "keywords": "view, folderview, sortby, sortorder, viewtype, coversourceid, folder",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,icons,details,thumbnails) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,name,type,size,takenOrCreatedDateTime,lastModifiedDateTime,sequence) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(ascending,descending) are in resource, but () are in table"
  ],
  "tocPath": "Facets/FolderView"
} -->

