---
title: updateWindow 资源类型
description: updateWindow 资源类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 57fb977dd853261300ed09dd8d9b3c343f62bea0
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840952"
---
# <a name="updatewindow-resource-type"></a><span data-ttu-id="4443e-103">updateWindow 资源类型</span><span class="sxs-lookup"><span data-stu-id="4443e-103">updateWindow resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4443e-104">表示[代理](onpremisesagent.md)可以接收更新的时间窗口。</span><span class="sxs-lookup"><span data-stu-id="4443e-104">Represents time window during which [agents](onpremisesagent.md) can receive updates.</span></span>

## <a name="properties"></a><span data-ttu-id="4443e-105">属性</span><span class="sxs-lookup"><span data-stu-id="4443e-105">Properties</span></span>

| <span data-ttu-id="4443e-106">属性</span><span class="sxs-lookup"><span data-stu-id="4443e-106">Property</span></span>     | <span data-ttu-id="4443e-107">类型</span><span class="sxs-lookup"><span data-stu-id="4443e-107">Type</span></span>        | <span data-ttu-id="4443e-108">说明</span><span class="sxs-lookup"><span data-stu-id="4443e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4443e-109">updateWindowEndTime</span><span class="sxs-lookup"><span data-stu-id="4443e-109">updateWindowEndTime</span></span>|<span data-ttu-id="4443e-110">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4443e-110">TimeOfDay</span></span>|<span data-ttu-id="4443e-111">代理可以在其中接收更新的时间窗口结束</span><span class="sxs-lookup"><span data-stu-id="4443e-111">End of a time window during which agents can receive updates</span></span>|
|<span data-ttu-id="4443e-112">updateWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="4443e-112">updateWindowStartTime</span></span>|<span data-ttu-id="4443e-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4443e-113">TimeOfDay</span></span>|<span data-ttu-id="4443e-114">代理可在其中接收更新的时间范围的开始时间</span><span class="sxs-lookup"><span data-stu-id="4443e-114">Start of a time window during which agents can receive updates</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4443e-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4443e-115">JSON representation</span></span>

<span data-ttu-id="4443e-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4443e-116">The following is a JSON representation of the resource.</span></span>

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
