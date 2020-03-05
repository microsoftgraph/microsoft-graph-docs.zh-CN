---
title: labelingOptions 资源类型
description: 表示可提供给评估 Api 的标记选项。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 97557ad6e233506e5e074c408ffb04f83297f0af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523000"
---
# <a name="labelingoptions-resource-type"></a><span data-ttu-id="5c026-103">labelingOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c026-103">labelingOptions resource type</span></span>

<span data-ttu-id="5c026-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5c026-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c026-105">表示可提供给评估 Api 的标记选项。</span><span class="sxs-lookup"><span data-stu-id="5c026-105">Represents the labeling options that can be provided to the evaluation APIs.</span></span> <span data-ttu-id="5c026-106">**labelingOptions**必须传递到[evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API，以指定要应用的标签的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5c026-106">**labelingOptions** must be passed in to the [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API to specify details about the label that is to be applied.</span></span> 

## <a name="properties"></a><span data-ttu-id="5c026-107">属性</span><span class="sxs-lookup"><span data-stu-id="5c026-107">Properties</span></span>

| <span data-ttu-id="5c026-108">属性</span><span class="sxs-lookup"><span data-stu-id="5c026-108">Property</span></span>               | <span data-ttu-id="5c026-109">类型</span><span class="sxs-lookup"><span data-stu-id="5c026-109">Type</span></span>                                                | <span data-ttu-id="5c026-110">说明</span><span class="sxs-lookup"><span data-stu-id="5c026-110">Description</span></span>                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5c026-111">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="5c026-111">assignmentMethod</span></span>       | <span data-ttu-id="5c026-112">String</span><span class="sxs-lookup"><span data-stu-id="5c026-112">String</span></span>                                              | <span data-ttu-id="5c026-113">可取值为：`standard`、`privileged`、`auto`。</span><span class="sxs-lookup"><span data-stu-id="5c026-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>                                                                        |
| <span data-ttu-id="5c026-114">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="5c026-114">downgradeJustification</span></span> | [<span data-ttu-id="5c026-115">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="5c026-115">downgradeJustification</span></span>](downgradejustification.md) | <span data-ttu-id="5c026-116">降级理由对象，该对象指示降级是否已两端对齐，如果是，则指示原因。</span><span class="sxs-lookup"><span data-stu-id="5c026-116">The downgrade justification object that indicates if downgrade was justified and, if so, the reason.</span></span>                          |
| <span data-ttu-id="5c026-117">extendedProperties</span><span class="sxs-lookup"><span data-stu-id="5c026-117">extendedProperties</span></span>     | <span data-ttu-id="5c026-118">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5c026-118">[keyValuePair](keyvaluepair.md) collection</span></span>          | <span data-ttu-id="5c026-119">扩展属性将在作为标签信息一部分的标准 MIP 标记元数据格式中进行分析和返回。</span><span class="sxs-lookup"><span data-stu-id="5c026-119">Extended properties will be parsed and returned in the standard MIP labeled metadata format as part of the label information.</span></span> |
| <span data-ttu-id="5c026-120">labelId</span><span class="sxs-lookup"><span data-stu-id="5c026-120">labelId</span></span>                | <span data-ttu-id="5c026-121">Guid</span><span class="sxs-lookup"><span data-stu-id="5c026-121">Guid</span></span>                                                | <span data-ttu-id="5c026-122">应应用于信息的标签的 GUID。</span><span class="sxs-lookup"><span data-stu-id="5c026-122">The GUID of the label that should be applied to the information.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="5c026-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c026-123">JSON representation</span></span>

<span data-ttu-id="5c026-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c026-124">The following is a JSON representation of the resource.</span></span>

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