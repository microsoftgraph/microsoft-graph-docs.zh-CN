---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FolderView
ms.openlocfilehash: 1658751371f3a3ae186d5a092ae5610f016d26b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041776"
---
# <a name="folderview-resource-type"></a><span data-ttu-id="9b23d-102">FolderView 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b23d-102">FolderView resource type</span></span>

> <span data-ttu-id="9b23d-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9b23d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b23d-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9b23d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b23d-105">**FolderView** 资源提供或设置关于文件夹的用户体验建议。</span><span class="sxs-lookup"><span data-stu-id="9b23d-105">The **FolderView** resource provides or sets recommendations on the user-experience of a folder.</span></span>

<span data-ttu-id="9b23d-106">可通过 [driveItem][item-resource] 资源的 [folder][folder-facet] 属性获取。</span><span class="sxs-lookup"><span data-stu-id="9b23d-106">It is available from the [folder][folder-facet] property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b23d-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b23d-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a><span data-ttu-id="9b23d-108">属性</span><span class="sxs-lookup"><span data-stu-id="9b23d-108">Properties</span></span>

| <span data-ttu-id="9b23d-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="9b23d-109">Property name</span></span>         | <span data-ttu-id="9b23d-110">类型</span><span class="sxs-lookup"><span data-stu-id="9b23d-110">Type</span></span>   | <span data-ttu-id="9b23d-111">说明</span><span class="sxs-lookup"><span data-stu-id="9b23d-111">Description</span></span>
|:----------------------|:-------|:--------------------------------------------
| <span data-ttu-id="9b23d-112">**sortBy**</span><span class="sxs-lookup"><span data-stu-id="9b23d-112">**sortBy**</span></span>            | <span data-ttu-id="9b23d-113">string</span><span class="sxs-lookup"><span data-stu-id="9b23d-113">string</span></span> | <span data-ttu-id="9b23d-114">文件夹应采用的排序方法。</span><span class="sxs-lookup"><span data-stu-id="9b23d-114">The method by which the folder should be sorted.</span></span>
| <span data-ttu-id="9b23d-115">**sortOrder**</span><span class="sxs-lookup"><span data-stu-id="9b23d-115">**sortOrder**</span></span>         | <span data-ttu-id="9b23d-116">string</span><span class="sxs-lookup"><span data-stu-id="9b23d-116">string</span></span> | <span data-ttu-id="9b23d-117">如果为 true，表明应按降序排列项。</span><span class="sxs-lookup"><span data-stu-id="9b23d-117">If true, indicates that items should be sorted in descending order.</span></span> <span data-ttu-id="9b23d-118">否则，应按升序排列项。</span><span class="sxs-lookup"><span data-stu-id="9b23d-118">Otherwise, items should be sorted ascending.</span></span>
| <span data-ttu-id="9b23d-119">**viewType**</span><span class="sxs-lookup"><span data-stu-id="9b23d-119">**viewType**</span></span>          | <span data-ttu-id="9b23d-120">string</span><span class="sxs-lookup"><span data-stu-id="9b23d-120">string</span></span> | <span data-ttu-id="9b23d-121">应用于表示文件夹的视图类型。</span><span class="sxs-lookup"><span data-stu-id="9b23d-121">The type of view that should be used to represent the folder.</span></span>

<span data-ttu-id="9b23d-122">可以使用 _sortBy_ 属性控制遵循 **viewType** Facet 的应用中项的排序顺序。</span><span class="sxs-lookup"><span data-stu-id="9b23d-122">You can use the _sortBy_ property to control the sort order of the items in applications that respect the **viewType** facet.</span></span>

### <a name="sortby-values"></a><span data-ttu-id="9b23d-123">sortBy 值</span><span class="sxs-lookup"><span data-stu-id="9b23d-123">sortBy values</span></span>

<span data-ttu-id="9b23d-124">以下值是针对 **sortBy** 属性进行定义。</span><span class="sxs-lookup"><span data-stu-id="9b23d-124">The following values are defined for the **sortBy** property.</span></span>

