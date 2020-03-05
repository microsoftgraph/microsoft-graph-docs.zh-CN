---
author: JeremyKelley
ms.author: jeremyke
title: 捆绑资源类型
description: 描述作为其他 Driveitem 的逻辑分组的 driveItem 的 Facet
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ae03674970c8861c7d1c158e62662d9691e74789
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507864"
---
# <a name="bundle-resource-type"></a><span data-ttu-id="88837-103">捆绑资源类型</span><span class="sxs-lookup"><span data-stu-id="88837-103">bundle resource type</span></span>

<span data-ttu-id="88837-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="88837-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88837-105">捆绑包是一次用于一次性共享多个文件的文件的逻辑分组。</span><span class="sxs-lookup"><span data-stu-id="88837-105">A bundle is a logical grouping of files used to share multiple files at once.</span></span> <span data-ttu-id="88837-106">它由包含`bundle` Facet 的[driveItem][]实体表示，并且可以像其他任何其他 driveItem 一样进行共享。</span><span class="sxs-lookup"><span data-stu-id="88837-106">It is represented by a [driveItem][] entity containing a `bundle` facet and can be shared in the same way as any other driveItem.</span></span>

<span data-ttu-id="88837-107">DriveItem `bundle`上的 facet [][]将项目标识为捆绑包，并将捆绑包中的信息分组到一个单一结构中。</span><span class="sxs-lookup"><span data-stu-id="88837-107">The `bundle` facet on a [driveItem][] identifies an item as a bundle and groups bundle-specific information into a single structure.</span></span> <span data-ttu-id="88837-108">它仅包含在从**捆绑包**终结点返回的[driveItem][]资源中。</span><span class="sxs-lookup"><span data-stu-id="88837-108">It is only included on [driveItem][] resources returned from the **bundles** endpoint.</span></span>

<span data-ttu-id="88837-109">请注意， `bundle`资源类型本身并不是自己的实体，并且只是[driveItem][]上的一个 facet。</span><span class="sxs-lookup"><span data-stu-id="88837-109">Note that the `bundle` resource type itself is not an entity of its own, and is only a facet on a [driveItem][].</span></span> <span data-ttu-id="88837-110">驱动器`bundles`上的集合[][]的类型为[driveItem][]，而不`bundle`是。</span><span class="sxs-lookup"><span data-stu-id="88837-110">The `bundles` collection on a [drive][] is of type [driveItem][], not `bundle`.</span></span>

## <a name="methods"></a><span data-ttu-id="88837-111">方法</span><span class="sxs-lookup"><span data-stu-id="88837-111">Methods</span></span>

