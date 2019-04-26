---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。
localization_priority: Normal
ms.openlocfilehash: 60e45c6d914c64f92b9f15f78fda22372a23e91f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345839"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="94bea-103">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="94bea-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="94bea-104">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="94bea-104">For internal use only.</span></span> <span data-ttu-id="94bea-105">未来将弃用此复杂类型。</span><span class="sxs-lookup"><span data-stu-id="94bea-105">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="94bea-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94bea-106">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "type": 12345,
  "identityProvider": "string",
  "key": {"@odata.type": "Edm.Binary"}
}
```

## <a name="properties"></a><span data-ttu-id="94bea-107">属性</span><span class="sxs-lookup"><span data-stu-id="94bea-107">Properties</span></span>
| <span data-ttu-id="94bea-108">属性</span><span class="sxs-lookup"><span data-stu-id="94bea-108">Property</span></span>         | <span data-ttu-id="94bea-109">类型</span><span class="sxs-lookup"><span data-stu-id="94bea-109">Type</span></span>       | <span data-ttu-id="94bea-110">说明</span><span class="sxs-lookup"><span data-stu-id="94bea-110">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="94bea-111">类型</span><span class="sxs-lookup"><span data-stu-id="94bea-111">type</span></span>             | <span data-ttu-id="94bea-112">Int32</span><span class="sxs-lookup"><span data-stu-id="94bea-112">Int32</span></span>      | <span data-ttu-id="94bea-113">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="94bea-113">For internal use only</span></span>
| <span data-ttu-id="94bea-114">identityProvider</span><span class="sxs-lookup"><span data-stu-id="94bea-114">identityProvider</span></span> | <span data-ttu-id="94bea-115">string</span><span class="sxs-lookup"><span data-stu-id="94bea-115">string</span></span>     | <span data-ttu-id="94bea-116">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="94bea-116">For internal use only</span></span>
| <span data-ttu-id="94bea-117">注册表项</span><span class="sxs-lookup"><span data-stu-id="94bea-117">key</span></span>              | <span data-ttu-id="94bea-118">Edm</span><span class="sxs-lookup"><span data-stu-id="94bea-118">Edm.Binary</span></span> | <span data-ttu-id="94bea-119">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="94bea-119">For internal use only</span></span>
