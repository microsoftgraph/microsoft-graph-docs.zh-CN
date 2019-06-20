---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。 未来将弃用此复杂类型。
localization_priority: Normal
ms.openlocfilehash: 31e5501c504b8813f8910a8b8b352a1fa0ce9478
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/20/2019
ms.locfileid: "35083940"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="0ff89-104">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ff89-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="0ff89-105">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="0ff89-105">For internal use only.</span></span> <span data-ttu-id="0ff89-106">未来将弃用此复杂类型。</span><span class="sxs-lookup"><span data-stu-id="0ff89-106">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ff89-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ff89-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0ff89-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ff89-108">Properties</span></span>
| <span data-ttu-id="0ff89-109">属性</span><span class="sxs-lookup"><span data-stu-id="0ff89-109">Property</span></span>         | <span data-ttu-id="0ff89-110">类型</span><span class="sxs-lookup"><span data-stu-id="0ff89-110">Type</span></span>       | <span data-ttu-id="0ff89-111">说明</span><span class="sxs-lookup"><span data-stu-id="0ff89-111">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="0ff89-112">类型</span><span class="sxs-lookup"><span data-stu-id="0ff89-112">type</span></span>             | <span data-ttu-id="0ff89-113">Int32</span><span class="sxs-lookup"><span data-stu-id="0ff89-113">Int32</span></span>      | <span data-ttu-id="0ff89-114">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="0ff89-114">For internal use only</span></span>
| <span data-ttu-id="0ff89-115">identityProvider</span><span class="sxs-lookup"><span data-stu-id="0ff89-115">identityProvider</span></span> | <span data-ttu-id="0ff89-116">string</span><span class="sxs-lookup"><span data-stu-id="0ff89-116">string</span></span>     | <span data-ttu-id="0ff89-117">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="0ff89-117">For internal use only</span></span>
| <span data-ttu-id="0ff89-118">注册表项</span><span class="sxs-lookup"><span data-stu-id="0ff89-118">key</span></span>              | <span data-ttu-id="0ff89-119">Edm</span><span class="sxs-lookup"><span data-stu-id="0ff89-119">Edm.Binary</span></span> | <span data-ttu-id="0ff89-120">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="0ff89-120">For internal use only</span></span>
