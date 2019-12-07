---
title: openShiftItem 资源类型
description: 表示打开的班次的单个计数。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 86392d330403acf667f81c1dce4bbc951bb8185d
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895624"
---
# <a name="openshiftitem-resource-type"></a><span data-ttu-id="dd2c0-103">openShiftItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd2c0-103">openShiftItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd2c0-104">表示[openshift](../resources/openshift.md)的单个计数。</span><span class="sxs-lookup"><span data-stu-id="dd2c0-104">Represents a single count of an [openshift](../resources/openshift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dd2c0-105">属性</span><span class="sxs-lookup"><span data-stu-id="dd2c0-105">Properties</span></span>

| <span data-ttu-id="dd2c0-106">属性</span><span class="sxs-lookup"><span data-stu-id="dd2c0-106">Property</span></span>     | <span data-ttu-id="dd2c0-107">类型</span><span class="sxs-lookup"><span data-stu-id="dd2c0-107">Type</span></span>        | <span data-ttu-id="dd2c0-108">说明</span><span class="sxs-lookup"><span data-stu-id="dd2c0-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd2c0-109">openSlotCount</span><span class="sxs-lookup"><span data-stu-id="dd2c0-109">openSlotCount</span></span>|<span data-ttu-id="dd2c0-110">Int32</span><span class="sxs-lookup"><span data-stu-id="dd2c0-110">Int32</span></span>| <span data-ttu-id="dd2c0-111">给定的打开班次的槽数的计数。</span><span class="sxs-lookup"><span data-stu-id="dd2c0-111">Count of the number of slots for the given open shift.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd2c0-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd2c0-112">JSON representation</span></span>

<span data-ttu-id="dd2c0-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd2c0-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftItem",
  "baseType": "microsoft.graph.shiftItem"
}-->

```json
{
  "openSlotCount": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
