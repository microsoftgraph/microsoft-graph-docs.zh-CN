---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。 未来将弃用此复杂类型。
localization_priority: Normal
ms.openlocfilehash: 31e5501c504b8813f8910a8b8b352a1fa0ce9478
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348348"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="52b43-104">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="52b43-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="52b43-105">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="52b43-105">For internal use only.</span></span> <span data-ttu-id="52b43-106">未来将弃用此复杂类型。</span><span class="sxs-lookup"><span data-stu-id="52b43-106">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="52b43-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52b43-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="52b43-108">属性</span><span class="sxs-lookup"><span data-stu-id="52b43-108">Properties</span></span>
| <span data-ttu-id="52b43-109">属性</span><span class="sxs-lookup"><span data-stu-id="52b43-109">Property</span></span>         | <span data-ttu-id="52b43-110">类型</span><span class="sxs-lookup"><span data-stu-id="52b43-110">Type</span></span>       | <span data-ttu-id="52b43-111">说明</span><span class="sxs-lookup"><span data-stu-id="52b43-111">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="52b43-112">类型</span><span class="sxs-lookup"><span data-stu-id="52b43-112">type</span></span>             | <span data-ttu-id="52b43-113">Int32</span><span class="sxs-lookup"><span data-stu-id="52b43-113">Int32</span></span>      | <span data-ttu-id="52b43-114">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="52b43-114">For internal use only</span></span>
| <span data-ttu-id="52b43-115">identityProvider</span><span class="sxs-lookup"><span data-stu-id="52b43-115">identityProvider</span></span> | <span data-ttu-id="52b43-116">string</span><span class="sxs-lookup"><span data-stu-id="52b43-116">string</span></span>     | <span data-ttu-id="52b43-117">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="52b43-117">For internal use only</span></span>
| <span data-ttu-id="52b43-118">注册表项</span><span class="sxs-lookup"><span data-stu-id="52b43-118">key</span></span>              | <span data-ttu-id="52b43-119">Edm</span><span class="sxs-lookup"><span data-stu-id="52b43-119">Edm.Binary</span></span> | <span data-ttu-id="52b43-120">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="52b43-120">For internal use only</span></span>
