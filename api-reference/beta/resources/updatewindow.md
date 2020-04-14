---
title: updateWindow 资源类型
description: updateWindow 资源类型。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a85cef3d3d87ac3b0c4f3bedcb291d6e6c03a054
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401656"
---
# <a name="updatewindow-resource-type"></a><span data-ttu-id="84837-103">updateWindow 资源类型</span><span class="sxs-lookup"><span data-stu-id="84837-103">updateWindow resource type</span></span>

<span data-ttu-id="84837-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84837-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84837-105">表示[代理](onpremisesagent.md)可以接收更新的时间窗口。</span><span class="sxs-lookup"><span data-stu-id="84837-105">Represents time window during which [agents](onpremisesagent.md) can receive updates.</span></span>

## <a name="properties"></a><span data-ttu-id="84837-106">属性</span><span class="sxs-lookup"><span data-stu-id="84837-106">Properties</span></span>

| <span data-ttu-id="84837-107">属性</span><span class="sxs-lookup"><span data-stu-id="84837-107">Property</span></span>     | <span data-ttu-id="84837-108">类型</span><span class="sxs-lookup"><span data-stu-id="84837-108">Type</span></span>        | <span data-ttu-id="84837-109">说明</span><span class="sxs-lookup"><span data-stu-id="84837-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="84837-110">updateWindowEndTime</span><span class="sxs-lookup"><span data-stu-id="84837-110">updateWindowEndTime</span></span>|<span data-ttu-id="84837-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="84837-111">TimeOfDay</span></span>|<span data-ttu-id="84837-112">代理可以在其中接收更新的时间窗口结束</span><span class="sxs-lookup"><span data-stu-id="84837-112">End of a time window during which agents can receive updates</span></span>|
|<span data-ttu-id="84837-113">updateWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="84837-113">updateWindowStartTime</span></span>|<span data-ttu-id="84837-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="84837-114">TimeOfDay</span></span>|<span data-ttu-id="84837-115">代理可在其中接收更新的时间范围的开始时间</span><span class="sxs-lookup"><span data-stu-id="84837-115">Start of a time window during which agents can receive updates</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84837-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84837-116">JSON representation</span></span>

<span data-ttu-id="84837-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84837-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.updateWindow",
  "baseType": null
}-->

```json
{
  "updateWindowEndTime": "String (timestamp)",
  "updateWindowStartTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "updateWindow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
