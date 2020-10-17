---
title: conditionalAccessGrantControls 资源类型
description: 表示授予通过策略所需满足的控件。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 431ea73f20b36b189ae7638cc56a01239c1f113f
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582126"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="84393-103">conditionalAccessGrantControls 资源类型</span><span class="sxs-lookup"><span data-stu-id="84393-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="84393-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84393-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="84393-105">表示授予通过策略所需满足的控件。</span><span class="sxs-lookup"><span data-stu-id="84393-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="84393-106">属性</span><span class="sxs-lookup"><span data-stu-id="84393-106">Properties</span></span>

| <span data-ttu-id="84393-107">属性</span><span class="sxs-lookup"><span data-stu-id="84393-107">Property</span></span> | <span data-ttu-id="84393-108">类型</span><span class="sxs-lookup"><span data-stu-id="84393-108">Type</span></span> | <span data-ttu-id="84393-109">说明</span><span class="sxs-lookup"><span data-stu-id="84393-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="84393-110">operator</span><span class="sxs-lookup"><span data-stu-id="84393-110">operator</span></span> | <span data-ttu-id="84393-111">字符串</span><span class="sxs-lookup"><span data-stu-id="84393-111">String</span></span> | <span data-ttu-id="84393-112">定义授予控件的关系。</span><span class="sxs-lookup"><span data-stu-id="84393-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="84393-113">可能的值： `AND` 、 `OR` 。</span><span class="sxs-lookup"><span data-stu-id="84393-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="84393-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="84393-114">builtInControls</span></span> | <span data-ttu-id="84393-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="84393-115">String collection</span></span> | <span data-ttu-id="84393-116">策略所需的内置控件的值列表。</span><span class="sxs-lookup"><span data-stu-id="84393-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="84393-117">可能的值： `Block` 、、、、 `Mfa` `CompliantDevice` `DomainJoinedDevice` `ApprovedApplication` 、 `CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="84393-117">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="84393-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="84393-118">customAuthenticationFactors</span></span> | <span data-ttu-id="84393-119">String 集合</span><span class="sxs-lookup"><span data-stu-id="84393-119">String collection</span></span> | <span data-ttu-id="84393-120">策略所需的自定义控件 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="84393-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="84393-121">有关详细信息，请参阅 [自定义控件](/azure/active-directory/conditional-access/controls)。</span><span class="sxs-lookup"><span data-stu-id="84393-121">For more information, see [Custom controls](/azure/active-directory/conditional-access/controls).</span></span> |
| <span data-ttu-id="84393-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="84393-122">termsOfUse</span></span> | <span data-ttu-id="84393-123">String 集合</span><span class="sxs-lookup"><span data-stu-id="84393-123">String collection</span></span> | <span data-ttu-id="84393-124">策略所需的 [使用条款](/graph/api/resources/agreement) id 的列表。</span><span class="sxs-lookup"><span data-stu-id="84393-124">List of [terms of use](/graph/api/resources/agreement) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="84393-125">关系</span><span class="sxs-lookup"><span data-stu-id="84393-125">Relationships</span></span>

<span data-ttu-id="84393-126">无。</span><span class="sxs-lookup"><span data-stu-id="84393-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="84393-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84393-127">JSON representation</span></span>

<span data-ttu-id="84393-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84393-128">The following is a JSON representation of the resource.</span></span>

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