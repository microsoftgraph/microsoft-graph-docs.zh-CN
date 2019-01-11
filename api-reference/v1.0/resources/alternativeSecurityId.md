---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。
localization_priority: Normal
ms.openlocfilehash: 23ef74085a4a3cc383f0854e9139c9a0b63e3d40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853800"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="f1d7f-103">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1d7f-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="f1d7f-104">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="f1d7f-104">For internal use only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1d7f-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1d7f-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f1d7f-106">属性</span><span class="sxs-lookup"><span data-stu-id="f1d7f-106">Properties</span></span>
| <span data-ttu-id="f1d7f-107">属性</span><span class="sxs-lookup"><span data-stu-id="f1d7f-107">Property</span></span>         | <span data-ttu-id="f1d7f-108">类型</span><span class="sxs-lookup"><span data-stu-id="f1d7f-108">Type</span></span>       | <span data-ttu-id="f1d7f-109">说明</span><span class="sxs-lookup"><span data-stu-id="f1d7f-109">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="f1d7f-110">类型</span><span class="sxs-lookup"><span data-stu-id="f1d7f-110">type</span></span>             | <span data-ttu-id="f1d7f-111">Int32</span><span class="sxs-lookup"><span data-stu-id="f1d7f-111">Int32</span></span>      | <span data-ttu-id="f1d7f-112">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="f1d7f-112">For internal use only</span></span>
| <span data-ttu-id="f1d7f-113">identityProvider</span><span class="sxs-lookup"><span data-stu-id="f1d7f-113">identityProvider</span></span> | <span data-ttu-id="f1d7f-114">string</span><span class="sxs-lookup"><span data-stu-id="f1d7f-114">string</span></span>     | <span data-ttu-id="f1d7f-115">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="f1d7f-115">For internal use only</span></span>
| <span data-ttu-id="f1d7f-116">Key</span><span class="sxs-lookup"><span data-stu-id="f1d7f-116">key</span></span>              | <span data-ttu-id="f1d7f-117">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="f1d7f-117">Edm.Binary</span></span> | <span data-ttu-id="f1d7f-118">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="f1d7f-118">For internal use only</span></span>
