---
title: updateWindow 资源类型
description: updateWindow 资源类型。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 7d8f12c7cfcb4c83075087d7b894dc95fe92a695
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761224"
---
# <a name="updatewindow-resource-type"></a><span data-ttu-id="54469-103">updateWindow 资源类型</span><span class="sxs-lookup"><span data-stu-id="54469-103">updateWindow resource type</span></span>

<span data-ttu-id="54469-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54469-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54469-105">表示代理可接收 [更新](onpremisesagent.md) 的时间窗口。</span><span class="sxs-lookup"><span data-stu-id="54469-105">Represents time window during which [agents](onpremisesagent.md) can receive updates.</span></span>

## <a name="properties"></a><span data-ttu-id="54469-106">属性</span><span class="sxs-lookup"><span data-stu-id="54469-106">Properties</span></span>

| <span data-ttu-id="54469-107">属性</span><span class="sxs-lookup"><span data-stu-id="54469-107">Property</span></span>     | <span data-ttu-id="54469-108">类型</span><span class="sxs-lookup"><span data-stu-id="54469-108">Type</span></span>        | <span data-ttu-id="54469-109">说明</span><span class="sxs-lookup"><span data-stu-id="54469-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="54469-110">updateWindowEndTime</span><span class="sxs-lookup"><span data-stu-id="54469-110">updateWindowEndTime</span></span>|<span data-ttu-id="54469-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="54469-111">TimeOfDay</span></span>|<span data-ttu-id="54469-112">代理可以接收更新的时间窗口结束</span><span class="sxs-lookup"><span data-stu-id="54469-112">End of a time window during which agents can receive updates</span></span>|
|<span data-ttu-id="54469-113">updateWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="54469-113">updateWindowStartTime</span></span>|<span data-ttu-id="54469-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="54469-114">TimeOfDay</span></span>|<span data-ttu-id="54469-115">代理可以接收更新的时间窗口的开始时间</span><span class="sxs-lookup"><span data-stu-id="54469-115">Start of a time window during which agents can receive updates</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54469-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54469-116">JSON representation</span></span>

<span data-ttu-id="54469-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54469-117">The following is a JSON representation of the resource.</span></span>

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


