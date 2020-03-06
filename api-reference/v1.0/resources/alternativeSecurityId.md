---
title: alternativeSecurityId 资源类型
description: 仅供内部使用。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d86d5f07a957abe45b898be08744c7c93853d78e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533155"
---
# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="29c74-103">alternativeSecurityId 资源类型</span><span class="sxs-lookup"><span data-stu-id="29c74-103">alternativeSecurityId resource type</span></span>

<span data-ttu-id="29c74-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29c74-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="29c74-105">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="29c74-105">For internal use only.</span></span> <span data-ttu-id="29c74-106">未来将弃用此复杂类型。</span><span class="sxs-lookup"><span data-stu-id="29c74-106">This complex type will be deprecated in the future.</span></span>

## <a name="json-representation"></a><span data-ttu-id="29c74-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29c74-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="29c74-108">属性</span><span class="sxs-lookup"><span data-stu-id="29c74-108">Properties</span></span>
| <span data-ttu-id="29c74-109">属性</span><span class="sxs-lookup"><span data-stu-id="29c74-109">Property</span></span>         | <span data-ttu-id="29c74-110">类型</span><span class="sxs-lookup"><span data-stu-id="29c74-110">Type</span></span>       | <span data-ttu-id="29c74-111">说明</span><span class="sxs-lookup"><span data-stu-id="29c74-111">Description</span></span>
|:-----------------|:-----------|:---------------------
| <span data-ttu-id="29c74-112">类型</span><span class="sxs-lookup"><span data-stu-id="29c74-112">type</span></span>             | <span data-ttu-id="29c74-113">Int32</span><span class="sxs-lookup"><span data-stu-id="29c74-113">Int32</span></span>      | <span data-ttu-id="29c74-114">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="29c74-114">For internal use only</span></span>
| <span data-ttu-id="29c74-115">identityProvider</span><span class="sxs-lookup"><span data-stu-id="29c74-115">identityProvider</span></span> | <span data-ttu-id="29c74-116">字符串</span><span class="sxs-lookup"><span data-stu-id="29c74-116">string</span></span>     | <span data-ttu-id="29c74-117">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="29c74-117">For internal use only</span></span>
| <span data-ttu-id="29c74-118">注册表项</span><span class="sxs-lookup"><span data-stu-id="29c74-118">key</span></span>              | <span data-ttu-id="29c74-119">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="29c74-119">Edm.Binary</span></span> | <span data-ttu-id="29c74-120">仅供内部使用</span><span class="sxs-lookup"><span data-stu-id="29c74-120">For internal use only</span></span>
