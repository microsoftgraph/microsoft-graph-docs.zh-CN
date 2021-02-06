---
title: conditionalAccessGrantControls 资源类型
description: 表示为通过策略而必须实现的授予控制。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6d8717c1ca8fcd9113b8aeacb5a4a1cefce8df8f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130471"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="2b4e5-103">conditionalAccessGrantControls 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b4e5-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="2b4e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b4e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b4e5-105">表示为通过策略而必须实现的授予控制。</span><span class="sxs-lookup"><span data-stu-id="2b4e5-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="2b4e5-106">属性</span><span class="sxs-lookup"><span data-stu-id="2b4e5-106">Properties</span></span>

| <span data-ttu-id="2b4e5-107">属性</span><span class="sxs-lookup"><span data-stu-id="2b4e5-107">Property</span></span> | <span data-ttu-id="2b4e5-108">类型</span><span class="sxs-lookup"><span data-stu-id="2b4e5-108">Type</span></span> | <span data-ttu-id="2b4e5-109">说明</span><span class="sxs-lookup"><span data-stu-id="2b4e5-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="2b4e5-110">operator</span><span class="sxs-lookup"><span data-stu-id="2b4e5-110">operator</span></span> | <span data-ttu-id="2b4e5-111">字符串</span><span class="sxs-lookup"><span data-stu-id="2b4e5-111">String</span></span> | <span data-ttu-id="2b4e5-112">定义授予控件的关系。</span><span class="sxs-lookup"><span data-stu-id="2b4e5-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="2b4e5-113">可能的值： `AND` `OR` .</span><span class="sxs-lookup"><span data-stu-id="2b4e5-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="2b4e5-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="2b4e5-114">builtInControls</span></span> | <span data-ttu-id="2b4e5-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="2b4e5-115">String collection</span></span> | <span data-ttu-id="2b4e5-116">策略所需的内置控件的值列表。</span><span class="sxs-lookup"><span data-stu-id="2b4e5-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="2b4e5-117">可能的值： `block` `mfa` ， ， ， `compliantDevice` ， `domainJoinedDevice` `approvedApplication` `compliantApplication` 。 `passwordChange`</span><span class="sxs-lookup"><span data-stu-id="2b4e5-117">Possible values: `block`, `mfa`, `compliantDevice`, `domainJoinedDevice`, `approvedApplication`, `compliantApplication`, `passwordChange`.</span></span> |
| <span data-ttu-id="2b4e5-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="2b4e5-118">customAuthenticationFactors</span></span> | <span data-ttu-id="2b4e5-119">字符串集合</span><span class="sxs-lookup"><span data-stu-id="2b4e5-119">String collection</span></span> | <span data-ttu-id="2b4e5-120">策略所需的自定义控件的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="2b4e5-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="2b4e5-121">在此处了解有关自定义控件的更多信息： https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="2b4e5-121">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="2b4e5-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="2b4e5-122">termsOfUse</span></span> | <span data-ttu-id="2b4e5-123">字符串集合</span><span class="sxs-lookup"><span data-stu-id="2b4e5-123">String collection</span></span> | <span data-ttu-id="2b4e5-124">策略 [所需的](agreement.md) 使用条款 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="2b4e5-124">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a><span data-ttu-id="2b4e5-125">用作控件 `passwordChange` 时的特殊注意事项</span><span class="sxs-lookup"><span data-stu-id="2b4e5-125">Special considerations when using `passwordChange` as a control</span></span>

<span data-ttu-id="2b4e5-126">使用控件时，请考虑 `passwordChange` 以下事项：</span><span class="sxs-lookup"><span data-stu-id="2b4e5-126">Consider the following when you use the `passwordChange` control:</span></span> 

- <span data-ttu-id="2b4e5-127">`passwordChange` 必须附带使用 `mfa` `AND` 运算符。</span><span class="sxs-lookup"><span data-stu-id="2b4e5-127">`passwordChange` must be accompanied by `mfa` using an `AND` operator.</span></span> <span data-ttu-id="2b4e5-128">此组合可确保以安全的方式更新密码。</span><span class="sxs-lookup"><span data-stu-id="2b4e5-128">This combination ensures that the password will be updated in a secure way.</span></span>
- <span data-ttu-id="2b4e5-129">`passwordChange` 必须在包含的策略中使用 `userRiskLevels` 。</span><span class="sxs-lookup"><span data-stu-id="2b4e5-129">`passwordChange` must be used in a policy containing `userRiskLevels`.</span></span> <span data-ttu-id="2b4e5-130">这旨在支持用户必须使用安全更改密码重置其用户风险的方案。</span><span class="sxs-lookup"><span data-stu-id="2b4e5-130">This is designed to enable scenarios where users must use a secure change password to reset their user risk.</span></span>
- <span data-ttu-id="2b4e5-131">该策略应面向 `all` 应用程序，而不是排除任何应用程序。</span><span class="sxs-lookup"><span data-stu-id="2b4e5-131">The policy should target `all` applications, and not exclude any applications.</span></span>
- <span data-ttu-id="2b4e5-132">策略不能包含任何其他条件。</span><span class="sxs-lookup"><span data-stu-id="2b4e5-132">The policy cannot contain any other condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="2b4e5-133">关系</span><span class="sxs-lookup"><span data-stu-id="2b4e5-133">Relationships</span></span>

<span data-ttu-id="2b4e5-134">无。</span><span class="sxs-lookup"><span data-stu-id="2b4e5-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b4e5-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b4e5-135">JSON representation</span></span>

<span data-ttu-id="2b4e5-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b4e5-136">The following is a JSON representation of the resource.</span></span>

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


