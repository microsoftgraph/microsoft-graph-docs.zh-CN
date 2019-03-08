---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: f82242da39ebc13d769a0a3471b60dd4ac9df8dc
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480920"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="3d43b-102">FolderView 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d43b-102">FolderView resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d43b-103">**FolderView** 资源提供或设置关于文件夹的用户体验建议。</span><span class="sxs-lookup"><span data-stu-id="3d43b-103">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="3d43b-104">可通过 [driveItem][item-resource] 资源的 [folder][folder-facet] 属性获取。</span><span class="sxs-lookup"><span data-stu-id="3d43b-104">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d43b-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d43b-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="3d43b-106">属性</span><span class="sxs-lookup"><span data-stu-id="3d43b-106">Properties</span></span>

| <span data-ttu-id="3d43b-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="3d43b-107">Property name</span></span>         | <span data-ttu-id="3d43b-108">类型</span><span class="sxs-lookup"><span data-stu-id="3d43b-108">Type</span></span>   | <span data-ttu-id="3d43b-109">说明</span><span class="sxs-lookup"><span data-stu-id="3d43b-109">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="3d43b-110">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="3d43b-110">**sortBy**</span></span>            | <span data-ttu-id="3d43b-111">string</span><span class="sxs-lookup"><span data-stu-id="3d43b-111">string</span></span> | <span data-ttu-id="3d43b-112">文件夹应采用的排序方法。</span><span class="sxs-lookup"><span data-stu-id="3d43b-112">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="3d43b-113">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="3d43b-113">**sortOrder**</span></span>         | <span data-ttu-id="3d43b-114">string</span><span class="sxs-lookup"><span data-stu-id="3d43b-114">string</span></span> | <span data-ttu-id="3d43b-p101">如果为 true，表明应按降序排列项。 否则，应按升序排列项。</span><span class="sxs-lookup"><span data-stu-id="3d43b-p101">If true, indicates that items should be sorted in descending order. Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="3d43b-117">**viewType**</span><span class="sxs-lookup"><span data-stu-id="3d43b-117">**viewType**</span></span>          | <span data-ttu-id="3d43b-118">string</span><span class="sxs-lookup"><span data-stu-id="3d43b-118">string</span></span> | <span data-ttu-id="3d43b-119">应用于表示文件夹的视图类型。</span><span class="sxs-lookup"><span data-stu-id="3d43b-119">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="3d43b-120">可以使用 _sortBy_ 属性控制遵循 **viewType** Facet 的应用中项的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="3d43b-120">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="3d43b-121">sortBy 值</span><span class="sxs-lookup"><span data-stu-id="3d43b-121">sortBy values</span></span>

<span data-ttu-id="3d43b-122">以下值是针对 **sortBy** 属性进行定义。</span><span class="sxs-lookup"><span data-stu-id="3d43b-122">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="3d43b-123">值</span><span class="sxs-lookup"><span data-stu-id="3d43b-123">Value</span></span>                    | <span data-ttu-id="3d43b-124">说明</span><span class="sxs-lookup"><span data-stu-id="3d43b-124">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="3d43b-125">应用的默认排序顺序。</span><span class="sxs-lookup"><span data-stu-id="3d43b-125">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="3d43b-126">应按项的 **name** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="3d43b-126">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="3d43b-127">应按项类型排列项。</span><span class="sxs-lookup"><span data-stu-id="3d43b-127">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="3d43b-128">应按项的 **size** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="3d43b-128">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="3d43b-p102">应按 **Photo** Facet 的 **takenDateTime** 属性排列项。 如果此属性不可用，应按 **createdDateTime** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="3d43b-p102">Items should be arranged by the **takenDateTime** property of the **photo** facet. If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="3d43b-131">应按项的 **lastModifiedDateTime** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="3d43b-131">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="3d43b-132">这些项按照用户指定的自定义序列排列。</span><span class="sxs-lookup"><span data-stu-id="3d43b-132">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="3d43b-133">sortOrder 值</span><span class="sxs-lookup"><span data-stu-id="3d43b-133">sortOrder values</span></span>

<span data-ttu-id="3d43b-134">以下值是针对 **sortOrder** 属性进行定义。</span><span class="sxs-lookup"><span data-stu-id="3d43b-134">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="3d43b-135">值</span><span class="sxs-lookup"><span data-stu-id="3d43b-135">Value</span></span>        | <span data-ttu-id="3d43b-136">说明</span><span class="sxs-lookup"><span data-stu-id="3d43b-136">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="3d43b-137">应按升序排列项。</span><span class="sxs-lookup"><span data-stu-id="3d43b-137">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="3d43b-138">应按降序排列项。</span><span class="sxs-lookup"><span data-stu-id="3d43b-138">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="3d43b-139">viewType 值</span><span class="sxs-lookup"><span data-stu-id="3d43b-139">viewType values</span></span>

<span data-ttu-id="3d43b-140">以下值是针对 **viewType** 属性进行定义。</span><span class="sxs-lookup"><span data-stu-id="3d43b-140">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="3d43b-141">值</span><span class="sxs-lookup"><span data-stu-id="3d43b-141">Value</span></span>        | <span data-ttu-id="3d43b-142">说明</span><span class="sxs-lookup"><span data-stu-id="3d43b-142">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="3d43b-143">应用的默认视图类型。</span><span class="sxs-lookup"><span data-stu-id="3d43b-143">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="3d43b-144">使用图标表示 driveItem 的视图。</span><span class="sxs-lookup"><span data-stu-id="3d43b-144">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="3d43b-145">使用多个列提供每一项的其他详细信息的视图。</span><span class="sxs-lookup"><span data-stu-id="3d43b-145">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="3d43b-146">使用 driveItem 的大缩略图表示项的视图。</span><span class="sxs-lookup"><span data-stu-id="3d43b-146">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


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
  "suppressions": [
    "Error: /api-reference/beta/resources/folderview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
