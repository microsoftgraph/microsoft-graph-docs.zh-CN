---
author: JeremyKelley
ms.author: jeremyke
title: 捆绑资源类型
description: 描述作为其他 Driveitem 的逻辑分组的 driveItem 的 Facet
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f843afa112f95e391761d0c8804600018a67534c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974085"
---
# <a name="bundle-resource-type"></a><span data-ttu-id="a13ef-103">捆绑资源类型</span><span class="sxs-lookup"><span data-stu-id="a13ef-103">bundle resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a13ef-104">捆绑包是一次用于一次性共享多个文件的文件的逻辑分组。</span><span class="sxs-lookup"><span data-stu-id="a13ef-104">A bundle is a logical grouping of files used to share multiple files at once.</span></span> <span data-ttu-id="a13ef-105">它由包含`bundle` Facet 的[driveItem][]实体表示, 并且可以像其他任何其他 driveItem 一样进行共享。</span><span class="sxs-lookup"><span data-stu-id="a13ef-105">It is represented by a [driveItem][] entity containing a `bundle` facet and can be shared in the same way as any other driveItem.</span></span>

<span data-ttu-id="a13ef-106">DriveItem `bundle`上的 facet [][]将项目标识为捆绑包, 并将捆绑包中的信息分组到一个单一结构中。</span><span class="sxs-lookup"><span data-stu-id="a13ef-106">The `bundle` facet on a [driveItem][] identifies an item as a bundle and groups bundle-specific information into a single structure.</span></span> <span data-ttu-id="a13ef-107">它仅包含在从**捆绑包**终结点返回的[driveItem][]资源中。</span><span class="sxs-lookup"><span data-stu-id="a13ef-107">It is only included on [driveItem][] resources returned from the **bundles** endpoint.</span></span>

<span data-ttu-id="a13ef-108">请注意, `bundle`资源类型本身并不是自己的实体, 并且只是[driveItem][]上的一个 facet。</span><span class="sxs-lookup"><span data-stu-id="a13ef-108">Note that the `bundle` resource type itself is not an entity of its own, and is only a facet on a [driveItem][].</span></span> <span data-ttu-id="a13ef-109">驱动器`bundles`上的集合[][]的类型为[driveItem][], 而不`bundle`是。</span><span class="sxs-lookup"><span data-stu-id="a13ef-109">The `bundles` collection on a [drive][] is of type [driveItem][], not `bundle`.</span></span>

## <a name="methods"></a><span data-ttu-id="a13ef-110">方法</span><span class="sxs-lookup"><span data-stu-id="a13ef-110">Methods</span></span>

