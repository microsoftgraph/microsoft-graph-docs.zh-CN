---
title: conditionalAccessDeviceStates 资源类型
description: 表示策略作用域中的设备状态。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 822f819cd8e9ef0f93279c67b94972a1e9fb7929
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638580"
---
# <a name="conditionalaccessdevicestates-resource-type"></a><span data-ttu-id="16327-103">conditionalAccessDeviceStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="16327-103">conditionalAccessDeviceStates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16327-104">表示策略作用域中的设备状态。</span><span class="sxs-lookup"><span data-stu-id="16327-104">Represents device states in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="16327-105">属性</span><span class="sxs-lookup"><span data-stu-id="16327-105">Properties</span></span>

| <span data-ttu-id="16327-106">属性</span><span class="sxs-lookup"><span data-stu-id="16327-106">Property</span></span>     | <span data-ttu-id="16327-107">类型</span><span class="sxs-lookup"><span data-stu-id="16327-107">Type</span></span>        | <span data-ttu-id="16327-108">说明</span><span class="sxs-lookup"><span data-stu-id="16327-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="16327-109">includeStates</span><span class="sxs-lookup"><span data-stu-id="16327-109">includeStates</span></span> | <span data-ttu-id="16327-110">String collection</span><span class="sxs-lookup"><span data-stu-id="16327-110">String collection</span></span> | <span data-ttu-id="16327-111">策略作用域中的状态。</span><span class="sxs-lookup"><span data-stu-id="16327-111">States in the scope of the policy.</span></span> <span data-ttu-id="16327-112">`All`是唯一允许的值。</span><span class="sxs-lookup"><span data-stu-id="16327-112">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="16327-113">excludeStates</span><span class="sxs-lookup"><span data-stu-id="16327-113">excludeStates</span></span> | <span data-ttu-id="16327-114">String collection</span><span class="sxs-lookup"><span data-stu-id="16327-114">String collection</span></span> | <span data-ttu-id="16327-115">策略作用域中排除的状态。</span><span class="sxs-lookup"><span data-stu-id="16327-115">States excluded from the scope of the policy.</span></span> <span data-ttu-id="16327-116">可能的值`Compliant`： `DomainJoined`、。</span><span class="sxs-lookup"><span data-stu-id="16327-116">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="16327-117">关系</span><span class="sxs-lookup"><span data-stu-id="16327-117">Relationships</span></span>

<span data-ttu-id="16327-118">无。</span><span class="sxs-lookup"><span data-stu-id="16327-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="16327-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16327-119">JSON representation</span></span>

<span data-ttu-id="16327-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16327-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeStates",
    "excludeStates"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDeviceStates",
  "baseType": null
}-->

```json
{
  "includeStates": [ "String" ],
  "excludeStates": [ "String" ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessDeviceStates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->