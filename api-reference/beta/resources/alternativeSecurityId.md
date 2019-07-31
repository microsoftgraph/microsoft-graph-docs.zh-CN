---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。 未来将弃用此复杂类型。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 32930b1e6dc5c4f58232d307dd67780d9b3981e0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974330"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="73b3f-104">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="73b3f-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="73b3f-105">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="73b3f-105">For internal use only.</span></span> <span data-ttu-id="73b3f-106">未来将弃用此复杂类型。</span><span class="sxs-lookup"><span data-stu-id="73b3f-106">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="73b3f-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73b3f-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="73b3f-108">属性</span><span class="sxs-lookup"><span data-stu-id="73b3f-108">Properties</span></span>
| <span data-ttu-id="73b3f-109">属性</span><span class="sxs-lookup"><span data-stu-id="73b3f-109">Property</span></span>         | <span data-ttu-id="73b3f-110">类型</span><span class="sxs-lookup"><span data-stu-id="73b3f-110">Type</span></span>       | <span data-ttu-id="73b3f-111">说明</span><span class="sxs-lookup"><span data-stu-id="73b3f-111">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="73b3f-112">类型</span><span class="sxs-lookup"><span data-stu-id="73b3f-112">type</span></span>             | <span data-ttu-id="73b3f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="73b3f-113">Int32</span></span>      | <span data-ttu-id="73b3f-114">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="73b3f-114">For internal use only</span></span>
| <span data-ttu-id="73b3f-115">identityProvider</span><span class="sxs-lookup"><span data-stu-id="73b3f-115">identityProvider</span></span> | <span data-ttu-id="73b3f-116">string</span><span class="sxs-lookup"><span data-stu-id="73b3f-116">string</span></span>     | <span data-ttu-id="73b3f-117">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="73b3f-117">For internal use only</span></span>
| <span data-ttu-id="73b3f-118">注册表项</span><span class="sxs-lookup"><span data-stu-id="73b3f-118">key</span></span>              | <span data-ttu-id="73b3f-119">Edm</span><span class="sxs-lookup"><span data-stu-id="73b3f-119">Edm.Binary</span></span> | <span data-ttu-id="73b3f-120">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="73b3f-120">For internal use only</span></span>