|                        <span data-ttu-id="88837-112">方法</span><span class="sxs-lookup"><span data-stu-id="88837-112">Method</span></span>             |         <span data-ttu-id="88837-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="88837-113">Return type</span></span>      | <span data-ttu-id="88837-114">说明</span><span class="sxs-lookup"><span data-stu-id="88837-114">Description</span></span>        |
| :---------------------------------------- | :----------------------- | :------------------|
| <span data-ttu-id="88837-115">[列出捆绑包][bundle-list]</span><span class="sxs-lookup"><span data-stu-id="88837-115">[List bundles][bundle-list]</span></span>               | <span data-ttu-id="88837-116">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="88837-116">[driveItem][] collection</span></span> | <span data-ttu-id="88837-117">列出驱动器中的所有捆绑包</span><span class="sxs-lookup"><span data-stu-id="88837-117">List all bundles in a drive</span></span> |
| <span data-ttu-id="88837-118">[获取捆绑包][bundle-get]</span><span class="sxs-lookup"><span data-stu-id="88837-118">[Get bundle][bundle-get]</span></span>                  | <span data-ttu-id="88837-119">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="88837-119">[driveItem][]</span></span>            | <span data-ttu-id="88837-120">获取捆绑包元数据</span><span class="sxs-lookup"><span data-stu-id="88837-120">Get bundle metadata</span></span> |
| <span data-ttu-id="88837-121">[创建捆绑包][bundle-create]</span><span class="sxs-lookup"><span data-stu-id="88837-121">[Create bundle][bundle-create]</span></span>            | <span data-ttu-id="88837-122">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="88837-122">[driveItem][]</span></span>            | <span data-ttu-id="88837-123">创建新的捆绑包</span><span class="sxs-lookup"><span data-stu-id="88837-123">Create a new bundle</span></span> |
| <span data-ttu-id="88837-124">[添加项目][bundle-add-item]</span><span class="sxs-lookup"><span data-stu-id="88837-124">[Add item][bundle-add-item]</span></span>               | <span data-ttu-id="88837-125">无</span><span class="sxs-lookup"><span data-stu-id="88837-125">None</span></span>                     | <span data-ttu-id="88837-126">将[driveItem][]添加到现有捆绑包</span><span class="sxs-lookup"><span data-stu-id="88837-126">Add a [driveItem][] to an existing bundle</span></span> |
| <span data-ttu-id="88837-127">[删除项][bundle-remove-item]</span><span class="sxs-lookup"><span data-stu-id="88837-127">[Remove item][bundle-remove-item]</span></span>         | <span data-ttu-id="88837-128">无</span><span class="sxs-lookup"><span data-stu-id="88837-128">None</span></span>                     | <span data-ttu-id="88837-129">从现有捆绑包中删除[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="88837-129">Remove a [driveItem][] from an existing bundle</span></span> |
| <span data-ttu-id="88837-130">[更新捆绑包][bundle-update]</span><span class="sxs-lookup"><span data-stu-id="88837-130">[Update bundle][bundle-update]</span></span>            | <span data-ttu-id="88837-131">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="88837-131">[driveItem][]</span></span>            | <span data-ttu-id="88837-132">更新捆绑包元数据</span><span class="sxs-lookup"><span data-stu-id="88837-132">Update bundle metadata</span></span> |
| <span data-ttu-id="88837-133">[删除捆绑包][bundle-delete]</span><span class="sxs-lookup"><span data-stu-id="88837-133">[Delete bundle][bundle-delete]</span></span>            | <span data-ttu-id="88837-134">无</span><span class="sxs-lookup"><span data-stu-id="88837-134">None</span></span>                     | <span data-ttu-id="88837-135">删除捆绑包</span><span class="sxs-lookup"><span data-stu-id="88837-135">Delete bundle</span></span> |


## <a name="properties"></a><span data-ttu-id="88837-136">属性</span><span class="sxs-lookup"><span data-stu-id="88837-136">Properties</span></span>

| <span data-ttu-id="88837-137">属性名称</span><span class="sxs-lookup"><span data-stu-id="88837-137">Property name</span></span> | <span data-ttu-id="88837-138">类型</span><span class="sxs-lookup"><span data-stu-id="88837-138">Type</span></span>      | <span data-ttu-id="88837-139">说明</span><span class="sxs-lookup"><span data-stu-id="88837-139">Description</span></span>
|:--------------|:----------|:------------------------------------------------
| <span data-ttu-id="88837-140">childCount</span><span class="sxs-lookup"><span data-stu-id="88837-140">childCount</span></span>    | <span data-ttu-id="88837-141">Int32</span><span class="sxs-lookup"><span data-stu-id="88837-141">Int32</span></span>     | <span data-ttu-id="88837-142">此容器包含的直接子项数量。</span><span class="sxs-lookup"><span data-stu-id="88837-142">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="88837-143">album</span><span class="sxs-lookup"><span data-stu-id="88837-143">album</span></span>         | <span data-ttu-id="88837-144">[album][]</span><span class="sxs-lookup"><span data-stu-id="88837-144">[album][]</span></span> | <span data-ttu-id="88837-145">如果捆绑包是[唱片集][]，则会`album`将该属性包含</span><span class="sxs-lookup"><span data-stu-id="88837-145">If the bundle is an [album][], then the `album` property is included</span></span>

## <a name="json-representation"></a><span data-ttu-id="88837-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88837-146">JSON representation</span></span>

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
