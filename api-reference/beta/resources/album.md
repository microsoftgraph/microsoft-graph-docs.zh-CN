---
author: JeremyKelley
ms.author: jeremyke
title: 唱集资源类型
description: 描述属于相册的捆绑包的 Facet。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b17a910a488e1fb5f051b4acc02d788a21d530d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067410"
---
# <a name="album-resource-type"></a><span data-ttu-id="1c451-103">唱集资源类型</span><span class="sxs-lookup"><span data-stu-id="1c451-103">album resource type</span></span>

<span data-ttu-id="1c451-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c451-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c451-105">相册是在[捆绑包][]中将[driveitem][driveItem]与[照片][]facet 组合在一起的一种方式。</span><span class="sxs-lookup"><span data-stu-id="1c451-105">A photo album is a way to virtually group [driveItems][driveItem] with [photo][] facets together in a [bundle][].</span></span> <span data-ttu-id="1c451-106">此类型的捆绑包将在[捆绑][]资源上设置**唱集**属性。</span><span class="sxs-lookup"><span data-stu-id="1c451-106">Bundles of this type will have the **album** property set on the [bundle][] resource.</span></span>

## <a name="properties"></a><span data-ttu-id="1c451-107">属性</span><span class="sxs-lookup"><span data-stu-id="1c451-107">Properties</span></span>

| <span data-ttu-id="1c451-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="1c451-108">Property name</span></span>     | <span data-ttu-id="1c451-109">类型</span><span class="sxs-lookup"><span data-stu-id="1c451-109">Type</span></span>   | <span data-ttu-id="1c451-110">说明</span><span class="sxs-lookup"><span data-stu-id="1c451-110">Description</span></span>
|:------------------|:-------|:------------------------------------------------
| <span data-ttu-id="1c451-111">coverImageItemId</span><span class="sxs-lookup"><span data-stu-id="1c451-111">coverImageItemId</span></span> | <span data-ttu-id="1c451-112">String</span><span class="sxs-lookup"><span data-stu-id="1c451-112">String</span></span> | <span data-ttu-id="1c451-113">[DriveItem][]的唯一标识符，它是唱片集的封面。</span><span class="sxs-lookup"><span data-stu-id="1c451-113">Unique identifier of the [driveItem][] that is the cover of the album.</span></span>

<span data-ttu-id="1c451-114">**注意：** 如果尚未设置 **coverImageItemId** ，则会自动选择影集的缩略图。</span><span class="sxs-lookup"><span data-stu-id="1c451-114">**Note:** If a **coverImageItemId** has not been set before, the thumbnails for an album are chosen automatically.</span></span>
<span data-ttu-id="1c451-115">设置 **coverImageItemId** 后，影集的缩略图将始终为与该 id 关联的项目。您可以通过修补 [捆绑包项目][捆绑] 并将 **coverImageItemId** 属性设置 `album` 为包含在影集中的图像的 id 来覆盖默认封面。</span><span class="sxs-lookup"><span data-stu-id="1c451-115">After **coverImageItemId** has been set, the thumbnails for an album will always be the item associated with that id. You can override the default cover by PATCHing the [bundle item][bundle] and setting the **coverImageItemId** property on the `album` to the id of an image contained within the album.</span></span>
<span data-ttu-id="1c451-116">若要删除自定义设置的封面，可以将 **coverImageItemId** 属性设置为 null，并再次自动选择默认属性。</span><span class="sxs-lookup"><span data-stu-id="1c451-116">To remove a custom-set cover, you can set the **coverImageItemId** property to null, and a default one will be chosen automatically again.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c451-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c451-117">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.album" } -->

```json
{
  "coverImageItemId": "string"
}
```

[bundle]: bundle.md
[driveItem]: driveItem.md
[photo]: photo.md


