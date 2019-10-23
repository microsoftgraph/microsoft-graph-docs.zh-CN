---
title: conditionalAccessGrantControls 资源类型
description: 表示授予通过策略所需满足的控件。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ebeb84ccf0e010ad792133f16f7819ca1d8b8ed0
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638496"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="e6f65-103">conditionalAccessGrantControls 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6f65-103">conditionalAccessGrantControls resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6f65-104">表示授予通过策略所需满足的控件。</span><span class="sxs-lookup"><span data-stu-id="e6f65-104">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="e6f65-105">属性</span><span class="sxs-lookup"><span data-stu-id="e6f65-105">Properties</span></span>

| <span data-ttu-id="e6f65-106">属性</span><span class="sxs-lookup"><span data-stu-id="e6f65-106">Property</span></span> | <span data-ttu-id="e6f65-107">类型</span><span class="sxs-lookup"><span data-stu-id="e6f65-107">Type</span></span> | <span data-ttu-id="e6f65-108">说明</span><span class="sxs-lookup"><span data-stu-id="e6f65-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="e6f65-109">operator</span><span class="sxs-lookup"><span data-stu-id="e6f65-109">operator</span></span> | <span data-ttu-id="e6f65-110">String</span><span class="sxs-lookup"><span data-stu-id="e6f65-110">String</span></span> | <span data-ttu-id="e6f65-111">定义授予控件的关系。</span><span class="sxs-lookup"><span data-stu-id="e6f65-111">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="e6f65-112">可能的值`AND`： `OR`、。</span><span class="sxs-lookup"><span data-stu-id="e6f65-112">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="e6f65-113">builtInControls</span><span class="sxs-lookup"><span data-stu-id="e6f65-113">builtInControls</span></span> | <span data-ttu-id="e6f65-114">String collection</span><span class="sxs-lookup"><span data-stu-id="e6f65-114">String collection</span></span> | <span data-ttu-id="e6f65-115">策略所需的内置控件的值列表。</span><span class="sxs-lookup"><span data-stu-id="e6f65-115">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="e6f65-116">可能的值`Block`： `Mfa`、 `CompliantDevice`、 `DomainJoinedDevice`、 `ApprovedApplication`、、`CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="e6f65-116">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="e6f65-117">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="e6f65-117">customAuthenticationFactors</span></span> | <span data-ttu-id="e6f65-118">String collection</span><span class="sxs-lookup"><span data-stu-id="e6f65-118">String collection</span></span> | <span data-ttu-id="e6f65-119">策略所需的自定义控件 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="e6f65-119">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="e6f65-120">在此处了解有关自定义控件的详细信息：https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="e6f65-120">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="e6f65-121">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="e6f65-121">termsOfUse</span></span> | <span data-ttu-id="e6f65-122">String collection</span><span class="sxs-lookup"><span data-stu-id="e6f65-122">String collection</span></span> | <span data-ttu-id="e6f65-123">策略所需的[使用条款](agreement.md)id 的列表。</span><span class="sxs-lookup"><span data-stu-id="e6f65-123">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e6f65-124">关系</span><span class="sxs-lookup"><span data-stu-id="e6f65-124">Relationships</span></span>

<span data-ttu-id="e6f65-125">无。</span><span class="sxs-lookup"><span data-stu-id="e6f65-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6f65-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6f65-126">JSON representation</span></span>

<span data-ttu-id="e6f65-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6f65-127">The following is a JSON representation of the resource.</span></span>

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