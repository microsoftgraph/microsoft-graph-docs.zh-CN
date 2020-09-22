---
title: openShiftItem 资源类型
description: 表示打开的班次的单个计数。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3945300e340e91d8ace82fb07ba3fc3aea2dd444
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998528"
---
# <a name="openshiftitem-resource-type"></a><span data-ttu-id="cbaec-103">openShiftItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="cbaec-103">openShiftItem resource type</span></span>

<span data-ttu-id="cbaec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbaec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbaec-105">表示 [openshift](../resources/openshift.md)的单个计数。</span><span class="sxs-lookup"><span data-stu-id="cbaec-105">Represents a single count of an [openshift](../resources/openshift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cbaec-106">属性</span><span class="sxs-lookup"><span data-stu-id="cbaec-106">Properties</span></span>

| <span data-ttu-id="cbaec-107">属性</span><span class="sxs-lookup"><span data-stu-id="cbaec-107">Property</span></span>     | <span data-ttu-id="cbaec-108">类型</span><span class="sxs-lookup"><span data-stu-id="cbaec-108">Type</span></span>        | <span data-ttu-id="cbaec-109">说明</span><span class="sxs-lookup"><span data-stu-id="cbaec-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cbaec-110">openSlotCount</span><span class="sxs-lookup"><span data-stu-id="cbaec-110">openSlotCount</span></span>|<span data-ttu-id="cbaec-111">Int32</span><span class="sxs-lookup"><span data-stu-id="cbaec-111">Int32</span></span>| <span data-ttu-id="cbaec-112">给定的打开班次的槽数的计数。</span><span class="sxs-lookup"><span data-stu-id="cbaec-112">Count of the number of slots for the given open shift.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cbaec-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cbaec-113">JSON representation</span></span>

<span data-ttu-id="cbaec-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbaec-114">The following is a JSON representation of the resource.</span></span>

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


