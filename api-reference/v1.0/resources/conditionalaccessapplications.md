---
title: conditionalAccessApplications 资源类型
description: 表示策略作用域中包含和排除的应用程序和用户操作。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8b09a3531d3734aed67e9ff91fee1d917f76054b
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384472"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="83698-103">conditionalAccessApplications 资源类型</span><span class="sxs-lookup"><span data-stu-id="83698-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="83698-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83698-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="83698-105">表示策略中包含和排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="83698-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="83698-106">属性</span><span class="sxs-lookup"><span data-stu-id="83698-106">Properties</span></span>

| <span data-ttu-id="83698-107">属性</span><span class="sxs-lookup"><span data-stu-id="83698-107">Property</span></span>     | <span data-ttu-id="83698-108">类型</span><span class="sxs-lookup"><span data-stu-id="83698-108">Type</span></span>        | <span data-ttu-id="83698-109">说明</span><span class="sxs-lookup"><span data-stu-id="83698-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="83698-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="83698-110">includeApplications</span></span> | <span data-ttu-id="83698-111">String collection</span><span class="sxs-lookup"><span data-stu-id="83698-111">String collection</span></span> | <span data-ttu-id="83698-112">策略应用于的应用程序 Id 列表，除非明确排除（在 excludeApplications 中）。</span><span class="sxs-lookup"><span data-stu-id="83698-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="83698-113">也可以将设置为 `All` 。</span><span class="sxs-lookup"><span data-stu-id="83698-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="83698-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="83698-114">excludeApplications</span></span> | <span data-ttu-id="83698-115">String collection</span><span class="sxs-lookup"><span data-stu-id="83698-115">String collection</span></span> | <span data-ttu-id="83698-116">从策略中显式排除的应用程序 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="83698-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="83698-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="83698-117">includeUserActions</span></span> | <span data-ttu-id="83698-118">String collection</span><span class="sxs-lookup"><span data-stu-id="83698-118">String collection</span></span> | <span data-ttu-id="83698-119">要包括的用户操作。</span><span class="sxs-lookup"><span data-stu-id="83698-119">User actions to include.</span></span> <span data-ttu-id="83698-120">例如，`urn:user:registersecurityinfo`</span><span class="sxs-lookup"><span data-stu-id="83698-120">For example, `urn:user:registersecurityinfo`</span></span> |

## <a name="relationships"></a><span data-ttu-id="83698-121">关系</span><span class="sxs-lookup"><span data-stu-id="83698-121">Relationships</span></span>

<span data-ttu-id="83698-122">无。</span><span class="sxs-lookup"><span data-stu-id="83698-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="83698-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83698-123">JSON representation</span></span>

<span data-ttu-id="83698-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83698-124">The following is a JSON representation of the resource.</span></span>

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
