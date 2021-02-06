---
title: evaluateDynamicMembershipResult 资源类型
description: 表示成员身份评估的结果。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 1df07449605f3b1d48c01b1e352100d534fc9b1d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129504"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a><span data-ttu-id="cb2ad-103">evaluateDynamicMembershipResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb2ad-103">evaluateDynamicMembershipResult resource type</span></span>

<span data-ttu-id="cb2ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb2ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb2ad-105">表示成员身份评估的结果。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-105">Represents the result of membership evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="cb2ad-106">属性</span><span class="sxs-lookup"><span data-stu-id="cb2ad-106">Properties</span></span>

| <span data-ttu-id="cb2ad-107">属性</span><span class="sxs-lookup"><span data-stu-id="cb2ad-107">Property</span></span> | <span data-ttu-id="cb2ad-108">类型</span><span class="sxs-lookup"><span data-stu-id="cb2ad-108">Type</span></span> | <span data-ttu-id="cb2ad-109">说明</span><span class="sxs-lookup"><span data-stu-id="cb2ad-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="cb2ad-110">membershipRule</span><span class="sxs-lookup"><span data-stu-id="cb2ad-110">membershipRule</span></span> | <span data-ttu-id="cb2ad-111">String</span><span class="sxs-lookup"><span data-stu-id="cb2ad-111">String</span></span> | <span data-ttu-id="cb2ad-112">如果提供了组 ID，则值为组的成员身份规则。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-112">If a group ID is provided, the value is the membership rule for the group.</span></span> <span data-ttu-id="cb2ad-113">如果未提供组 ID，则值为作为参数提供的成员资格规则。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-113">If a group ID is not provided, the value is the membership rule that was provided as a parameter.</span></span> <span data-ttu-id="cb2ad-114">有关详细信息，请参阅 [Azure Active Directory 中组的动态成员身份规则](/azure/active-directory/users-groups-roles/groups-dynamic-membership)。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-114">For more information, see [Dynamic membership rules for groups in Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span> |
| <span data-ttu-id="cb2ad-115">membershipRuleEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="cb2ad-115">membershipRuleEvaluationDetails</span></span> | [<span data-ttu-id="cb2ad-116">expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="cb2ad-116">expressionEvaluationDetails</span></span>](expressionevaluationdetails.md) | <span data-ttu-id="cb2ad-117">提供成员资格评估结果的详细分析。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-117">Provides a detailed anaylsis of the membership evaluation result.</span></span> |
| <span data-ttu-id="cb2ad-118">membershipRuleEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="cb2ad-118">membershipRuleEvaluationResult</span></span> | <span data-ttu-id="cb2ad-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb2ad-119">Boolean</span></span> | <span data-ttu-id="cb2ad-120">该值是 `true` 用户或设备是组的成员。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-120">The value is `true` if the user or device is a member of the group.</span></span> <span data-ttu-id="cb2ad-121">如果提供了成员资格规则，并且用户或设备通过规则评估，则值也可能 `true` 为 ;否则 `false` 为 。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-121">The value can also be `true` if a membership rule was provided and the user or device passes the rule evaluation; otherwise `false`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cb2ad-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb2ad-122">JSON representation</span></span>

<span data-ttu-id="cb2ad-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb2ad-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.evaluateDynamicMembershipResult",
  "baseType": null
}-->

```json
{
  "membershipRule": "String",
  "membershipRuleEvaluationDetails": {"@odata.type": "microsoft.graph.expressionEvaluationDetails"},
  "membershipRuleEvaluationResult": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "evaluateDynamicMembershipResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->