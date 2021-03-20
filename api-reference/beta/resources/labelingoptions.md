---
title: labelingOptions 资源类型
description: 表示可提供给评估 API 的标签选项。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7d2409bf538de3d37ca32cdf2fd1afb78a659817
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950297"
---
# <a name="labelingoptions-resource-type"></a><span data-ttu-id="bdff7-103">labelingOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="bdff7-103">labelingOptions resource type</span></span>

<span data-ttu-id="bdff7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdff7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdff7-105">表示可提供给评估 API 的标签选项。</span><span class="sxs-lookup"><span data-stu-id="bdff7-105">Represents the labeling options that can be provided to the evaluation APIs.</span></span> <span data-ttu-id="bdff7-106">**labelingOptions** 必须传递到 [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API，以指定有关要应用的标签的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bdff7-106">**labelingOptions** must be passed in to the [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API to specify details about the label that is to be applied.</span></span> 

## <a name="properties"></a><span data-ttu-id="bdff7-107">属性</span><span class="sxs-lookup"><span data-stu-id="bdff7-107">Properties</span></span>

| <span data-ttu-id="bdff7-108">属性</span><span class="sxs-lookup"><span data-stu-id="bdff7-108">Property</span></span>               | <span data-ttu-id="bdff7-109">类型</span><span class="sxs-lookup"><span data-stu-id="bdff7-109">Type</span></span>                                                | <span data-ttu-id="bdff7-110">说明</span><span class="sxs-lookup"><span data-stu-id="bdff7-110">Description</span></span>                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="bdff7-111">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="bdff7-111">assignmentMethod</span></span>       | <span data-ttu-id="bdff7-112">String</span><span class="sxs-lookup"><span data-stu-id="bdff7-112">String</span></span>                                              | <span data-ttu-id="bdff7-113">可取值为：`standard`、`privileged`、`auto`。</span><span class="sxs-lookup"><span data-stu-id="bdff7-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>                                                                        |
| <span data-ttu-id="bdff7-114">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="bdff7-114">downgradeJustification</span></span> | [<span data-ttu-id="bdff7-115">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="bdff7-115">downgradeJustification</span></span>](downgradejustification.md) | <span data-ttu-id="bdff7-116">用于指示降级是否合理以及原因（如果有）的降级理由对象。</span><span class="sxs-lookup"><span data-stu-id="bdff7-116">The downgrade justification object that indicates if downgrade was justified and, if so, the reason.</span></span>                          |
| <span data-ttu-id="bdff7-117">extendedProperties</span><span class="sxs-lookup"><span data-stu-id="bdff7-117">extendedProperties</span></span>     | <span data-ttu-id="bdff7-118">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bdff7-118">[keyValuePair](keyvaluepair.md) collection</span></span>          | <span data-ttu-id="bdff7-119">扩展属性将在标签信息中以标准 MIP 标记元数据格式进行分析和返回。</span><span class="sxs-lookup"><span data-stu-id="bdff7-119">Extended properties will be parsed and returned in the standard MIP labeled metadata format as part of the label information.</span></span> |
| <span data-ttu-id="bdff7-120">labelId</span><span class="sxs-lookup"><span data-stu-id="bdff7-120">labelId</span></span>                | <span data-ttu-id="bdff7-121">Guid</span><span class="sxs-lookup"><span data-stu-id="bdff7-121">Guid</span></span>                                                | <span data-ttu-id="bdff7-122">应用于信息的标签的 GUID。</span><span class="sxs-lookup"><span data-stu-id="bdff7-122">The GUID of the label that should be applied to the information.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="bdff7-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bdff7-123">JSON representation</span></span>

<span data-ttu-id="bdff7-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bdff7-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.labelingOptions",
  "baseType": null
}-->

```json
{
  "assignmentMethod": "String",
  "downgradeJustification": {"@odata.type": "microsoft.graph.downgradeJustification"},
  "extendedProperties": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "labelId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "labelingOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

