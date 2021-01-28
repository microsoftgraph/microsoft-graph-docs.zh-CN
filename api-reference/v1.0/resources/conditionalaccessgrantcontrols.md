---
title: conditionalAccessGrantControls 资源类型
description: 表示通过策略时必须实现的授予控制。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b0b93508db666fc1673f1c8154ef638762a872f3
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013665"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="e7f71-103">conditionalAccessGrantControls 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7f71-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="e7f71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7f71-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e7f71-105">表示通过策略时必须实现的授予控制。</span><span class="sxs-lookup"><span data-stu-id="e7f71-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="e7f71-106">属性</span><span class="sxs-lookup"><span data-stu-id="e7f71-106">Properties</span></span>

| <span data-ttu-id="e7f71-107">属性</span><span class="sxs-lookup"><span data-stu-id="e7f71-107">Property</span></span> | <span data-ttu-id="e7f71-108">类型</span><span class="sxs-lookup"><span data-stu-id="e7f71-108">Type</span></span> | <span data-ttu-id="e7f71-109">说明</span><span class="sxs-lookup"><span data-stu-id="e7f71-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="e7f71-110">operator</span><span class="sxs-lookup"><span data-stu-id="e7f71-110">operator</span></span> | <span data-ttu-id="e7f71-111">String</span><span class="sxs-lookup"><span data-stu-id="e7f71-111">String</span></span> | <span data-ttu-id="e7f71-112">定义授予控件的关系。</span><span class="sxs-lookup"><span data-stu-id="e7f71-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="e7f71-113">可能的值： `AND` `OR` .</span><span class="sxs-lookup"><span data-stu-id="e7f71-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="e7f71-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="e7f71-114">builtInControls</span></span> | <span data-ttu-id="e7f71-115">String collection</span><span class="sxs-lookup"><span data-stu-id="e7f71-115">String collection</span></span> | <span data-ttu-id="e7f71-116">策略所需的内置控件的值列表。</span><span class="sxs-lookup"><span data-stu-id="e7f71-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="e7f71-117">可能的值： `block` `mfa` ， `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` 。 `passwordChange`</span><span class="sxs-lookup"><span data-stu-id="e7f71-117">Possible values: `block`, `mfa`, `compliantDevice`, `domainJoinedDevice`, `approvedApplication`, `compliantApplication`, `passwordChange`.</span></span> |
| <span data-ttu-id="e7f71-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="e7f71-118">customAuthenticationFactors</span></span> | <span data-ttu-id="e7f71-119">String collection</span><span class="sxs-lookup"><span data-stu-id="e7f71-119">String collection</span></span> | <span data-ttu-id="e7f71-120">策略所需的自定义控件的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="e7f71-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="e7f71-121">有关详细信息，请参阅自定义 [控件](/azure/active-directory/conditional-access/controls)。</span><span class="sxs-lookup"><span data-stu-id="e7f71-121">For more information, see [Custom controls](/azure/active-directory/conditional-access/controls).</span></span> |
| <span data-ttu-id="e7f71-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="e7f71-122">termsOfUse</span></span> | <span data-ttu-id="e7f71-123">String collection</span><span class="sxs-lookup"><span data-stu-id="e7f71-123">String collection</span></span> | <span data-ttu-id="e7f71-124">策略 [所需的](/graph/api/resources/agreement) 使用条款 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="e7f71-124">List of [terms of use](/graph/api/resources/agreement) IDs required by the policy.</span></span> |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a><span data-ttu-id="e7f71-125">用作控件 `passwordChange` 时的特殊注意事项</span><span class="sxs-lookup"><span data-stu-id="e7f71-125">Special considerations when using `passwordChange` as a control</span></span>

<span data-ttu-id="e7f71-126">使用控件时，请考虑 `passwordChange` 以下事项：</span><span class="sxs-lookup"><span data-stu-id="e7f71-126">Consider the following when you use the `passwordChange` control:</span></span> 

- <span data-ttu-id="e7f71-127">`passwordChange` 必须附带使用 `mfa` `AND` 运算符。</span><span class="sxs-lookup"><span data-stu-id="e7f71-127">`passwordChange` must be accompanied by `mfa` using an `AND` operator.</span></span> <span data-ttu-id="e7f71-128">此组合可确保以安全方式更新密码。</span><span class="sxs-lookup"><span data-stu-id="e7f71-128">This combination ensures that the password will be updated in a secure way.</span></span>
- <span data-ttu-id="e7f71-129">`passwordChange` 必须在包含的策略中使用 `userRiskLevels` 。</span><span class="sxs-lookup"><span data-stu-id="e7f71-129">`passwordChange` must be used in a policy containing `userRiskLevels`.</span></span> <span data-ttu-id="e7f71-130">这旨在支持用户必须使用安全更改密码重置其用户风险的方案。</span><span class="sxs-lookup"><span data-stu-id="e7f71-130">This is designed to enable scenarios where users must use a secure change password to reset their user risk.</span></span>
- <span data-ttu-id="e7f71-131">该策略应面向 `all` 应用程序，而不是排除任何应用程序。</span><span class="sxs-lookup"><span data-stu-id="e7f71-131">The policy should target `all` applications, and not exclude any applications.</span></span>
- <span data-ttu-id="e7f71-132">该策略不能包含除 .和 以外的 `users` `applications` 任何其他条件 `userRiskLevels` 。</span><span class="sxs-lookup"><span data-stu-id="e7f71-132">The policy cannot contain any other condition except `users`, `applications` and `userRiskLevels`.</span></span>

## <a name="relationships"></a><span data-ttu-id="e7f71-133">关系</span><span class="sxs-lookup"><span data-stu-id="e7f71-133">Relationships</span></span>

<span data-ttu-id="e7f71-134">无。</span><span class="sxs-lookup"><span data-stu-id="e7f71-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7f71-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7f71-135">JSON representation</span></span>

<span data-ttu-id="e7f71-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7f71-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "operator",
    "builtInControls",
    "customAuthenticationFactors",
    "termsOfUse"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessGrantControls",
  "baseType": null
}-->

```json
{
  "builtInControls": ["String"],
  "customAuthenticationFactors": ["String"],
  "operator": "String",
  "termsOfUse": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessGrantControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->