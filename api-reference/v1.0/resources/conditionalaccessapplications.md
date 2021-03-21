---
title: conditionalAccessApplications 资源类型
description: 表示策略作用域中包含和排除的应用程序和用户操作。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3d864acfdd794bc5bcb914c460b29800c4a86291
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962502"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="9ba5e-103">conditionalAccessApplications 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ba5e-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="9ba5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ba5e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9ba5e-105">表示包含在策略中和从策略中排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="9ba5e-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="9ba5e-106">属性</span><span class="sxs-lookup"><span data-stu-id="9ba5e-106">Properties</span></span>

| <span data-ttu-id="9ba5e-107">属性</span><span class="sxs-lookup"><span data-stu-id="9ba5e-107">Property</span></span>     | <span data-ttu-id="9ba5e-108">类型</span><span class="sxs-lookup"><span data-stu-id="9ba5e-108">Type</span></span>        | <span data-ttu-id="9ba5e-109">说明</span><span class="sxs-lookup"><span data-stu-id="9ba5e-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9ba5e-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="9ba5e-110">includeApplications</span></span> | <span data-ttu-id="9ba5e-111">String collection</span><span class="sxs-lookup"><span data-stu-id="9ba5e-111">String collection</span></span> | <span data-ttu-id="9ba5e-112">除非在 excludeApplications (中明确排除策略所适用的应用程序) 。</span><span class="sxs-lookup"><span data-stu-id="9ba5e-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="9ba5e-113">也可以设置为 `All` 。</span><span class="sxs-lookup"><span data-stu-id="9ba5e-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="9ba5e-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="9ba5e-114">excludeApplications</span></span> | <span data-ttu-id="9ba5e-115">String collection</span><span class="sxs-lookup"><span data-stu-id="9ba5e-115">String collection</span></span> | <span data-ttu-id="9ba5e-116">从策略中显式排除的应用程序 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="9ba5e-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="9ba5e-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="9ba5e-117">includeUserActions</span></span> | <span data-ttu-id="9ba5e-118">String collection</span><span class="sxs-lookup"><span data-stu-id="9ba5e-118">String collection</span></span> | <span data-ttu-id="9ba5e-119">要包含的用户操作。</span><span class="sxs-lookup"><span data-stu-id="9ba5e-119">User actions to include.</span></span> <span data-ttu-id="9ba5e-120">支持的值 `urn:user:registersecurityinfo` 包括 和 `urn:user:registerdevice`</span><span class="sxs-lookup"><span data-stu-id="9ba5e-120">Supported values are `urn:user:registersecurityinfo` and `urn:user:registerdevice`</span></span> |

## <a name="relationships"></a><span data-ttu-id="9ba5e-121">关系</span><span class="sxs-lookup"><span data-stu-id="9ba5e-121">Relationships</span></span>

<span data-ttu-id="9ba5e-122">无。</span><span class="sxs-lookup"><span data-stu-id="9ba5e-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ba5e-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ba5e-123">JSON representation</span></span>

<span data-ttu-id="9ba5e-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ba5e-124">The following is a JSON representation of the resource.</span></span>

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

