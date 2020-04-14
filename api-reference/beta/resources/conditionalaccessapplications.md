---
title: conditionalAccessApplications 资源类型
description: 表示策略作用域中包含和排除的应用程序和用户操作。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6484ec54b5e39ad2e6b189cc70c05fd666b81297
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413514"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="159ac-103">conditionalAccessApplications 资源类型</span><span class="sxs-lookup"><span data-stu-id="159ac-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="159ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="159ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="159ac-105">表示策略中包含和排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="159ac-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="159ac-106">属性</span><span class="sxs-lookup"><span data-stu-id="159ac-106">Properties</span></span>

| <span data-ttu-id="159ac-107">属性</span><span class="sxs-lookup"><span data-stu-id="159ac-107">Property</span></span> | <span data-ttu-id="159ac-108">类型</span><span class="sxs-lookup"><span data-stu-id="159ac-108">Type</span></span> | <span data-ttu-id="159ac-109">说明</span><span class="sxs-lookup"><span data-stu-id="159ac-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="159ac-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="159ac-110">includeApplications</span></span> | <span data-ttu-id="159ac-111">String 集合</span><span class="sxs-lookup"><span data-stu-id="159ac-111">String collection</span></span> | <span data-ttu-id="159ac-112">策略应用于的应用程序 Id 列表，除非明确排除（在 excludeApplications 中）。</span><span class="sxs-lookup"><span data-stu-id="159ac-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="159ac-113">也可以将设置为`All`。</span><span class="sxs-lookup"><span data-stu-id="159ac-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="159ac-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="159ac-114">excludeApplications</span></span> | <span data-ttu-id="159ac-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="159ac-115">String collection</span></span> | <span data-ttu-id="159ac-116">从策略中显式排除的应用程序 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="159ac-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="159ac-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="159ac-117">includeUserActions</span></span> | <span data-ttu-id="159ac-118">String 集合</span><span class="sxs-lookup"><span data-stu-id="159ac-118">String collection</span></span> | <span data-ttu-id="159ac-119">要包括的用户操作（例如`urn:user:registersecurityinfo`）</span><span class="sxs-lookup"><span data-stu-id="159ac-119">User actions to include (e.g. `urn:user:registersecurityinfo`)</span></span> |

## <a name="relationships"></a><span data-ttu-id="159ac-120">关系</span><span class="sxs-lookup"><span data-stu-id="159ac-120">Relationships</span></span>

<span data-ttu-id="159ac-121">无。</span><span class="sxs-lookup"><span data-stu-id="159ac-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="159ac-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="159ac-122">JSON representation</span></span>

<span data-ttu-id="159ac-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="159ac-123">The following is a JSON representation of the resource.</span></span>

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