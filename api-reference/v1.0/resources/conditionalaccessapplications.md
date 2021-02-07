---
title: conditionalAccessApplications 资源类型
description: 表示包含在策略作用域中和从策略作用域中排除的应用程序和用户操作。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 42ceafb6c786666378d1327ecd158a04559d7f0d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132158"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="5eb2f-103">conditionalAccessApplications 资源类型</span><span class="sxs-lookup"><span data-stu-id="5eb2f-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="5eb2f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5eb2f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5eb2f-105">表示包含在策略中和从策略中排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="5eb2f-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="5eb2f-106">属性</span><span class="sxs-lookup"><span data-stu-id="5eb2f-106">Properties</span></span>

| <span data-ttu-id="5eb2f-107">属性</span><span class="sxs-lookup"><span data-stu-id="5eb2f-107">Property</span></span>     | <span data-ttu-id="5eb2f-108">类型</span><span class="sxs-lookup"><span data-stu-id="5eb2f-108">Type</span></span>        | <span data-ttu-id="5eb2f-109">说明</span><span class="sxs-lookup"><span data-stu-id="5eb2f-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5eb2f-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="5eb2f-110">includeApplications</span></span> | <span data-ttu-id="5eb2f-111">String collection</span><span class="sxs-lookup"><span data-stu-id="5eb2f-111">String collection</span></span> | <span data-ttu-id="5eb2f-112">除非在 excludeApplications (中明确) 。</span><span class="sxs-lookup"><span data-stu-id="5eb2f-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="5eb2f-113">也可以设置为 `All` 。</span><span class="sxs-lookup"><span data-stu-id="5eb2f-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="5eb2f-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="5eb2f-114">excludeApplications</span></span> | <span data-ttu-id="5eb2f-115">String collection</span><span class="sxs-lookup"><span data-stu-id="5eb2f-115">String collection</span></span> | <span data-ttu-id="5eb2f-116">从策略中明确排除的应用程序 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="5eb2f-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="5eb2f-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="5eb2f-117">includeUserActions</span></span> | <span data-ttu-id="5eb2f-118">String collection</span><span class="sxs-lookup"><span data-stu-id="5eb2f-118">String collection</span></span> | <span data-ttu-id="5eb2f-119">要包含的用户操作。</span><span class="sxs-lookup"><span data-stu-id="5eb2f-119">User actions to include.</span></span> <span data-ttu-id="5eb2f-120">例如，`urn:user:registersecurityinfo`</span><span class="sxs-lookup"><span data-stu-id="5eb2f-120">For example, `urn:user:registersecurityinfo`</span></span> |

## <a name="relationships"></a><span data-ttu-id="5eb2f-121">关系</span><span class="sxs-lookup"><span data-stu-id="5eb2f-121">Relationships</span></span>

<span data-ttu-id="5eb2f-122">无。</span><span class="sxs-lookup"><span data-stu-id="5eb2f-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5eb2f-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5eb2f-123">JSON representation</span></span>

<span data-ttu-id="5eb2f-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5eb2f-124">The following is a JSON representation of the resource.</span></span>

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

