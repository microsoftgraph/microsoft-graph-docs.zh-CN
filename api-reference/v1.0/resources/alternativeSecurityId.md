---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d4cdfa609e5cc2daf484bf0f35b863285ee811dd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033241"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="014d4-103">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="014d4-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="014d4-104">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="014d4-104">For internal use only.</span></span> <span data-ttu-id="014d4-105">未来将弃用此复杂类型。</span><span class="sxs-lookup"><span data-stu-id="014d4-105">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="014d4-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="014d4-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="014d4-107">属性</span><span class="sxs-lookup"><span data-stu-id="014d4-107">Properties</span></span>
| <span data-ttu-id="014d4-108">属性</span><span class="sxs-lookup"><span data-stu-id="014d4-108">Property</span></span>         | <span data-ttu-id="014d4-109">类型</span><span class="sxs-lookup"><span data-stu-id="014d4-109">Type</span></span>       | <span data-ttu-id="014d4-110">说明</span><span class="sxs-lookup"><span data-stu-id="014d4-110">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="014d4-111">类型</span><span class="sxs-lookup"><span data-stu-id="014d4-111">type</span></span>             | <span data-ttu-id="014d4-112">Int32</span><span class="sxs-lookup"><span data-stu-id="014d4-112">Int32</span></span>      | <span data-ttu-id="014d4-113">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="014d4-113">For internal use only</span></span>
| <span data-ttu-id="014d4-114">identityProvider</span><span class="sxs-lookup"><span data-stu-id="014d4-114">identityProvider</span></span> | <span data-ttu-id="014d4-115">string</span><span class="sxs-lookup"><span data-stu-id="014d4-115">string</span></span>     | <span data-ttu-id="014d4-116">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="014d4-116">For internal use only</span></span>
| <span data-ttu-id="014d4-117">注册表项</span><span class="sxs-lookup"><span data-stu-id="014d4-117">key</span></span>              | <span data-ttu-id="014d4-118">Edm</span><span class="sxs-lookup"><span data-stu-id="014d4-118">Edm.Binary</span></span> | <span data-ttu-id="014d4-119">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="014d4-119">For internal use only</span></span>
