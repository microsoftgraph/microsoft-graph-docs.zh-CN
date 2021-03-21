---
title: recommendLabelAction 资源类型
description: 表示应建议用户根据敏感信息类型向文件应用的标签。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 10d3ac687605ab648cdd3d68d6a3721c8fba2e30
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962572"
---
# <a name="recommendlabelaction-resource-type"></a><span data-ttu-id="d159a-103">recommendLabelAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="d159a-103">recommendLabelAction resource type</span></span>

<span data-ttu-id="d159a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d159a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d159a-105">表示应建议用户根据发现的敏感信息类型向文件应用的标签。</span><span class="sxs-lookup"><span data-stu-id="d159a-105">Represents a label that should be recommended to the user for application to the file based on discovered sensitive information types.</span></span> <span data-ttu-id="d159a-106">如果 Microsoft 信息保护标签策略设置为推荐和标签，而不是强制执行标签，[则 evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md)可能会返回 **recommendLabelAction。** </span><span class="sxs-lookup"><span data-stu-id="d159a-106">The [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) may return a **recommendLabelAction** if the Microsoft Information Protection labeling policy is set to **recommend** and label rather than enforce a label.</span></span> <span data-ttu-id="d159a-107">用户或应用可以选择忽略或接受建议。</span><span class="sxs-lookup"><span data-stu-id="d159a-107">The user or appliation may choose to ignore or accept the recommendation.</span></span> 

## <a name="properties"></a><span data-ttu-id="d159a-108">属性</span><span class="sxs-lookup"><span data-stu-id="d159a-108">Properties</span></span>

| <span data-ttu-id="d159a-109">属性</span><span class="sxs-lookup"><span data-stu-id="d159a-109">Property</span></span>                    | <span data-ttu-id="d159a-110">类型</span><span class="sxs-lookup"><span data-stu-id="d159a-110">Type</span></span>                                                                     | <span data-ttu-id="d159a-111">说明</span><span class="sxs-lookup"><span data-stu-id="d159a-111">Description</span></span>                                                           |
| :-------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| <span data-ttu-id="d159a-112">actionSource</span><span class="sxs-lookup"><span data-stu-id="d159a-112">actionSource</span></span>                | <span data-ttu-id="d159a-113">String</span><span class="sxs-lookup"><span data-stu-id="d159a-113">String</span></span>                                                                   | <span data-ttu-id="d159a-114">可能的值是：`manual`、`automatic`、`recommended`、`default`。</span><span class="sxs-lookup"><span data-stu-id="d159a-114">Possible values are: `manual`, `automatic`, `recommended`, `default`.</span></span> |
| <span data-ttu-id="d159a-115">actions</span><span class="sxs-lookup"><span data-stu-id="d159a-115">actions</span></span>                     | <span data-ttu-id="d159a-116">[informationProtectionAction](informationprotectionaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d159a-116">[informationProtectionAction](informationprotectionaction.md) collection</span></span> | <span data-ttu-id="d159a-117">用户接受标签时要采取的操作。</span><span class="sxs-lookup"><span data-stu-id="d159a-117">Actions to take if the label is accepted by the user.</span></span>                                                                       |
| <span data-ttu-id="d159a-118">label</span><span class="sxs-lookup"><span data-stu-id="d159a-118">label</span></span>                       | [<span data-ttu-id="d159a-119">labelDetails</span><span class="sxs-lookup"><span data-stu-id="d159a-119">labelDetails</span></span>](labeldetails.md)                                          | <span data-ttu-id="d159a-120">建议的标签。</span><span class="sxs-lookup"><span data-stu-id="d159a-120">The label that is being recommended.</span></span>                                                                      |
| <span data-ttu-id="d159a-121">responsibleSensitiveTypeIds</span><span class="sxs-lookup"><span data-stu-id="d159a-121">responsibleSensitiveTypeIds</span></span> | <span data-ttu-id="d159a-122">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="d159a-122">Guid collection</span></span>                                                          | <span data-ttu-id="d159a-123">导致给出建议的敏感信息类型 GUID。</span><span class="sxs-lookup"><span data-stu-id="d159a-123">The sensitive information type GUIDs that caused the recommendation to be given.</span></span>                                                                      |

## <a name="json-representation"></a><span data-ttu-id="d159a-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d159a-124">JSON representation</span></span>

<span data-ttu-id="d159a-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d159a-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recommendLabelAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "actionSource": "String",
  "actions": [{"@odata.type": "microsoft.graph.informationProtectionAction"}],
  "label": {"@odata.type": "microsoft.graph.labelDetails"},
  "responsibleSensitiveTypeIds": ["Guid"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recommendLabelAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


