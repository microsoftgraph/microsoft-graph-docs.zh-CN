---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。
localization_priority: Normal
author: spunukol
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 82647c1bcc73444cc70febf53f8bdaf336b84ad4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041692"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="08ea5-103">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="08ea5-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="08ea5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08ea5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08ea5-105">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="08ea5-105">For internal use only.</span></span> <span data-ttu-id="08ea5-106">未来将弃用此复杂类型。</span><span class="sxs-lookup"><span data-stu-id="08ea5-106">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="08ea5-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="08ea5-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="08ea5-108">属性</span><span class="sxs-lookup"><span data-stu-id="08ea5-108">Properties</span></span>
| <span data-ttu-id="08ea5-109">属性</span><span class="sxs-lookup"><span data-stu-id="08ea5-109">Property</span></span>         | <span data-ttu-id="08ea5-110">类型</span><span class="sxs-lookup"><span data-stu-id="08ea5-110">Type</span></span>       | <span data-ttu-id="08ea5-111">说明</span><span class="sxs-lookup"><span data-stu-id="08ea5-111">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="08ea5-112">类型</span><span class="sxs-lookup"><span data-stu-id="08ea5-112">type</span></span>             | <span data-ttu-id="08ea5-113">Int32</span><span class="sxs-lookup"><span data-stu-id="08ea5-113">Int32</span></span>      | <span data-ttu-id="08ea5-114">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="08ea5-114">For internal use only</span></span>
| <span data-ttu-id="08ea5-115">identityProvider</span><span class="sxs-lookup"><span data-stu-id="08ea5-115">identityProvider</span></span> | <span data-ttu-id="08ea5-116">字符串</span><span class="sxs-lookup"><span data-stu-id="08ea5-116">string</span></span>     | <span data-ttu-id="08ea5-117">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="08ea5-117">For internal use only</span></span>
| <span data-ttu-id="08ea5-118">注册表项</span><span class="sxs-lookup"><span data-stu-id="08ea5-118">key</span></span>              | <span data-ttu-id="08ea5-119">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="08ea5-119">Edm.Binary</span></span> | <span data-ttu-id="08ea5-120">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="08ea5-120">For internal use only</span></span>

