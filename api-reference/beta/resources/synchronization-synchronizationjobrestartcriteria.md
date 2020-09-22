---
title: synchronizationJobRestartCriteria 资源类型
description: 定义 synchronizationJob： restart 操作的范围。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 82d671f411725a1e6537580205c7298cf887e3a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023840"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="c84f4-103">synchronizationJobRestartCriteria 资源类型</span><span class="sxs-lookup"><span data-stu-id="c84f4-103">synchronizationJobRestartCriteria resource type</span></span>

<span data-ttu-id="c84f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c84f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c84f4-105">定义 [synchronizationJob： restart](../api/synchronization-synchronizationjob-restart.md) 操作的范围。</span><span class="sxs-lookup"><span data-stu-id="c84f4-105">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="c84f4-106">属性</span><span class="sxs-lookup"><span data-stu-id="c84f4-106">Properties</span></span>
| <span data-ttu-id="c84f4-107">属性</span><span class="sxs-lookup"><span data-stu-id="c84f4-107">Property</span></span>     | <span data-ttu-id="c84f4-108">类型</span><span class="sxs-lookup"><span data-stu-id="c84f4-108">Type</span></span>   |<span data-ttu-id="c84f4-109">说明</span><span class="sxs-lookup"><span data-stu-id="c84f4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c84f4-110">resetScope</span><span class="sxs-lookup"><span data-stu-id="c84f4-110">resetScope</span></span>|<span data-ttu-id="c84f4-111">String</span><span class="sxs-lookup"><span data-stu-id="c84f4-111">String</span></span>| <span data-ttu-id="c84f4-112">以下值的逗号分隔组合：、、 `Full` 、 `QuarantineState` `Watermark` `Escrows` `ConnectorDataStore` 。</span><span class="sxs-lookup"><span data-stu-id="c84f4-112">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="c84f4-113">`Full`如果您想要所有选项，请使用。</span><span class="sxs-lookup"><span data-stu-id="c84f4-113">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c84f4-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c84f4-114">JSON representation</span></span>

<span data-ttu-id="c84f4-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c84f4-115">The following is a JSON representation of the resource.</span></span>

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


