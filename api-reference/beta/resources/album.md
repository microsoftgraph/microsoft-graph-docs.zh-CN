---
author: JeremyKelley
ms.author: jeremyke
title: 唱集资源类型
description: 描述属于相册的捆绑包的 Facet。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 59717995870cbfe970fd23b160377d32cb722835
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974449"
---
# <a name="album-resource-type"></a><span data-ttu-id="15171-103">唱集资源类型</span><span class="sxs-lookup"><span data-stu-id="15171-103">album resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15171-104">相册是在[捆绑包][]中将[driveitem][driveItem]与[照片][]facet 组合在一起的一种方式。</span><span class="sxs-lookup"><span data-stu-id="15171-104">A photo album is a way to virtually group [driveItems][driveItem] with [photo][] facets together in a [bundle][].</span></span> <span data-ttu-id="15171-105">此类型的捆绑包将在[捆绑][]资源上设置**唱集**属性。</span><span class="sxs-lookup"><span data-stu-id="15171-105">Bundles of this type will have the **album** property set on the [bundle][] resource.</span></span>

## <a name="properties"></a><span data-ttu-id="15171-106">属性</span><span class="sxs-lookup"><span data-stu-id="15171-106">Properties</span></span>

| <span data-ttu-id="15171-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="15171-107">Property name</span></span>     | <span data-ttu-id="15171-108">类型</span><span class="sxs-lookup"><span data-stu-id="15171-108">Type</span></span>   | <span data-ttu-id="15171-109">说明</span><span class="sxs-lookup"><span data-stu-id="15171-109">Description</span></span>
|:------------------|:-------|:------------------------------------------------
| <span data-ttu-id="15171-110">coverImageItemId</span><span class="sxs-lookup"><span data-stu-id="15171-110">coverImageItemId</span></span> | <span data-ttu-id="15171-111">String</span><span class="sxs-lookup"><span data-stu-id="15171-111">String</span></span> | <span data-ttu-id="15171-112">[DriveItem][]的唯一标识符, 它是唱片集的封面。</span><span class="sxs-lookup"><span data-stu-id="15171-112">Unique identifier of the [driveItem][] that is the cover of the album.</span></span>

<span data-ttu-id="15171-113">**注意:** 如果尚未设置**coverImageItemId** , 则会自动选择影集的缩略图。</span><span class="sxs-lookup"><span data-stu-id="15171-113">**Note:** If a **coverImageItemId** has not been set before, the thumbnails for an album are chosen automatically.</span></span>
<span data-ttu-id="15171-114">设置**coverImageItemId**后, 影集的缩略图将始终为与该 id 关联的项目。您可以通过修补[捆绑包项目][捆绑]并将**coverImageItemId**属性设置`album`为包含在影集中的图像的 id 来覆盖默认封面。</span><span class="sxs-lookup"><span data-stu-id="15171-114">After **coverImageItemId** has been set, the thumbnails for an album will always be the item associated with that id. You can override the default cover by PATCHing the [bundle item][bundle] and setting the **coverImageItemId** property on the `album` to the id of an image contained within the album.</span></span>
<span data-ttu-id="15171-115">若要删除自定义设置的封面, 可以将**coverImageItemId**属性设置为 null, 并再次自动选择默认属性。</span><span class="sxs-lookup"><span data-stu-id="15171-115">To remove a custom-set cover, you can set the **coverImageItemId** property to null, and a default one will be chosen automatically again.</span></span>

## <a name="json-representation"></a><span data-ttu-id="15171-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15171-116">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.album" } -->

```json
{
  "coverImageItemId": "string"
}
```

[bundle]: bundle.md
[driveItem]: driveItem.md
[photo]: photo.md
