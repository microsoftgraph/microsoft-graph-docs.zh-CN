---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FolderView
ms.openlocfilehash: e73846a18f8576af8fe3cf5949e8ca5c63891837
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265153"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="47933-102">FolderView 资源类型</span><span class="sxs-lookup"><span data-stu-id="47933-102">FolderView resource type</span></span>

<span data-ttu-id="47933-103">**FolderView** 资源提供或设置关于文件夹的用户体验建议。</span><span class="sxs-lookup"><span data-stu-id="47933-103">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="47933-104">可通过 [driveItem][item-resource] 资源的 [folder][folder-facet] 属性获取。</span><span class="sxs-lookup"><span data-stu-id="47933-104">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="47933-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47933-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortOrder": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="47933-106">属性</span><span class="sxs-lookup"><span data-stu-id="47933-106">Properties</span></span>

| <span data-ttu-id="47933-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="47933-107">Property name</span></span>         | <span data-ttu-id="47933-108">类型</span><span class="sxs-lookup"><span data-stu-id="47933-108">Type</span></span>   | <span data-ttu-id="47933-109">说明</span><span class="sxs-lookup"><span data-stu-id="47933-109">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="47933-110">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="47933-110">**sortBy**</span></span>            | <span data-ttu-id="47933-111">字符串</span><span class="sxs-lookup"><span data-stu-id="47933-111">string</span></span> | <span data-ttu-id="47933-112">文件夹应采用的排序方法。</span><span class="sxs-lookup"><span data-stu-id="47933-112">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="47933-113">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="47933-113">**sortOrder**</span></span>         | <span data-ttu-id="47933-114">字符串</span><span class="sxs-lookup"><span data-stu-id="47933-114">string</span></span> | <span data-ttu-id="47933-115">如果为 true，表明应按降序排列项。</span><span class="sxs-lookup"><span data-stu-id="47933-115">If true, indicates that items should be sorted in descending order.</span></span> <span data-ttu-id="47933-116">否则，应按升序排列项。</span><span class="sxs-lookup"><span data-stu-id="47933-116">Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="47933-117">**viewType**</span><span class="sxs-lookup"><span data-stu-id="47933-117">**viewType**</span></span>          | <span data-ttu-id="47933-118">字符串</span><span class="sxs-lookup"><span data-stu-id="47933-118">string</span></span> | <span data-ttu-id="47933-119">应用于表示文件夹的视图类型。</span><span class="sxs-lookup"><span data-stu-id="47933-119">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="47933-120">可以使用 _sortBy_ 属性控制遵循 **viewType** Facet 的应用中项的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="47933-120">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-options"></a><span data-ttu-id="47933-121">sortBy 选项</span><span class="sxs-lookup"><span data-stu-id="47933-121">sortBy options</span></span>

<span data-ttu-id="47933-122">以下值是针对 **sortBy** 属性进行定义。</span><span class="sxs-lookup"><span data-stu-id="47933-122">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="47933-123">值</span><span class="sxs-lookup"><span data-stu-id="47933-123">Value</span></span>                    | <span data-ttu-id="47933-124">说明</span><span class="sxs-lookup"><span data-stu-id="47933-124">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="47933-125">应用的默认排序顺序。</span><span class="sxs-lookup"><span data-stu-id="47933-125">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="47933-126">应按项的 **name** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="47933-126">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="47933-127">应按项类型排列项。</span><span class="sxs-lookup"><span data-stu-id="47933-127">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="47933-128">应按项的 **size** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="47933-128">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="47933-129">应按 **Photo** Facet 的 **takenDateTime** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="47933-129">Items should be arranged by the **takenDateTime** property of the **photo** facet.</span></span> <span data-ttu-id="47933-130">如果此属性不可用，应按 **createdDateTime** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="47933-130">If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="47933-131">应按项的 **lastModifiedDateTime** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="47933-131">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="47933-132">这些项按照用户指定的自定义序列排列。</span><span class="sxs-lookup"><span data-stu-id="47933-132">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-options"></a><span data-ttu-id="47933-133">sortOrder 选项</span><span class="sxs-lookup"><span data-stu-id="47933-133">sortOrder options</span></span>

<span data-ttu-id="47933-134">以下值是针对 **sortOrder** 属性进行定义。</span><span class="sxs-lookup"><span data-stu-id="47933-134">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="47933-135">值</span><span class="sxs-lookup"><span data-stu-id="47933-135">Value</span></span>        | <span data-ttu-id="47933-136">说明</span><span class="sxs-lookup"><span data-stu-id="47933-136">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="47933-137">应按升序排列项。</span><span class="sxs-lookup"><span data-stu-id="47933-137">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="47933-138">应按降序排列项。</span><span class="sxs-lookup"><span data-stu-id="47933-138">Items should be arranged in descending order.</span></span>


### <a name="viewtype-options"></a><span data-ttu-id="47933-139">viewType 选项</span><span class="sxs-lookup"><span data-stu-id="47933-139">viewType options</span></span>

<span data-ttu-id="47933-140">以下值是针对 **viewType** 属性进行定义。</span><span class="sxs-lookup"><span data-stu-id="47933-140">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="47933-141">值</span><span class="sxs-lookup"><span data-stu-id="47933-141">Value</span></span>        | <span data-ttu-id="47933-142">说明</span><span class="sxs-lookup"><span data-stu-id="47933-142">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="47933-143">应用的默认视图类型。</span><span class="sxs-lookup"><span data-stu-id="47933-143">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="47933-144">使用图标表示 driveItem 的视图。</span><span class="sxs-lookup"><span data-stu-id="47933-144">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="47933-145">使用多个列提供每一项的其他详细信息的视图。</span><span class="sxs-lookup"><span data-stu-id="47933-145">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="47933-146">使用 driveItem 的大缩略图表示项的视图。</span><span class="sxs-lookup"><span data-stu-id="47933-146">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


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
