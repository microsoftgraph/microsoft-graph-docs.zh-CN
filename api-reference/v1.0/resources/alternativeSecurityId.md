---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。
localization_priority: Normal
author: spunukol
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 33658a93f3a495a13b2300704cb7b677dc380d84
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547630"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="268ee-103">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="268ee-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="268ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="268ee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="268ee-105">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="268ee-105">For internal use only.</span></span> <span data-ttu-id="268ee-106">将来将弃用此复杂类型。</span><span class="sxs-lookup"><span data-stu-id="268ee-106">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="268ee-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="268ee-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="268ee-108">属性</span><span class="sxs-lookup"><span data-stu-id="268ee-108">Properties</span></span>
| <span data-ttu-id="268ee-109">属性</span><span class="sxs-lookup"><span data-stu-id="268ee-109">Property</span></span>         | <span data-ttu-id="268ee-110">类型</span><span class="sxs-lookup"><span data-stu-id="268ee-110">Type</span></span>       | <span data-ttu-id="268ee-111">描述</span><span class="sxs-lookup"><span data-stu-id="268ee-111">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="268ee-112">类型</span><span class="sxs-lookup"><span data-stu-id="268ee-112">type</span></span>             | <span data-ttu-id="268ee-113">Int32</span><span class="sxs-lookup"><span data-stu-id="268ee-113">Int32</span></span>      | <span data-ttu-id="268ee-114">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="268ee-114">For internal use only</span></span>
| <span data-ttu-id="268ee-115">identityProvider</span><span class="sxs-lookup"><span data-stu-id="268ee-115">identityProvider</span></span> | <span data-ttu-id="268ee-116">字符串</span><span class="sxs-lookup"><span data-stu-id="268ee-116">string</span></span>     | <span data-ttu-id="268ee-117">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="268ee-117">For internal use only</span></span>
| <span data-ttu-id="268ee-118">注册表项</span><span class="sxs-lookup"><span data-stu-id="268ee-118">key</span></span>              | <span data-ttu-id="268ee-119">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="268ee-119">Edm.Binary</span></span> | <span data-ttu-id="268ee-120">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="268ee-120">For internal use only</span></span>