| <span data-ttu-id="9b23d-125">值</span><span class="sxs-lookup"><span data-stu-id="9b23d-125">Value</span></span>                    | <span data-ttu-id="9b23d-126">说明</span><span class="sxs-lookup"><span data-stu-id="9b23d-126">Description</span></span>
| ------------------------ | --------------------------------------------------
| `default`                | <span data-ttu-id="9b23d-127">应用的默认排序顺序。</span><span class="sxs-lookup"><span data-stu-id="9b23d-127">The default sort order of the application.</span></span>
| `name`                   | <span data-ttu-id="9b23d-128">应按项的 **name** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="9b23d-128">Items should be arranged by the **name** property of the items.</span></span>
| `type`                   | <span data-ttu-id="9b23d-129">应按项类型排列项。</span><span class="sxs-lookup"><span data-stu-id="9b23d-129">Items should be arranged by the type of item.</span></span>
| `size`                   | <span data-ttu-id="9b23d-130">应按项的 **size** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="9b23d-130">Items should be arranged by the **size** property of the items.</span></span>
| `takenOrCreatedDateTime` | <span data-ttu-id="9b23d-131">应按 **Photo** Facet 的 **takenDateTime** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="9b23d-131">Items should be arranged by the **takenDateTime** property of the **photo** facet.</span></span> <span data-ttu-id="9b23d-132">如果此属性不可用，应按 **createdDateTime** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="9b23d-132">If not available, the **createdDateTime** property should be used.</span></span>
| `lastModifiedDateTime`   | <span data-ttu-id="9b23d-133">应按项的 **lastModifiedDateTime** 属性排列项。</span><span class="sxs-lookup"><span data-stu-id="9b23d-133">Items should be arranged by the **lastModifiedDateTime** property of the items.</span></span>
| `sequence`               | <span data-ttu-id="9b23d-134">这些项按照用户指定的自定义序列排列。</span><span class="sxs-lookup"><span data-stu-id="9b23d-134">Items follow a custom sequence specified by the user.</span></span>


### <a name="sortorder-values"></a><span data-ttu-id="9b23d-135">sortOrder 值</span><span class="sxs-lookup"><span data-stu-id="9b23d-135">sortOrder values</span></span>

<span data-ttu-id="9b23d-136">以下值是针对 **sortOrder** 属性进行定义。</span><span class="sxs-lookup"><span data-stu-id="9b23d-136">The following values are defined for the **sortOrder** property.</span></span>

| <span data-ttu-id="9b23d-137">值</span><span class="sxs-lookup"><span data-stu-id="9b23d-137">Value</span></span>        | <span data-ttu-id="9b23d-138">说明</span><span class="sxs-lookup"><span data-stu-id="9b23d-138">Description</span></span>
| ------------ | --------------------------------------------------------------
| `ascending`  | <span data-ttu-id="9b23d-139">应按升序排列项。</span><span class="sxs-lookup"><span data-stu-id="9b23d-139">Items should be arranged in ascending order.</span></span>
| `descending` | <span data-ttu-id="9b23d-140">应按降序排列项。</span><span class="sxs-lookup"><span data-stu-id="9b23d-140">Items should be arranged in descending order.</span></span>


### <a name="viewtype-values"></a><span data-ttu-id="9b23d-141">viewType 值</span><span class="sxs-lookup"><span data-stu-id="9b23d-141">viewType values</span></span>

<span data-ttu-id="9b23d-142">以下值是针对 **viewType** 属性进行定义。</span><span class="sxs-lookup"><span data-stu-id="9b23d-142">The following values are defined for the **viewType** property.</span></span>

| <span data-ttu-id="9b23d-143">值</span><span class="sxs-lookup"><span data-stu-id="9b23d-143">Value</span></span>        | <span data-ttu-id="9b23d-144">说明</span><span class="sxs-lookup"><span data-stu-id="9b23d-144">Description</span></span>
| ------------ | --------------------------------------------------------------
| `default`    | <span data-ttu-id="9b23d-145">应用的默认视图类型。</span><span class="sxs-lookup"><span data-stu-id="9b23d-145">The default view type for the application.</span></span>
| `icons`      | <span data-ttu-id="9b23d-146">使用图标表示 driveItem 的视图。</span><span class="sxs-lookup"><span data-stu-id="9b23d-146">A view that uses icons to represent driveItems.</span></span>
| `details`    | <span data-ttu-id="9b23d-147">使用多个列提供每一项的其他详细信息的视图。</span><span class="sxs-lookup"><span data-stu-id="9b23d-147">A view with multiple columns that provide additional details about each item.</span></span>
| `thumbnails` | <span data-ttu-id="9b23d-148">使用 driveItem 的大缩略图表示项的视图。</span><span class="sxs-lookup"><span data-stu-id="9b23d-148">A view that uses larger thumbnails of driveItems to represent the items.</span></span>


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
