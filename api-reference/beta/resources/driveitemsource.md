---
author: MarcMroz
description: driveItemSource 包含有关创建驱动器项的源应用程序的元数据。
title: driveItemSource 资源类型
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: a403f570ac550b62f9c0e7fa0c3c2fa9758e1772
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236293"
---
# <a name="driveitemsource-resource-type"></a><span data-ttu-id="84909-103">driveItemSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="84909-103">driveItemSource resource type</span></span>

<span data-ttu-id="84909-104">包含有关驱动器项源的元数据。</span><span class="sxs-lookup"><span data-stu-id="84909-104">Contains metadata about the source of the drive item.</span></span>

<span data-ttu-id="84909-105">可用于 [driveItem][item-resource] 资源的 source 属性。</span><span class="sxs-lookup"><span data-stu-id="84909-105">It is available on the source property of [driveItem][item-resource] resources.</span></span>

## <a name="properties"></a><span data-ttu-id="84909-106">属性</span><span class="sxs-lookup"><span data-stu-id="84909-106">Properties</span></span>

| <span data-ttu-id="84909-107">属性</span><span class="sxs-lookup"><span data-stu-id="84909-107">Property</span></span>                 | <span data-ttu-id="84909-108">类型</span><span class="sxs-lookup"><span data-stu-id="84909-108">Type</span></span>                       | <span data-ttu-id="84909-109">说明</span><span class="sxs-lookup"><span data-stu-id="84909-109">Description</span></span>                                                                                      |
| :----------------------- | :------------------------  | :----------------------------------------------------------------------------------------------- |
| <span data-ttu-id="84909-110">**application**</span><span class="sxs-lookup"><span data-stu-id="84909-110">**application**</span></span>          | <span data-ttu-id="84909-111">driveItemSourceApplication</span><span class="sxs-lookup"><span data-stu-id="84909-111">driveItemSourceApplication</span></span> | <span data-ttu-id="84909-112">指示创建文件的源应用程序的枚举值。</span><span class="sxs-lookup"><span data-stu-id="84909-112">Enumeration value that indicates the source application where the file was created.</span></span>              |
| <span data-ttu-id="84909-113">**externalId**</span><span class="sxs-lookup"><span data-stu-id="84909-113">**externalId**</span></span>           | <span data-ttu-id="84909-114">字符串</span><span class="sxs-lookup"><span data-stu-id="84909-114">string</span></span>                     | <span data-ttu-id="84909-115">源中的驱动器项的外部标识符。</span><span class="sxs-lookup"><span data-stu-id="84909-115">The external identifier for the drive item from the source.</span></span>                                      |

### <a name="driveitemsourceapplication-values"></a><span data-ttu-id="84909-116">driveItemSourceApplication 值</span><span class="sxs-lookup"><span data-stu-id="84909-116">driveItemSourceApplication values</span></span>

| <span data-ttu-id="84909-117">值</span><span class="sxs-lookup"><span data-stu-id="84909-117">Value</span></span>               | <span data-ttu-id="84909-118">说明</span><span class="sxs-lookup"><span data-stu-id="84909-118">Description</span></span>                                       |
|:--------------------|:--------------------------------------------------|
| <span data-ttu-id="84909-119">teams</span><span class="sxs-lookup"><span data-stu-id="84909-119">teams</span></span>               | <span data-ttu-id="84909-120">应用程序已Teams。</span><span class="sxs-lookup"><span data-stu-id="84909-120">The application is Teams.</span></span>                         |
| <span data-ttu-id="84909-121">yammer</span><span class="sxs-lookup"><span data-stu-id="84909-121">yammer</span></span>              | <span data-ttu-id="84909-122">应用程序已Yammer。</span><span class="sxs-lookup"><span data-stu-id="84909-122">The application is Yammer.</span></span>                        |
| <span data-ttu-id="84909-123">sharePoint</span><span class="sxs-lookup"><span data-stu-id="84909-123">sharePoint</span></span>          | <span data-ttu-id="84909-124">应用程序已SharePoint。</span><span class="sxs-lookup"><span data-stu-id="84909-124">The application is SharePoint.</span></span>                    |
| <span data-ttu-id="84909-125">oneDrive</span><span class="sxs-lookup"><span data-stu-id="84909-125">oneDrive</span></span>            | <span data-ttu-id="84909-126">应用程序已OneDrive。</span><span class="sxs-lookup"><span data-stu-id="84909-126">The application is OneDrive.</span></span>                      |
| <span data-ttu-id="84909-127">stream</span><span class="sxs-lookup"><span data-stu-id="84909-127">stream</span></span>              | <span data-ttu-id="84909-128">应用程序为 Stream。</span><span class="sxs-lookup"><span data-stu-id="84909-128">The application is Stream.</span></span>                        |
| <span data-ttu-id="84909-129">powerPoint</span><span class="sxs-lookup"><span data-stu-id="84909-129">powerPoint</span></span>          | <span data-ttu-id="84909-130">应用程序已PowerPoint</span><span class="sxs-lookup"><span data-stu-id="84909-130">The application is PowerPoint</span></span>                     |
| <span data-ttu-id="84909-131">办公室</span><span class="sxs-lookup"><span data-stu-id="84909-131">office</span></span>              | <span data-ttu-id="84909-132">应用程序已Office</span><span class="sxs-lookup"><span data-stu-id="84909-132">The application is Office</span></span>                         |
| <span data-ttu-id="84909-133">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="84909-133">unknownFutureValue</span></span>  | <span data-ttu-id="84909-134">用于将来兼容性的标记值。</span><span class="sxs-lookup"><span data-stu-id="84909-134">Marker value for future compatibility.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="84909-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84909-135">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "application",
    "externalId",
  ],
  "@odata.type": "microsoft.graph.driveItemSource"
}-->

```json
{
  "application": "string",
  "externalId" : "string"
}
```

## <a name="see-also"></a><span data-ttu-id="84909-136">另请参阅</span><span class="sxs-lookup"><span data-stu-id="84909-136">See also</span></span>

<span data-ttu-id="84909-137">有关 driveItem 上 Facet 的信息，请参阅 [driveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="84909-137">For more information about the facets on a driveItem, see [driveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The driveItemSource facet provides information about drive item source.",
  "keywords": "driveItemSoruce,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/driveItemSource"
} -->
