---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。
ms.openlocfilehash: 9d941469da133d9a3e7149dfca55c813f60b3ce8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007645"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="69680-103">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="69680-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="69680-104">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="69680-104">For internal use only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="69680-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69680-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="69680-106">属性</span><span class="sxs-lookup"><span data-stu-id="69680-106">Properties</span></span>
| <span data-ttu-id="69680-107">属性</span><span class="sxs-lookup"><span data-stu-id="69680-107">Property</span></span>         | <span data-ttu-id="69680-108">类型</span><span class="sxs-lookup"><span data-stu-id="69680-108">Type</span></span>       | <span data-ttu-id="69680-109">说明</span><span class="sxs-lookup"><span data-stu-id="69680-109">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="69680-110">类型</span><span class="sxs-lookup"><span data-stu-id="69680-110">type</span></span>             | <span data-ttu-id="69680-111">Int32</span><span class="sxs-lookup"><span data-stu-id="69680-111">Int32</span></span>      | <span data-ttu-id="69680-112">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="69680-112">For internal use only</span></span>
| <span data-ttu-id="69680-113">identityProvider</span><span class="sxs-lookup"><span data-stu-id="69680-113">identityProvider</span></span> | <span data-ttu-id="69680-114">string</span><span class="sxs-lookup"><span data-stu-id="69680-114">string</span></span>     | <span data-ttu-id="69680-115">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="69680-115">For internal use only</span></span>
| <span data-ttu-id="69680-116">Key</span><span class="sxs-lookup"><span data-stu-id="69680-116">key</span></span>              | <span data-ttu-id="69680-117">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="69680-117">Edm.Binary</span></span> | <span data-ttu-id="69680-118">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="69680-118">For internal use only</span></span>
