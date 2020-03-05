---
title: updateWindow 资源类型
description: updateWindow 资源类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d0f509accba2cb73709a4a5fa504a5d2a716b038
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519580"
---
# <a name="updatewindow-resource-type"></a><span data-ttu-id="8fedf-103">updateWindow 资源类型</span><span class="sxs-lookup"><span data-stu-id="8fedf-103">updateWindow resource type</span></span>

<span data-ttu-id="8fedf-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8fedf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fedf-105">表示[代理](onpremisesagent.md)可以接收更新的时间窗口。</span><span class="sxs-lookup"><span data-stu-id="8fedf-105">Represents time window during which [agents](onpremisesagent.md) can receive updates.</span></span>

## <a name="properties"></a><span data-ttu-id="8fedf-106">属性</span><span class="sxs-lookup"><span data-stu-id="8fedf-106">Properties</span></span>

| <span data-ttu-id="8fedf-107">属性</span><span class="sxs-lookup"><span data-stu-id="8fedf-107">Property</span></span>     | <span data-ttu-id="8fedf-108">类型</span><span class="sxs-lookup"><span data-stu-id="8fedf-108">Type</span></span>        | <span data-ttu-id="8fedf-109">说明</span><span class="sxs-lookup"><span data-stu-id="8fedf-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8fedf-110">updateWindowEndTime</span><span class="sxs-lookup"><span data-stu-id="8fedf-110">updateWindowEndTime</span></span>|<span data-ttu-id="8fedf-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8fedf-111">TimeOfDay</span></span>|<span data-ttu-id="8fedf-112">代理可以在其中接收更新的时间窗口结束</span><span class="sxs-lookup"><span data-stu-id="8fedf-112">End of a time window during which agents can receive updates</span></span>|
|<span data-ttu-id="8fedf-113">updateWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="8fedf-113">updateWindowStartTime</span></span>|<span data-ttu-id="8fedf-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8fedf-114">TimeOfDay</span></span>|<span data-ttu-id="8fedf-115">代理可在其中接收更新的时间范围的开始时间</span><span class="sxs-lookup"><span data-stu-id="8fedf-115">Start of a time window during which agents can receive updates</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8fedf-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8fedf-116">JSON representation</span></span>

<span data-ttu-id="8fedf-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fedf-117">The following is a JSON representation of the resource.</span></span>

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
