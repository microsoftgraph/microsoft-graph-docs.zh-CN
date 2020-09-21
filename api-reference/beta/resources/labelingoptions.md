---
title: labelingOptions 资源类型
description: 表示可提供给评估 Api 的标记选项。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: da2231ae3eb95260663d2907f56f91b96e08278c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084016"
---
# <a name="labelingoptions-resource-type"></a><span data-ttu-id="5ed02-103">labelingOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ed02-103">labelingOptions resource type</span></span>

<span data-ttu-id="5ed02-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ed02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ed02-105">表示可提供给评估 Api 的标记选项。</span><span class="sxs-lookup"><span data-stu-id="5ed02-105">Represents the labeling options that can be provided to the evaluation APIs.</span></span> <span data-ttu-id="5ed02-106">**labelingOptions** 必须传递到 [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API，以指定要应用的标签的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5ed02-106">**labelingOptions** must be passed in to the [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API to specify details about the label that is to be applied.</span></span> 

## <a name="properties"></a><span data-ttu-id="5ed02-107">属性</span><span class="sxs-lookup"><span data-stu-id="5ed02-107">Properties</span></span>

| <span data-ttu-id="5ed02-108">属性</span><span class="sxs-lookup"><span data-stu-id="5ed02-108">Property</span></span>               | <span data-ttu-id="5ed02-109">类型</span><span class="sxs-lookup"><span data-stu-id="5ed02-109">Type</span></span>                                                | <span data-ttu-id="5ed02-110">说明</span><span class="sxs-lookup"><span data-stu-id="5ed02-110">Description</span></span>                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5ed02-111">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="5ed02-111">assignmentMethod</span></span>       | <span data-ttu-id="5ed02-112">字符串</span><span class="sxs-lookup"><span data-stu-id="5ed02-112">String</span></span>                                              | <span data-ttu-id="5ed02-113">可取值为：`standard`、`privileged`、`auto`。</span><span class="sxs-lookup"><span data-stu-id="5ed02-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>                                                                        |
| <span data-ttu-id="5ed02-114">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="5ed02-114">downgradeJustification</span></span> | [<span data-ttu-id="5ed02-115">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="5ed02-115">downgradeJustification</span></span>](downgradejustification.md) | <span data-ttu-id="5ed02-116">降级理由对象，该对象指示降级是否已两端对齐，如果是，则指示原因。</span><span class="sxs-lookup"><span data-stu-id="5ed02-116">The downgrade justification object that indicates if downgrade was justified and, if so, the reason.</span></span>                          |
| <span data-ttu-id="5ed02-117">extendedProperties</span><span class="sxs-lookup"><span data-stu-id="5ed02-117">extendedProperties</span></span>     | <span data-ttu-id="5ed02-118">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5ed02-118">[keyValuePair](keyvaluepair.md) collection</span></span>          | <span data-ttu-id="5ed02-119">扩展属性将在作为标签信息一部分的标准 MIP 标记元数据格式中进行分析和返回。</span><span class="sxs-lookup"><span data-stu-id="5ed02-119">Extended properties will be parsed and returned in the standard MIP labeled metadata format as part of the label information.</span></span> |
| <span data-ttu-id="5ed02-120">labelId</span><span class="sxs-lookup"><span data-stu-id="5ed02-120">labelId</span></span>                | <span data-ttu-id="5ed02-121">Guid</span><span class="sxs-lookup"><span data-stu-id="5ed02-121">Guid</span></span>                                                | <span data-ttu-id="5ed02-122">应应用于信息的标签的 GUID。</span><span class="sxs-lookup"><span data-stu-id="5ed02-122">The GUID of the label that should be applied to the information.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="5ed02-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ed02-123">JSON representation</span></span>

<span data-ttu-id="5ed02-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ed02-124">The following is a JSON representation of the resource.</span></span>

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

