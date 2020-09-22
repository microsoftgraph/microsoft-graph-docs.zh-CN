---
title: conditionalAccessGrantControls 资源类型
description: 表示授予通过策略所需满足的控件。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e48d179e53111cc69b72eb8aa61c52ae105764df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018905"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="6ed78-103">conditionalAccessGrantControls 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ed78-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="6ed78-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ed78-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6ed78-105">表示授予通过策略所需满足的控件。</span><span class="sxs-lookup"><span data-stu-id="6ed78-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="6ed78-106">属性</span><span class="sxs-lookup"><span data-stu-id="6ed78-106">Properties</span></span>

| <span data-ttu-id="6ed78-107">属性</span><span class="sxs-lookup"><span data-stu-id="6ed78-107">Property</span></span> | <span data-ttu-id="6ed78-108">类型</span><span class="sxs-lookup"><span data-stu-id="6ed78-108">Type</span></span> | <span data-ttu-id="6ed78-109">说明</span><span class="sxs-lookup"><span data-stu-id="6ed78-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="6ed78-110">operator</span><span class="sxs-lookup"><span data-stu-id="6ed78-110">operator</span></span> | <span data-ttu-id="6ed78-111">String</span><span class="sxs-lookup"><span data-stu-id="6ed78-111">String</span></span> | <span data-ttu-id="6ed78-112">定义授予控件的关系。</span><span class="sxs-lookup"><span data-stu-id="6ed78-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="6ed78-113">可能的值： `AND` 、 `OR` 。</span><span class="sxs-lookup"><span data-stu-id="6ed78-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="6ed78-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="6ed78-114">builtInControls</span></span> | <span data-ttu-id="6ed78-115">String collection</span><span class="sxs-lookup"><span data-stu-id="6ed78-115">String collection</span></span> | <span data-ttu-id="6ed78-116">策略所需的内置控件的值列表。</span><span class="sxs-lookup"><span data-stu-id="6ed78-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="6ed78-117">可能的值： `Block` 、、、、 `Mfa` `CompliantDevice` `DomainJoinedDevice` `ApprovedApplication` 、 `CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="6ed78-117">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="6ed78-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="6ed78-118">customAuthenticationFactors</span></span> | <span data-ttu-id="6ed78-119">String collection</span><span class="sxs-lookup"><span data-stu-id="6ed78-119">String collection</span></span> | <span data-ttu-id="6ed78-120">策略所需的自定义控件 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="6ed78-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="6ed78-121">有关详细信息，请参阅 [自定义控件](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)。</span><span class="sxs-lookup"><span data-stu-id="6ed78-121">For more information, see [Custom controls](https://docs.microsoft.com/azure/active-directory/conditional-access/controls).</span></span> |
| <span data-ttu-id="6ed78-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="6ed78-122">termsOfUse</span></span> | <span data-ttu-id="6ed78-123">String collection</span><span class="sxs-lookup"><span data-stu-id="6ed78-123">String collection</span></span> | <span data-ttu-id="6ed78-124">策略所需的 [使用条款](https://docs.microsoft.com/graph/api/resources/agreement) id 的列表。</span><span class="sxs-lookup"><span data-stu-id="6ed78-124">List of [terms of use](https://docs.microsoft.com/graph/api/resources/agreement) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6ed78-125">关系</span><span class="sxs-lookup"><span data-stu-id="6ed78-125">Relationships</span></span>

<span data-ttu-id="6ed78-126">无。</span><span class="sxs-lookup"><span data-stu-id="6ed78-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ed78-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ed78-127">JSON representation</span></span>

<span data-ttu-id="6ed78-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ed78-128">The following is a JSON representation of the resource.</span></span>

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

