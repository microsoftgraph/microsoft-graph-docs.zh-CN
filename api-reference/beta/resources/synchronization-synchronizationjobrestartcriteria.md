---
title: synchronizationJobRestartCriteria 资源类型
description: 定义 synchronizationJob 的作用域：重新启动操作。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: ef15c9322c553d0eedb977c3f01ed5de2823e844
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136498"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="e4181-103">synchronizationJobRestartCriteria 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4181-103">synchronizationJobRestartCriteria resource type</span></span>

<span data-ttu-id="e4181-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4181-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4181-105">定义 [synchronizationJob](../api/synchronization-synchronizationjob-restart.md) 的作用域：重新启动操作。</span><span class="sxs-lookup"><span data-stu-id="e4181-105">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="e4181-106">属性</span><span class="sxs-lookup"><span data-stu-id="e4181-106">Properties</span></span>
| <span data-ttu-id="e4181-107">属性</span><span class="sxs-lookup"><span data-stu-id="e4181-107">Property</span></span>     | <span data-ttu-id="e4181-108">类型</span><span class="sxs-lookup"><span data-stu-id="e4181-108">Type</span></span>   |<span data-ttu-id="e4181-109">说明</span><span class="sxs-lookup"><span data-stu-id="e4181-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4181-110">resetScope</span><span class="sxs-lookup"><span data-stu-id="e4181-110">resetScope</span></span>|<span data-ttu-id="e4181-111">字符串</span><span class="sxs-lookup"><span data-stu-id="e4181-111">String</span></span>| <span data-ttu-id="e4181-112">以逗号分隔的下列值的组合： `Full` ， `QuarantineState` ， ， `Watermark` `Escrows` `ConnectorDataStore` 。</span><span class="sxs-lookup"><span data-stu-id="e4181-112">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="e4181-113">如果需要 `Full` 所有选项，请使用。</span><span class="sxs-lookup"><span data-stu-id="e4181-113">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4181-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4181-114">JSON representation</span></span>

<span data-ttu-id="e4181-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4181-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
    "criteria": {
        "resetScope": "String"
    }
}


```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


