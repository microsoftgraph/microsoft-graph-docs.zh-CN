---
author: JeremyKelley
description: FolderView 资源提供或设置关于文件夹的用户体验建议。
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 5238c749d509339cd0e922e49b7e2d4d2da3b23f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973546"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="4b080-103">FolderView 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b080-103">FolderView resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b080-104">**FolderView** 资源提供或设置关于文件夹的用户体验建议。</span><span class="sxs-lookup"><span data-stu-id="4b080-104">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="4b080-105">它可从[driveItem][item-resource]资源的[folder][folder-facet]属性中获取。</span><span class="sxs-lookup"><span data-stu-id="4b080-105">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b080-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b080-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "viewType": "default | icons | details | thumbnails",
  "sortOrder": "string"
}
```

## <a name="properties"></a><span data-ttu-id="4b080-107">属性</span><span class="sxs-lookup"><span data-stu-id="4b080-107">Properties</span></span>

| <span data-ttu-id="4b080-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="4b080-108">Property name</span></span>         | <span data-ttu-id="4b080-109">类型</span><span class="sxs-lookup"><span data-stu-id="4b080-109">Type</span></span>   | <span data-ttu-id="4b080-110">说明</span><span class="sxs-lookup"><span data-stu-id="4b080-110">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="4b080-111">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="4b080-111">**sortBy**</span></span>            | <span data-ttu-id="4b080-112">string</span><span class="sxs-lookup"><span data-stu-id="4b080-112">string</span></span> | <span data-ttu-id="4b080-113">文件夹应采用的排序方法。</span><span class="sxs-lookup"><span data-stu-id="4b080-113">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="4b080-114">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="4b080-114">**sortOrder**</span></span>         | <span data-ttu-id="4b080-115">string</span><span class="sxs-lookup"><span data-stu-id="4b080-115">string</span></span> | <span data-ttu-id="4b080-p101">如果为 true，表明应按降序排列项。 否则，应按升序排列项。</span><span class="sxs-lookup"><span data-stu-id="4b080-p101">If true, indicates that items should be sorted in descending order. Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="4b080-118">**viewType**</span><span class="sxs-lookup"><span data-stu-id="4b080-118">**viewType**</span></span>          | <span data-ttu-id="4b080-119">string</span><span class="sxs-lookup"><span data-stu-id="4b080-119">string</span></span> | <span data-ttu-id="4b080-120">应用于表示文件夹的视图类型。</span><span class="sxs-lookup"><span data-stu-id="4b080-120">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="4b080-121">可以使用 _sortBy_ 属性控制遵循 **viewType** Facet 的应用中项的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="4b080-121">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="4b080-122">sortBy 值</span><span class="sxs-lookup"><span data-stu-id="4b080-122">sortBy values</span></span>

<span data-ttu-id="4b080-123">以下值是针对 **sortBy** 属性进行定义。</span><span class="sxs-lookup"><span data-stu-id="4b080-123">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="4b080-124">值</span><span class="sxs-lookup"><span data-stu-id="4b080-124">Value</span></span>                    | <span data-ttu-id="4b080-125">说明</span><span class="sxs-lookup"><span data-stu-id="4b080-125">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="4b080-126">应用的默认排序顺序。</span><span class="sxs-lookup"><span data-stu-id="4b080-126">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="4b080-127">应按项的 **name** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="4b080-127">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="4b080-128">应按项类型排列项。</span><span class="sxs-lookup"><span data-stu-id="4b080-128">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="4b080-129">应按项的 **size** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="4b080-129">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="4b080-p102">应按 **Photo** Facet 的 **takenDateTime** 属性排列项。 如果此属性不可用，应按 **createdDateTime** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="4b080-p102">Items should be arranged by the **takenDateTime** property of the **photo** facet. If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="4b080-132">应按项的 **lastModifiedDateTime** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="4b080-132">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="4b080-133">这些项按照用户指定的自定义序列排列。</span><span class="sxs-lookup"><span data-stu-id="4b080-133">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="4b080-134">sortOrder 值</span><span class="sxs-lookup"><span data-stu-id="4b080-134">sortOrder values</span></span>

<span data-ttu-id="4b080-135">以下值是针对 **sortOrder** 属性进行定义。</span><span class="sxs-lookup"><span data-stu-id="4b080-135">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="4b080-136">值</span><span class="sxs-lookup"><span data-stu-id="4b080-136">Value</span></span>        | <span data-ttu-id="4b080-137">说明</span><span class="sxs-lookup"><span data-stu-id="4b080-137">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="4b080-138">应按升序排列项。</span><span class="sxs-lookup"><span data-stu-id="4b080-138">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="4b080-139">应按降序排列项。</span><span class="sxs-lookup"><span data-stu-id="4b080-139">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="4b080-140">viewType 值</span><span class="sxs-lookup"><span data-stu-id="4b080-140">viewType values</span></span>

<span data-ttu-id="4b080-141">以下值是针对 **viewType** 属性进行定义。</span><span class="sxs-lookup"><span data-stu-id="4b080-141">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="4b080-142">值</span><span class="sxs-lookup"><span data-stu-id="4b080-142">Value</span></span>        | <span data-ttu-id="4b080-143">说明</span><span class="sxs-lookup"><span data-stu-id="4b080-143">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="4b080-144">应用的默认视图类型。</span><span class="sxs-lookup"><span data-stu-id="4b080-144">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="4b080-145">使用图标表示 driveItem 的视图。</span><span class="sxs-lookup"><span data-stu-id="4b080-145">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="4b080-146">使用多个列提供每一项的其他详细信息的视图。</span><span class="sxs-lookup"><span data-stu-id="4b080-146">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="4b080-147">使用 driveItem 的大缩略图表示项的视图。</span><span class="sxs-lookup"><span data-stu-id="4b080-147">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
