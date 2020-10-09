---
title: evaluateDynamicMembershipResult 资源类型
description: 表示成员资格评估的结果。
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d00a2f1a0376c0d631354ea4f05c542dd4d1dcef
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402534"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a><span data-ttu-id="bb97d-103">evaluateDynamicMembershipResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb97d-103">evaluateDynamicMembershipResult resource type</span></span>

<span data-ttu-id="bb97d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb97d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb97d-105">表示成员资格评估的结果。</span><span class="sxs-lookup"><span data-stu-id="bb97d-105">Represents the result of membership evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="bb97d-106">属性</span><span class="sxs-lookup"><span data-stu-id="bb97d-106">Properties</span></span>

| <span data-ttu-id="bb97d-107">属性</span><span class="sxs-lookup"><span data-stu-id="bb97d-107">Property</span></span> | <span data-ttu-id="bb97d-108">类型</span><span class="sxs-lookup"><span data-stu-id="bb97d-108">Type</span></span> | <span data-ttu-id="bb97d-109">说明</span><span class="sxs-lookup"><span data-stu-id="bb97d-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="bb97d-110">membershipRule</span><span class="sxs-lookup"><span data-stu-id="bb97d-110">membershipRule</span></span> | <span data-ttu-id="bb97d-111">String</span><span class="sxs-lookup"><span data-stu-id="bb97d-111">String</span></span> | <span data-ttu-id="bb97d-112">如果提供了组 ID，则此值为组的成员身份规则。</span><span class="sxs-lookup"><span data-stu-id="bb97d-112">If a group ID is provided, the value is the membership rule for the group.</span></span> <span data-ttu-id="bb97d-113">如果未提供组 ID，则值是作为参数提供的成员身份规则。</span><span class="sxs-lookup"><span data-stu-id="bb97d-113">If a group ID is not provided, the value is the membership rule that was provided as a parameter.</span></span> <span data-ttu-id="bb97d-114">有关详细信息，请参阅 [Azure Active Directory 中的组的动态成员身份规则](/azure/active-directory/users-groups-roles/groups-dynamic-membership)。</span><span class="sxs-lookup"><span data-stu-id="bb97d-114">For more information, see [Dynamic membership rules for groups in Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span> |
| <span data-ttu-id="bb97d-115">membershipRuleEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="bb97d-115">membershipRuleEvaluationDetails</span></span> | [<span data-ttu-id="bb97d-116">expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="bb97d-116">expressionEvaluationDetails</span></span>](expressionevaluationdetails.md) | <span data-ttu-id="bb97d-117">提供成员资格评估结果的详细 anaylsis。</span><span class="sxs-lookup"><span data-stu-id="bb97d-117">Provides a detailed anaylsis of the membership evaluation result.</span></span> |
| <span data-ttu-id="bb97d-118">membershipRuleEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="bb97d-118">membershipRuleEvaluationResult</span></span> | <span data-ttu-id="bb97d-119">布尔</span><span class="sxs-lookup"><span data-stu-id="bb97d-119">Boolean</span></span> | <span data-ttu-id="bb97d-120">值为 `true` 用户或设备是否为组的成员。</span><span class="sxs-lookup"><span data-stu-id="bb97d-120">The value is `true` if the user or device is a member of the group.</span></span> <span data-ttu-id="bb97d-121">`true`如果提供了成员身份规则，并且用户或设备传递了规则评估，则也可以是值; 否则，也是如此 `false` 。</span><span class="sxs-lookup"><span data-stu-id="bb97d-121">The value can also be `true` if a membership rule was provided and the user or device passes the rule evaluation; otherwise `false`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bb97d-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb97d-122">JSON representation</span></span>

<span data-ttu-id="bb97d-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb97d-123">The following is a JSON representation of the resource.</span></span>

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