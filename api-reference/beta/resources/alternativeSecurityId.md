---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。 未来将弃用此复杂类型。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: spunukol
ms.openlocfilehash: 9aa6802dcf077ffd78ae29a73d45a4046d35cb71
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807547"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="f02bf-104">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="f02bf-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="f02bf-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f02bf-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f02bf-106">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="f02bf-106">For internal use only.</span></span> <span data-ttu-id="f02bf-107">未来将弃用此复杂类型。</span><span class="sxs-lookup"><span data-stu-id="f02bf-107">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f02bf-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f02bf-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f02bf-109">属性</span><span class="sxs-lookup"><span data-stu-id="f02bf-109">Properties</span></span>
| <span data-ttu-id="f02bf-110">属性</span><span class="sxs-lookup"><span data-stu-id="f02bf-110">Property</span></span>         | <span data-ttu-id="f02bf-111">类型</span><span class="sxs-lookup"><span data-stu-id="f02bf-111">Type</span></span>       | <span data-ttu-id="f02bf-112">说明</span><span class="sxs-lookup"><span data-stu-id="f02bf-112">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="f02bf-113">类型</span><span class="sxs-lookup"><span data-stu-id="f02bf-113">type</span></span>             | <span data-ttu-id="f02bf-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f02bf-114">Int32</span></span>      | <span data-ttu-id="f02bf-115">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="f02bf-115">For internal use only</span></span>
| <span data-ttu-id="f02bf-116">identityProvider</span><span class="sxs-lookup"><span data-stu-id="f02bf-116">identityProvider</span></span> | <span data-ttu-id="f02bf-117">string</span><span class="sxs-lookup"><span data-stu-id="f02bf-117">string</span></span>     | <span data-ttu-id="f02bf-118">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="f02bf-118">For internal use only</span></span>
| <span data-ttu-id="f02bf-119">注册表项</span><span class="sxs-lookup"><span data-stu-id="f02bf-119">key</span></span>              | <span data-ttu-id="f02bf-120">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="f02bf-120">Edm.Binary</span></span> | <span data-ttu-id="f02bf-121">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="f02bf-121">For internal use only</span></span>
