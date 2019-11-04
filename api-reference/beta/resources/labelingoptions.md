---
title: labelingOptions 资源类型
description: 表示可提供给评估 Api 的标记选项。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f8883c08bbd1f351dc5de003988f36c727ef85d7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939297"
---
# <a name="labelingoptions-resource-type"></a><span data-ttu-id="72050-103">labelingOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="72050-103">labelingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72050-104">表示可提供给评估 Api 的标记选项。</span><span class="sxs-lookup"><span data-stu-id="72050-104">Represents the labeling options that can be provided to the evaluation APIs.</span></span> <span data-ttu-id="72050-105">**labelingOptions**必须传递到[evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API，以指定要应用的标签的详细信息。</span><span class="sxs-lookup"><span data-stu-id="72050-105">**labelingOptions** must be passed in to the [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API to specify details about the label that is to be applied.</span></span> 

## <a name="properties"></a><span data-ttu-id="72050-106">属性</span><span class="sxs-lookup"><span data-stu-id="72050-106">Properties</span></span>

| <span data-ttu-id="72050-107">属性</span><span class="sxs-lookup"><span data-stu-id="72050-107">Property</span></span>               | <span data-ttu-id="72050-108">类型</span><span class="sxs-lookup"><span data-stu-id="72050-108">Type</span></span>                                                | <span data-ttu-id="72050-109">描述</span><span class="sxs-lookup"><span data-stu-id="72050-109">Description</span></span>                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="72050-110">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="72050-110">assignmentMethod</span></span>       | <span data-ttu-id="72050-111">字符串</span><span class="sxs-lookup"><span data-stu-id="72050-111">String</span></span>                                              | <span data-ttu-id="72050-112">可取值为：`standard`、`privileged`、`auto`。</span><span class="sxs-lookup"><span data-stu-id="72050-112">Possible values are: `standard`, `privileged`, `auto`.</span></span>                                                                        |
| <span data-ttu-id="72050-113">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="72050-113">downgradeJustification</span></span> | [<span data-ttu-id="72050-114">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="72050-114">downgradeJustification</span></span>](downgradejustification.md) | <span data-ttu-id="72050-115">降级理由对象，该对象指示降级是否已两端对齐，如果是，则指示原因。</span><span class="sxs-lookup"><span data-stu-id="72050-115">The downgrade justification object that indicates if downgrade was justified and, if so, the reason.</span></span>                          |
| <span data-ttu-id="72050-116">extendedProperties</span><span class="sxs-lookup"><span data-stu-id="72050-116">extendedProperties</span></span>     | <span data-ttu-id="72050-117">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72050-117">[keyValuePair](keyvaluepair.md) collection</span></span>          | <span data-ttu-id="72050-118">扩展属性将在作为标签信息一部分的标准 MIP 标记元数据格式中进行分析和返回。</span><span class="sxs-lookup"><span data-stu-id="72050-118">Extended properties will be parsed and returned in the standard MIP labeled metadata format as part of the label information.</span></span> |
| <span data-ttu-id="72050-119">labelId</span><span class="sxs-lookup"><span data-stu-id="72050-119">labelId</span></span>                | <span data-ttu-id="72050-120">Guid</span><span class="sxs-lookup"><span data-stu-id="72050-120">Guid</span></span>                                                | <span data-ttu-id="72050-121">应应用于信息的标签的 GUID。</span><span class="sxs-lookup"><span data-stu-id="72050-121">The GUID of the label that should be applied to the information.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="72050-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72050-122">JSON representation</span></span>

<span data-ttu-id="72050-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72050-123">The following is a JSON representation of the resource.</span></span>

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