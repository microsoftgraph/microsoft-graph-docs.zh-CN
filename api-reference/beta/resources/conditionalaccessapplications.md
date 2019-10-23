---
title: conditionalAccessApplications 资源类型
description: 表示策略作用域中包含和排除的应用程序和用户操作。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e163d8f958a400c9c478b0aca865bdfa077c8d60
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638587"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="46d89-103">conditionalAccessApplications 资源类型</span><span class="sxs-lookup"><span data-stu-id="46d89-103">conditionalAccessApplications resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46d89-104">表示策略中包含和排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="46d89-104">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="46d89-105">属性</span><span class="sxs-lookup"><span data-stu-id="46d89-105">Properties</span></span>

| <span data-ttu-id="46d89-106">属性</span><span class="sxs-lookup"><span data-stu-id="46d89-106">Property</span></span> | <span data-ttu-id="46d89-107">类型</span><span class="sxs-lookup"><span data-stu-id="46d89-107">Type</span></span> | <span data-ttu-id="46d89-108">说明</span><span class="sxs-lookup"><span data-stu-id="46d89-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="46d89-109">includeApplications</span><span class="sxs-lookup"><span data-stu-id="46d89-109">includeApplications</span></span> | <span data-ttu-id="46d89-110">String collection</span><span class="sxs-lookup"><span data-stu-id="46d89-110">String collection</span></span> | <span data-ttu-id="46d89-111">策略应用于的应用程序 Id 列表，除非明确排除（在 excludeApplications 中）。</span><span class="sxs-lookup"><span data-stu-id="46d89-111">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="46d89-112">也可以将设置为`All`。</span><span class="sxs-lookup"><span data-stu-id="46d89-112">Can also be set to `All`.</span></span> |
| <span data-ttu-id="46d89-113">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="46d89-113">excludeApplications</span></span> | <span data-ttu-id="46d89-114">String collection</span><span class="sxs-lookup"><span data-stu-id="46d89-114">String collection</span></span> | <span data-ttu-id="46d89-115">从策略中显式排除的应用程序 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="46d89-115">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="46d89-116">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="46d89-116">includeUserActions</span></span> | <span data-ttu-id="46d89-117">String collection</span><span class="sxs-lookup"><span data-stu-id="46d89-117">String collection</span></span> | <span data-ttu-id="46d89-118">要包括的用户操作（例如`urn:user:registersecurityinfo`）</span><span class="sxs-lookup"><span data-stu-id="46d89-118">User actions to include (e.g. `urn:user:registersecurityinfo`)</span></span> |

## <a name="relationships"></a><span data-ttu-id="46d89-119">关系</span><span class="sxs-lookup"><span data-stu-id="46d89-119">Relationships</span></span>

<span data-ttu-id="46d89-120">无。</span><span class="sxs-lookup"><span data-stu-id="46d89-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="46d89-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="46d89-121">JSON representation</span></span>

<span data-ttu-id="46d89-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46d89-122">The following is a JSON representation of the resource.</span></span>

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