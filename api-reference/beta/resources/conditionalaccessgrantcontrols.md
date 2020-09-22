---
title: conditionalAccessGrantControls 资源类型
description: 表示授予通过策略所需满足的控件。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2bcb150239e6e6a8487caa3f49f7704fbd2550a8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994272"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="87c2c-103">conditionalAccessGrantControls 资源类型</span><span class="sxs-lookup"><span data-stu-id="87c2c-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="87c2c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87c2c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87c2c-105">表示授予通过策略所需满足的控件。</span><span class="sxs-lookup"><span data-stu-id="87c2c-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="87c2c-106">属性</span><span class="sxs-lookup"><span data-stu-id="87c2c-106">Properties</span></span>

| <span data-ttu-id="87c2c-107">属性</span><span class="sxs-lookup"><span data-stu-id="87c2c-107">Property</span></span> | <span data-ttu-id="87c2c-108">类型</span><span class="sxs-lookup"><span data-stu-id="87c2c-108">Type</span></span> | <span data-ttu-id="87c2c-109">说明</span><span class="sxs-lookup"><span data-stu-id="87c2c-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="87c2c-110">operator</span><span class="sxs-lookup"><span data-stu-id="87c2c-110">operator</span></span> | <span data-ttu-id="87c2c-111">String</span><span class="sxs-lookup"><span data-stu-id="87c2c-111">String</span></span> | <span data-ttu-id="87c2c-112">定义授予控件的关系。</span><span class="sxs-lookup"><span data-stu-id="87c2c-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="87c2c-113">可能的值： `AND` 、 `OR` 。</span><span class="sxs-lookup"><span data-stu-id="87c2c-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="87c2c-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="87c2c-114">builtInControls</span></span> | <span data-ttu-id="87c2c-115">String collection</span><span class="sxs-lookup"><span data-stu-id="87c2c-115">String collection</span></span> | <span data-ttu-id="87c2c-116">策略所需的内置控件的值列表。</span><span class="sxs-lookup"><span data-stu-id="87c2c-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="87c2c-117">可能的值：、、、、、 `block` `mfa` `compliantDevice` `domainJoinedDevice` `approvedApplication` `compliantApplication` 、 `passwordChange` 。</span><span class="sxs-lookup"><span data-stu-id="87c2c-117">Possible values: `block`, `mfa`, `compliantDevice`, `domainJoinedDevice`, `approvedApplication`, `compliantApplication`, `passwordChange`.</span></span> |
| <span data-ttu-id="87c2c-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="87c2c-118">customAuthenticationFactors</span></span> | <span data-ttu-id="87c2c-119">String collection</span><span class="sxs-lookup"><span data-stu-id="87c2c-119">String collection</span></span> | <span data-ttu-id="87c2c-120">策略所需的自定义控件 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="87c2c-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="87c2c-121">在此处了解有关自定义控件的详细信息： https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="87c2c-121">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="87c2c-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="87c2c-122">termsOfUse</span></span> | <span data-ttu-id="87c2c-123">String collection</span><span class="sxs-lookup"><span data-stu-id="87c2c-123">String collection</span></span> | <span data-ttu-id="87c2c-124">策略所需的 [使用条款](agreement.md) id 的列表。</span><span class="sxs-lookup"><span data-stu-id="87c2c-124">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

### <a name="special-considerations-when-using-passwordchange-as-a-control"></a><span data-ttu-id="87c2c-125">使用 `passwordChange` 作为控件时的特殊注意事项</span><span class="sxs-lookup"><span data-stu-id="87c2c-125">Special considerations when using `passwordChange` as a control</span></span>

<span data-ttu-id="87c2c-126">使用控件时，请注意以下 `passwordChange` 几点：</span><span class="sxs-lookup"><span data-stu-id="87c2c-126">Consider the following when you use the `passwordChange` control:</span></span> 

- <span data-ttu-id="87c2c-127">`passwordChange` 必须 `mfa` 与运算符一起使用 `AND` 。</span><span class="sxs-lookup"><span data-stu-id="87c2c-127">`passwordChange` must be accompanied by `mfa` using an `AND` operator.</span></span> <span data-ttu-id="87c2c-128">此组合可确保密码将以安全的方式进行更新。</span><span class="sxs-lookup"><span data-stu-id="87c2c-128">This combination ensures that the password will be updated in a secure way.</span></span>
- <span data-ttu-id="87c2c-129">`passwordChange` 必须在包含的策略中使用 `userRiskLevels` 。</span><span class="sxs-lookup"><span data-stu-id="87c2c-129">`passwordChange` must be used in a policy containing `userRiskLevels`.</span></span> <span data-ttu-id="87c2c-130">这旨在实现用户必须使用安全更改密码重置其用户风险的方案。</span><span class="sxs-lookup"><span data-stu-id="87c2c-130">This is designed to enable scenarios where users must use a secure change password to reset their user risk.</span></span>
- <span data-ttu-id="87c2c-131">该策略应以 `all` 应用程序为目标，而不排除任何应用程序。</span><span class="sxs-lookup"><span data-stu-id="87c2c-131">The policy should target `all` applications, and not exclude any applications.</span></span>
- <span data-ttu-id="87c2c-132">策略不能包含任何其他条件。</span><span class="sxs-lookup"><span data-stu-id="87c2c-132">The policy cannot contain any other condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="87c2c-133">关系</span><span class="sxs-lookup"><span data-stu-id="87c2c-133">Relationships</span></span>

<span data-ttu-id="87c2c-134">无。</span><span class="sxs-lookup"><span data-stu-id="87c2c-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87c2c-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87c2c-135">JSON representation</span></span>

<span data-ttu-id="87c2c-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87c2c-136">The following is a JSON representation of the resource.</span></span>

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


