---
title: conditionalAccessFilter 资源类型
description: 表示策略作用域中的筛选器。
localization_priority: Normal
author: sandeo
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9f5b14a3faa593453c88cc155f7e44348fcfda35
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082404"
---
# <a name="conditionalaccessfilter-resource-type"></a><span data-ttu-id="01854-103">conditionalAccessFilter 资源类型</span><span class="sxs-lookup"><span data-stu-id="01854-103">conditionalAccessFilter resource type</span></span>

<span data-ttu-id="01854-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01854-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01854-105">表示策略作用域中的筛选器。</span><span class="sxs-lookup"><span data-stu-id="01854-105">Represents filter in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="01854-106">属性</span><span class="sxs-lookup"><span data-stu-id="01854-106">Properties</span></span>

| <span data-ttu-id="01854-107">属性</span><span class="sxs-lookup"><span data-stu-id="01854-107">Property</span></span>     | <span data-ttu-id="01854-108">类型</span><span class="sxs-lookup"><span data-stu-id="01854-108">Type</span></span>        | <span data-ttu-id="01854-109">说明</span><span class="sxs-lookup"><span data-stu-id="01854-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="01854-110">mode</span><span class="sxs-lookup"><span data-stu-id="01854-110">mode</span></span> | <span data-ttu-id="01854-111">filterMode</span><span class="sxs-lookup"><span data-stu-id="01854-111">filterMode</span></span> | <span data-ttu-id="01854-112">用于筛选器的模式。</span><span class="sxs-lookup"><span data-stu-id="01854-112">Mode to use for the filter.</span></span> <span data-ttu-id="01854-113">可能的值为 `include` 或 `exclude`。</span><span class="sxs-lookup"><span data-stu-id="01854-113">Possible values are `include` or `exclude`.</span></span> |
| <span data-ttu-id="01854-114">rule</span><span class="sxs-lookup"><span data-stu-id="01854-114">rule</span></span> | <span data-ttu-id="01854-115">String</span><span class="sxs-lookup"><span data-stu-id="01854-115">String</span></span> | <span data-ttu-id="01854-116">规则语法类似于用于 Azure AD 中组成员身份规则的语法。</span><span class="sxs-lookup"><span data-stu-id="01854-116">Rule syntax is similar to that used for membership rules for groups in Azure AD.</span></span> <span data-ttu-id="01854-117">有关详细信息，请参阅 [包含多个表达式的规则](/azure/active-directory/enterprise-users/groups-dynamic-membership#rules-with-multiple-expressions)</span><span class="sxs-lookup"><span data-stu-id="01854-117">For details, see [rules with multiple expressions](/azure/active-directory/enterprise-users/groups-dynamic-membership#rules-with-multiple-expressions)</span></span> |

## <a name="relationships"></a><span data-ttu-id="01854-118">关系</span><span class="sxs-lookup"><span data-stu-id="01854-118">Relationships</span></span>

<span data-ttu-id="01854-119">无。</span><span class="sxs-lookup"><span data-stu-id="01854-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="01854-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01854-120">JSON representation</span></span>

<span data-ttu-id="01854-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01854-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "mode",
    "rule"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessFilter",
  "baseType": null
}-->

```json
{
  "mode": "String",
  "rule": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessFilter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


