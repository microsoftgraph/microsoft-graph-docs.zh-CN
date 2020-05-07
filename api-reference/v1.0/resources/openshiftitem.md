---
title: openShiftItem 资源类型
description: 表示打开的班次的单个计数。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2fb690d06a2ca20fe8c4c50d41a06bc2d247ef1f
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154975"
---
# <a name="openshiftitem-resource-type"></a><span data-ttu-id="9468f-103">openShiftItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="9468f-103">openShiftItem resource type</span></span>

<span data-ttu-id="9468f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9468f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9468f-105">表示[openShift](../resources/openshift.md)的单个计数。</span><span class="sxs-lookup"><span data-stu-id="9468f-105">Represents a single count of an [openShift](../resources/openshift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9468f-106">属性</span><span class="sxs-lookup"><span data-stu-id="9468f-106">Properties</span></span>

| <span data-ttu-id="9468f-107">属性</span><span class="sxs-lookup"><span data-stu-id="9468f-107">Property</span></span>     | <span data-ttu-id="9468f-108">类型</span><span class="sxs-lookup"><span data-stu-id="9468f-108">Type</span></span>        | <span data-ttu-id="9468f-109">Description</span><span class="sxs-lookup"><span data-stu-id="9468f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9468f-110">openSlotCount</span><span class="sxs-lookup"><span data-stu-id="9468f-110">openSlotCount</span></span>|<span data-ttu-id="9468f-111">Int32</span><span class="sxs-lookup"><span data-stu-id="9468f-111">Int32</span></span>| <span data-ttu-id="9468f-112">给定的打开班次的槽数的计数。</span><span class="sxs-lookup"><span data-stu-id="9468f-112">Count of the number of slots for the given open shift.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9468f-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9468f-113">JSON representation</span></span>

<span data-ttu-id="9468f-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9468f-114">The following is a JSON representation of the resource.</span></span>

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
