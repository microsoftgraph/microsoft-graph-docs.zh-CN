---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。 将来将弃用此复杂类型。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: spunukol
ms.openlocfilehash: 3e696c824e2229ea26cacccee11c93a24d03fa97
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547553"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="57909-104">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="57909-104">alternativeSecurityId resource type</span></span>

<span data-ttu-id="57909-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57909-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57909-106">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="57909-106">For internal use only.</span></span> <span data-ttu-id="57909-107">将来将弃用此复杂类型。</span><span class="sxs-lookup"><span data-stu-id="57909-107">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="57909-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57909-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="57909-109">属性</span><span class="sxs-lookup"><span data-stu-id="57909-109">Properties</span></span>
| <span data-ttu-id="57909-110">属性</span><span class="sxs-lookup"><span data-stu-id="57909-110">Property</span></span>         | <span data-ttu-id="57909-111">类型</span><span class="sxs-lookup"><span data-stu-id="57909-111">Type</span></span>       | <span data-ttu-id="57909-112">说明</span><span class="sxs-lookup"><span data-stu-id="57909-112">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="57909-113">类型</span><span class="sxs-lookup"><span data-stu-id="57909-113">type</span></span>             | <span data-ttu-id="57909-114">Int32</span><span class="sxs-lookup"><span data-stu-id="57909-114">Int32</span></span>      | <span data-ttu-id="57909-115">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="57909-115">For internal use only</span></span>
| <span data-ttu-id="57909-116">identityProvider</span><span class="sxs-lookup"><span data-stu-id="57909-116">identityProvider</span></span> | <span data-ttu-id="57909-117">string</span><span class="sxs-lookup"><span data-stu-id="57909-117">string</span></span>     | <span data-ttu-id="57909-118">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="57909-118">For internal use only</span></span>
| <span data-ttu-id="57909-119">注册表项</span><span class="sxs-lookup"><span data-stu-id="57909-119">key</span></span>              | <span data-ttu-id="57909-120">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="57909-120">Edm.Binary</span></span> | <span data-ttu-id="57909-121">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="57909-121">For internal use only</span></span>


