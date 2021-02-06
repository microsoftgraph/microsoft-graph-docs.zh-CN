---
title: conditionalAccessApplications 资源类型
description: 表示包含在策略作用域中和从策略作用域中排除的应用程序和用户操作。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0a787a1c22209b502e4eed68790629e2e6e1b03b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137396"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="0e295-103">conditionalAccessApplications 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e295-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="0e295-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e295-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e295-105">表示包含在策略中和从策略中排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="0e295-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="0e295-106">属性</span><span class="sxs-lookup"><span data-stu-id="0e295-106">Properties</span></span>

| <span data-ttu-id="0e295-107">属性</span><span class="sxs-lookup"><span data-stu-id="0e295-107">Property</span></span> | <span data-ttu-id="0e295-108">类型</span><span class="sxs-lookup"><span data-stu-id="0e295-108">Type</span></span> | <span data-ttu-id="0e295-109">说明</span><span class="sxs-lookup"><span data-stu-id="0e295-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="0e295-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="0e295-110">includeApplications</span></span> | <span data-ttu-id="0e295-111">字符串集合</span><span class="sxs-lookup"><span data-stu-id="0e295-111">String collection</span></span> | <span data-ttu-id="0e295-112">除非在 excludeApplications (中明确) 。</span><span class="sxs-lookup"><span data-stu-id="0e295-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="0e295-113">也可以设置为 `All` 。</span><span class="sxs-lookup"><span data-stu-id="0e295-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="0e295-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="0e295-114">excludeApplications</span></span> | <span data-ttu-id="0e295-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="0e295-115">String collection</span></span> | <span data-ttu-id="0e295-116">从策略中明确排除的应用程序 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="0e295-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="0e295-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="0e295-117">includeUserActions</span></span> | <span data-ttu-id="0e295-118">字符串集合</span><span class="sxs-lookup"><span data-stu-id="0e295-118">String collection</span></span> | <span data-ttu-id="0e295-119">要包含的用户操作。</span><span class="sxs-lookup"><span data-stu-id="0e295-119">User actions to include.</span></span> <span data-ttu-id="0e295-120">支持的值 `urn:user:registersecurityinfo` 包括 `urn:user:registerdevice`</span><span class="sxs-lookup"><span data-stu-id="0e295-120">Supported values are `urn:user:registersecurityinfo` and `urn:user:registerdevice`</span></span> |

## <a name="relationships"></a><span data-ttu-id="0e295-121">关系</span><span class="sxs-lookup"><span data-stu-id="0e295-121">Relationships</span></span>

<span data-ttu-id="0e295-122">无。</span><span class="sxs-lookup"><span data-stu-id="0e295-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e295-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e295-123">JSON representation</span></span>

<span data-ttu-id="0e295-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e295-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeApplications",
    "excludeApplications",
    "includeUserActions"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessApplications"
}-->

```json
{
  "includeApplications": ["String"],
  "excludeApplications": ["String"],
  "includeUserActions": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessApplications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

