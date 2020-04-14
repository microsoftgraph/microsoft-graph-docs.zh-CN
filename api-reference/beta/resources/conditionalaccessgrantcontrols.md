---
title: conditionalAccessGrantControls 资源类型
description: 表示授予通过策略所需满足的控件。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9746bfb37dd3887def0f070256d90e46efecbdb6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413429"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="6768a-103">conditionalAccessGrantControls 资源类型</span><span class="sxs-lookup"><span data-stu-id="6768a-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="6768a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6768a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6768a-105">表示授予通过策略所需满足的控件。</span><span class="sxs-lookup"><span data-stu-id="6768a-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="6768a-106">属性</span><span class="sxs-lookup"><span data-stu-id="6768a-106">Properties</span></span>

| <span data-ttu-id="6768a-107">属性</span><span class="sxs-lookup"><span data-stu-id="6768a-107">Property</span></span> | <span data-ttu-id="6768a-108">类型</span><span class="sxs-lookup"><span data-stu-id="6768a-108">Type</span></span> | <span data-ttu-id="6768a-109">说明</span><span class="sxs-lookup"><span data-stu-id="6768a-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="6768a-110">operator</span><span class="sxs-lookup"><span data-stu-id="6768a-110">operator</span></span> | <span data-ttu-id="6768a-111">String</span><span class="sxs-lookup"><span data-stu-id="6768a-111">String</span></span> | <span data-ttu-id="6768a-112">定义授予控件的关系。</span><span class="sxs-lookup"><span data-stu-id="6768a-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="6768a-113">可能的值`AND`： `OR`、。</span><span class="sxs-lookup"><span data-stu-id="6768a-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="6768a-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="6768a-114">builtInControls</span></span> | <span data-ttu-id="6768a-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="6768a-115">String collection</span></span> | <span data-ttu-id="6768a-116">策略所需的内置控件的值列表。</span><span class="sxs-lookup"><span data-stu-id="6768a-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="6768a-117">可能的值`Block`： `Mfa`、 `CompliantDevice`、 `DomainJoinedDevice`、 `ApprovedApplication`、、`CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="6768a-117">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="6768a-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="6768a-118">customAuthenticationFactors</span></span> | <span data-ttu-id="6768a-119">String 集合</span><span class="sxs-lookup"><span data-stu-id="6768a-119">String collection</span></span> | <span data-ttu-id="6768a-120">策略所需的自定义控件 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="6768a-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="6768a-121">在此处了解有关自定义控件的详细信息：https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="6768a-121">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="6768a-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="6768a-122">termsOfUse</span></span> | <span data-ttu-id="6768a-123">String 集合</span><span class="sxs-lookup"><span data-stu-id="6768a-123">String collection</span></span> | <span data-ttu-id="6768a-124">策略所需的[使用条款](agreement.md)id 的列表。</span><span class="sxs-lookup"><span data-stu-id="6768a-124">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6768a-125">关系</span><span class="sxs-lookup"><span data-stu-id="6768a-125">Relationships</span></span>

<span data-ttu-id="6768a-126">无。</span><span class="sxs-lookup"><span data-stu-id="6768a-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6768a-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6768a-127">JSON representation</span></span>

<span data-ttu-id="6768a-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6768a-128">The following is a JSON representation of the resource.</span></span>

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