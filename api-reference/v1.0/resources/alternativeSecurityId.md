---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。
localization_priority: Normal
ms.openlocfilehash: 23ef74085a4a3cc383f0854e9139c9a0b63e3d40
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569478"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="76850-103">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="76850-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="76850-104">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="76850-104">For internal use only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76850-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76850-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="76850-106">属性</span><span class="sxs-lookup"><span data-stu-id="76850-106">Properties</span></span>
| <span data-ttu-id="76850-107">属性</span><span class="sxs-lookup"><span data-stu-id="76850-107">Property</span></span>         | <span data-ttu-id="76850-108">类型</span><span class="sxs-lookup"><span data-stu-id="76850-108">Type</span></span>       | <span data-ttu-id="76850-109">说明</span><span class="sxs-lookup"><span data-stu-id="76850-109">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="76850-110">类型</span><span class="sxs-lookup"><span data-stu-id="76850-110">type</span></span>             | <span data-ttu-id="76850-111">Int32</span><span class="sxs-lookup"><span data-stu-id="76850-111">Int32</span></span>      | <span data-ttu-id="76850-112">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="76850-112">For internal use only</span></span>
| <span data-ttu-id="76850-113">identityProvider</span><span class="sxs-lookup"><span data-stu-id="76850-113">identityProvider</span></span> | <span data-ttu-id="76850-114">string</span><span class="sxs-lookup"><span data-stu-id="76850-114">string</span></span>     | <span data-ttu-id="76850-115">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="76850-115">For internal use only</span></span>
| <span data-ttu-id="76850-116">注册表项</span><span class="sxs-lookup"><span data-stu-id="76850-116">key</span></span>              | <span data-ttu-id="76850-117">Edm</span><span class="sxs-lookup"><span data-stu-id="76850-117">Edm.Binary</span></span> | <span data-ttu-id="76850-118">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="76850-118">For internal use only</span></span>
