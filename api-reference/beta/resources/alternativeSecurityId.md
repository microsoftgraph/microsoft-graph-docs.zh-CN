---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。
ms.openlocfilehash: 9d941469da133d9a3e7149dfca55c813f60b3ce8
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29579840"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="d31d0-103">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="d31d0-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="d31d0-104">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="d31d0-104">For internal use only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d31d0-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d31d0-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d31d0-106">属性</span><span class="sxs-lookup"><span data-stu-id="d31d0-106">Properties</span></span>
| <span data-ttu-id="d31d0-107">属性</span><span class="sxs-lookup"><span data-stu-id="d31d0-107">Property</span></span>         | <span data-ttu-id="d31d0-108">类型</span><span class="sxs-lookup"><span data-stu-id="d31d0-108">Type</span></span>       | <span data-ttu-id="d31d0-109">说明</span><span class="sxs-lookup"><span data-stu-id="d31d0-109">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="d31d0-110">类型</span><span class="sxs-lookup"><span data-stu-id="d31d0-110">type</span></span>             | <span data-ttu-id="d31d0-111">Int32</span><span class="sxs-lookup"><span data-stu-id="d31d0-111">Int32</span></span>      | <span data-ttu-id="d31d0-112">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="d31d0-112">For internal use only</span></span>
| <span data-ttu-id="d31d0-113">identityProvider</span><span class="sxs-lookup"><span data-stu-id="d31d0-113">identityProvider</span></span> | <span data-ttu-id="d31d0-114">string</span><span class="sxs-lookup"><span data-stu-id="d31d0-114">string</span></span>     | <span data-ttu-id="d31d0-115">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="d31d0-115">For internal use only</span></span>
| <span data-ttu-id="d31d0-116">Key</span><span class="sxs-lookup"><span data-stu-id="d31d0-116">key</span></span>              | <span data-ttu-id="d31d0-117">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="d31d0-117">Edm.Binary</span></span> | <span data-ttu-id="d31d0-118">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="d31d0-118">For internal use only</span></span>
