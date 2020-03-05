---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。 未来将弃用此复杂类型。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4e3dfae11009000fa89eccb7c0263867fe2a1562
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508329"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="b2a65-104">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2a65-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="b2a65-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b2a65-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2a65-106">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="b2a65-106">For internal use only.</span></span> <span data-ttu-id="b2a65-107">未来将弃用此复杂类型。</span><span class="sxs-lookup"><span data-stu-id="b2a65-107">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2a65-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2a65-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b2a65-109">属性</span><span class="sxs-lookup"><span data-stu-id="b2a65-109">Properties</span></span>
| <span data-ttu-id="b2a65-110">属性</span><span class="sxs-lookup"><span data-stu-id="b2a65-110">Property</span></span>         | <span data-ttu-id="b2a65-111">类型</span><span class="sxs-lookup"><span data-stu-id="b2a65-111">Type</span></span>       | <span data-ttu-id="b2a65-112">说明</span><span class="sxs-lookup"><span data-stu-id="b2a65-112">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="b2a65-113">类型</span><span class="sxs-lookup"><span data-stu-id="b2a65-113">type</span></span>             | <span data-ttu-id="b2a65-114">Int32</span><span class="sxs-lookup"><span data-stu-id="b2a65-114">Int32</span></span>      | <span data-ttu-id="b2a65-115">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="b2a65-115">For internal use only</span></span>
| <span data-ttu-id="b2a65-116">identityProvider</span><span class="sxs-lookup"><span data-stu-id="b2a65-116">identityProvider</span></span> | <span data-ttu-id="b2a65-117">string</span><span class="sxs-lookup"><span data-stu-id="b2a65-117">string</span></span>     | <span data-ttu-id="b2a65-118">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="b2a65-118">For internal use only</span></span>
| <span data-ttu-id="b2a65-119">注册表项</span><span class="sxs-lookup"><span data-stu-id="b2a65-119">key</span></span>              | <span data-ttu-id="b2a65-120">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="b2a65-120">Edm.Binary</span></span> | <span data-ttu-id="b2a65-121">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="b2a65-121">For internal use only</span></span>
