---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。 未来将弃用此复杂类型。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: spunukol
ms.openlocfilehash: d08cf247961f4364486f2f9ba5d05508fd900688
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089803"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="de268-104">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="de268-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="de268-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de268-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de268-106">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="de268-106">For internal use only.</span></span> <span data-ttu-id="de268-107">未来将弃用此复杂类型。</span><span class="sxs-lookup"><span data-stu-id="de268-107">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="de268-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de268-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="de268-109">属性</span><span class="sxs-lookup"><span data-stu-id="de268-109">Properties</span></span>
| <span data-ttu-id="de268-110">属性</span><span class="sxs-lookup"><span data-stu-id="de268-110">Property</span></span>         | <span data-ttu-id="de268-111">类型</span><span class="sxs-lookup"><span data-stu-id="de268-111">Type</span></span>       | <span data-ttu-id="de268-112">说明</span><span class="sxs-lookup"><span data-stu-id="de268-112">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="de268-113">类型</span><span class="sxs-lookup"><span data-stu-id="de268-113">type</span></span>             | <span data-ttu-id="de268-114">Int32</span><span class="sxs-lookup"><span data-stu-id="de268-114">Int32</span></span>      | <span data-ttu-id="de268-115">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="de268-115">For internal use only</span></span>
| <span data-ttu-id="de268-116">identityProvider</span><span class="sxs-lookup"><span data-stu-id="de268-116">identityProvider</span></span> | <span data-ttu-id="de268-117">string</span><span class="sxs-lookup"><span data-stu-id="de268-117">string</span></span>     | <span data-ttu-id="de268-118">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="de268-118">For internal use only</span></span>
| <span data-ttu-id="de268-119">注册表项</span><span class="sxs-lookup"><span data-stu-id="de268-119">key</span></span>              | <span data-ttu-id="de268-120">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="de268-120">Edm.Binary</span></span> | <span data-ttu-id="de268-121">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="de268-121">For internal use only</span></span>


