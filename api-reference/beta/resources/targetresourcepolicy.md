---
title: targetResourcePolicy 资源类型
description: '指示已受影响的审核活动的策略。 派生 targetResource 资源。   '
localization_priority: Normal
ms.openlocfilehash: 355e6ac11741a2aa7aeb780bdac4b7be373092af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813137"
---
# <a name="targetresourcepolicy-resource-type"></a><span data-ttu-id="30d87-104">targetResourcePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="30d87-104">targetResourcePolicy resource type</span></span>
<span data-ttu-id="30d87-105">指示已受影响的审核活动的策略。</span><span class="sxs-lookup"><span data-stu-id="30d87-105">Indicates the policy that was impacted by the audit activity.</span></span> <span data-ttu-id="30d87-106">派生[targetResource](targetresource.md)资源。</span><span class="sxs-lookup"><span data-stu-id="30d87-106">Derived from the [targetResource](targetresource.md) resource.</span></span>   



## <a name="properties"></a><span data-ttu-id="30d87-107">属性</span><span class="sxs-lookup"><span data-stu-id="30d87-107">Properties</span></span>
| <span data-ttu-id="30d87-108">属性</span><span class="sxs-lookup"><span data-stu-id="30d87-108">Property</span></span>     | <span data-ttu-id="30d87-109">类型</span><span class="sxs-lookup"><span data-stu-id="30d87-109">Type</span></span>   |<span data-ttu-id="30d87-110">Description</span><span class="sxs-lookup"><span data-stu-id="30d87-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30d87-111">policyType</span><span class="sxs-lookup"><span data-stu-id="30d87-111">policyType</span></span>|<span data-ttu-id="30d87-112">字符串</span><span class="sxs-lookup"><span data-stu-id="30d87-112">String</span></span>|<span data-ttu-id="30d87-113">指示已更改或已更改的设定的策略名称</span><span class="sxs-lookup"><span data-stu-id="30d87-113">Indicates the Policy Name that changed or was targetted for change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30d87-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30d87-114">JSON representation</span></span>

<span data-ttu-id="30d87-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30d87-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourcePolicy"
}-->

```json
{
  "policyType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourcePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
