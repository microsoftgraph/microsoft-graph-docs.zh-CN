---
title: conditionalAccessGrantControls 资源类型
description: 表示授予通过策略所需满足的控件。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b91afb44cc43c3c6ac4970afc36914abcb08c4c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507546"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="b523d-103">conditionalAccessGrantControls 资源类型</span><span class="sxs-lookup"><span data-stu-id="b523d-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="b523d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b523d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b523d-105">表示授予通过策略所需满足的控件。</span><span class="sxs-lookup"><span data-stu-id="b523d-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="b523d-106">属性</span><span class="sxs-lookup"><span data-stu-id="b523d-106">Properties</span></span>

| <span data-ttu-id="b523d-107">属性</span><span class="sxs-lookup"><span data-stu-id="b523d-107">Property</span></span> | <span data-ttu-id="b523d-108">类型</span><span class="sxs-lookup"><span data-stu-id="b523d-108">Type</span></span> | <span data-ttu-id="b523d-109">说明</span><span class="sxs-lookup"><span data-stu-id="b523d-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="b523d-110">operator</span><span class="sxs-lookup"><span data-stu-id="b523d-110">operator</span></span> | <span data-ttu-id="b523d-111">String</span><span class="sxs-lookup"><span data-stu-id="b523d-111">String</span></span> | <span data-ttu-id="b523d-112">定义授予控件的关系。</span><span class="sxs-lookup"><span data-stu-id="b523d-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="b523d-113">可能的值`AND`： `OR`、。</span><span class="sxs-lookup"><span data-stu-id="b523d-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="b523d-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="b523d-114">builtInControls</span></span> | <span data-ttu-id="b523d-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="b523d-115">String collection</span></span> | <span data-ttu-id="b523d-116">策略所需的内置控件的值列表。</span><span class="sxs-lookup"><span data-stu-id="b523d-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="b523d-117">可能的值`Block`： `Mfa`、 `CompliantDevice`、 `DomainJoinedDevice`、 `ApprovedApplication`、、`CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="b523d-117">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="b523d-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="b523d-118">customAuthenticationFactors</span></span> | <span data-ttu-id="b523d-119">String 集合</span><span class="sxs-lookup"><span data-stu-id="b523d-119">String collection</span></span> | <span data-ttu-id="b523d-120">策略所需的自定义控件 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="b523d-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="b523d-121">在此处了解有关自定义控件的详细信息：https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="b523d-121">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="b523d-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="b523d-122">termsOfUse</span></span> | <span data-ttu-id="b523d-123">String 集合</span><span class="sxs-lookup"><span data-stu-id="b523d-123">String collection</span></span> | <span data-ttu-id="b523d-124">策略所需的[使用条款](agreement.md)id 的列表。</span><span class="sxs-lookup"><span data-stu-id="b523d-124">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b523d-125">关系</span><span class="sxs-lookup"><span data-stu-id="b523d-125">Relationships</span></span>

<span data-ttu-id="b523d-126">无。</span><span class="sxs-lookup"><span data-stu-id="b523d-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b523d-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b523d-127">JSON representation</span></span>

<span data-ttu-id="b523d-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b523d-128">The following is a JSON representation of the resource.</span></span>

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