|                        <span data-ttu-id="a13ef-111">方法</span><span class="sxs-lookup"><span data-stu-id="a13ef-111">Method</span></span>             |         <span data-ttu-id="a13ef-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="a13ef-112">Return type</span></span>      | <span data-ttu-id="a13ef-113">说明</span><span class="sxs-lookup"><span data-stu-id="a13ef-113">Description</span></span>        |
| :---------------------------------------- | :----------------------- | :------------------|
| <span data-ttu-id="a13ef-114">[列出捆绑包][bundle-list]</span><span class="sxs-lookup"><span data-stu-id="a13ef-114">[List bundles][bundle-list]</span></span>               | <span data-ttu-id="a13ef-115">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="a13ef-115">[driveItem][] collection</span></span> | <span data-ttu-id="a13ef-116">列出驱动器中的所有捆绑包</span><span class="sxs-lookup"><span data-stu-id="a13ef-116">List all bundles in a drive</span></span> |
| <span data-ttu-id="a13ef-117">[获取捆绑包][bundle-get]</span><span class="sxs-lookup"><span data-stu-id="a13ef-117">[Get bundle][bundle-get]</span></span>                  | <span data-ttu-id="a13ef-118">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="a13ef-118">[driveItem][]</span></span>            | <span data-ttu-id="a13ef-119">获取捆绑包元数据</span><span class="sxs-lookup"><span data-stu-id="a13ef-119">Get bundle metadata</span></span> |
| <span data-ttu-id="a13ef-120">[创建捆绑包][bundle-create]</span><span class="sxs-lookup"><span data-stu-id="a13ef-120">[Create bundle][bundle-create]</span></span>            | <span data-ttu-id="a13ef-121">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="a13ef-121">[driveItem][]</span></span>            | <span data-ttu-id="a13ef-122">创建新的捆绑包</span><span class="sxs-lookup"><span data-stu-id="a13ef-122">Create a new bundle</span></span> |
| <span data-ttu-id="a13ef-123">[添加项目][bundle-add-item]</span><span class="sxs-lookup"><span data-stu-id="a13ef-123">[Add item][bundle-add-item]</span></span>               | <span data-ttu-id="a13ef-124">无</span><span class="sxs-lookup"><span data-stu-id="a13ef-124">None</span></span>                     | <span data-ttu-id="a13ef-125">将[driveItem][]添加到现有捆绑包</span><span class="sxs-lookup"><span data-stu-id="a13ef-125">Add a [driveItem][] to an existing bundle</span></span> |
| <span data-ttu-id="a13ef-126">[删除项][bundle-remove-item]</span><span class="sxs-lookup"><span data-stu-id="a13ef-126">[Remove item][bundle-remove-item]</span></span>         | <span data-ttu-id="a13ef-127">无</span><span class="sxs-lookup"><span data-stu-id="a13ef-127">None</span></span>                     | <span data-ttu-id="a13ef-128">从现有捆绑包中删除[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="a13ef-128">Remove a [driveItem][] from an existing bundle</span></span> |
| <span data-ttu-id="a13ef-129">[更新捆绑包][bundle-update]</span><span class="sxs-lookup"><span data-stu-id="a13ef-129">[Update bundle][bundle-update]</span></span>            | <span data-ttu-id="a13ef-130">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="a13ef-130">[driveItem][]</span></span>            | <span data-ttu-id="a13ef-131">更新捆绑包元数据</span><span class="sxs-lookup"><span data-stu-id="a13ef-131">Update bundle metadata</span></span> |
| <span data-ttu-id="a13ef-132">[删除捆绑包][bundle-delete]</span><span class="sxs-lookup"><span data-stu-id="a13ef-132">[Delete bundle][bundle-delete]</span></span>            | <span data-ttu-id="a13ef-133">无</span><span class="sxs-lookup"><span data-stu-id="a13ef-133">None</span></span>                     | <span data-ttu-id="a13ef-134">删除捆绑包</span><span class="sxs-lookup"><span data-stu-id="a13ef-134">Delete bundle</span></span> |


## <a name="properties"></a><span data-ttu-id="a13ef-135">属性</span><span class="sxs-lookup"><span data-stu-id="a13ef-135">Properties</span></span>

| <span data-ttu-id="a13ef-136">属性名称</span><span class="sxs-lookup"><span data-stu-id="a13ef-136">Property name</span></span> | <span data-ttu-id="a13ef-137">类型</span><span class="sxs-lookup"><span data-stu-id="a13ef-137">Type</span></span>      | <span data-ttu-id="a13ef-138">说明</span><span class="sxs-lookup"><span data-stu-id="a13ef-138">Description</span></span>
|:--------------|:----------|:------------------------------------------------
| <span data-ttu-id="a13ef-139">childCount</span><span class="sxs-lookup"><span data-stu-id="a13ef-139">childCount</span></span>    | <span data-ttu-id="a13ef-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a13ef-140">Int32</span></span>     | <span data-ttu-id="a13ef-141">此容器包含的直接子项数量。</span><span class="sxs-lookup"><span data-stu-id="a13ef-141">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="a13ef-142">album</span><span class="sxs-lookup"><span data-stu-id="a13ef-142">album</span></span>         | <span data-ttu-id="a13ef-143">[album][]</span><span class="sxs-lookup"><span data-stu-id="a13ef-143">[album][]</span></span> | <span data-ttu-id="a13ef-144">如果捆绑包是[唱片集][], 则会`album`将该属性包含</span><span class="sxs-lookup"><span data-stu-id="a13ef-144">If the bundle is an [album][], then the `album` property is included</span></span>

## <a name="json-representation"></a><span data-ttu-id="a13ef-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a13ef-145">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.bundle" } -->
```json
{
  "childCount": 3,
  "album": { "@odata.type": "microsoft.graph.album" },
}
```

[album]: album.md
[drive]: drive.md
[driveItem]: driveItem.md

[bundle-list]: ../api/bundle-list.md
[bundle-get]: ../api/bundle-get.md
[bundle-create]: ../api/drive-post-bundles.md
[bundle-add-item]: ../api/bundle-addItem.md
[bundle-remove-item]: ../api/bundle-removeItem.md
[bundle-update]: ../api/bundle-update.md
[bundle-delete]: ../api/bundle-delete.md
