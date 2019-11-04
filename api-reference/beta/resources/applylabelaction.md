---
title: applyLabelAction 资源类型
description: 代表应用或更新标签应执行的一组操作。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fc7911b3a225f226edc74dc9b194a2522b7c4251
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939143"
---
# <a name="applylabelaction-resource-type"></a><span data-ttu-id="a6485-103">applyLabelAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6485-103">applyLabelAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6485-104">代表应用或更新标签应执行的一组操作。</span><span class="sxs-lookup"><span data-stu-id="a6485-104">Represents a set of actions that should be taken to apply or update a label.</span></span> <span data-ttu-id="a6485-105">当标签求值操作的结果是应应用标签时，将返回**applyLabelAction** 。</span><span class="sxs-lookup"><span data-stu-id="a6485-105">**applyLabelAction** is returned when the result of a label evaluation operation is that a label should be applied.</span></span> <span data-ttu-id="a6485-106">该`actions`属性包含一个[informationProtectionAction](informationProtectionaction.md)集合，该集合描述了要*应用*标签的完整操作集，包括删除旧元数据、内容标记和保护。</span><span class="sxs-lookup"><span data-stu-id="a6485-106">The `actions` property contains an [informationProtectionAction](informationProtectionaction.md) collection that described the full set of actions to *apply* the label, including removal of old metadata, content marking, and protection.</span></span>

## <a name="properties"></a><span data-ttu-id="a6485-107">属性</span><span class="sxs-lookup"><span data-stu-id="a6485-107">Properties</span></span>

| <span data-ttu-id="a6485-108">属性</span><span class="sxs-lookup"><span data-stu-id="a6485-108">Property</span></span>                    | <span data-ttu-id="a6485-109">类型</span><span class="sxs-lookup"><span data-stu-id="a6485-109">Type</span></span>                                                                     | <span data-ttu-id="a6485-110">描述</span><span class="sxs-lookup"><span data-stu-id="a6485-110">Description</span></span>                                                                                                                                                                                       |
| :-------------------------- | :----------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="a6485-111">actionSource</span><span class="sxs-lookup"><span data-stu-id="a6485-111">actionSource</span></span>                | <span data-ttu-id="a6485-112">String</span><span class="sxs-lookup"><span data-stu-id="a6485-112">String</span></span>                                                                   | <span data-ttu-id="a6485-113">可能的值是：`manual`、`automatic`、`recommended`、`default`。</span><span class="sxs-lookup"><span data-stu-id="a6485-113">Possible values are: `manual`, `automatic`, `recommended`, `default`.</span></span>                                                                                                                             |
| <span data-ttu-id="a6485-114">actions</span><span class="sxs-lookup"><span data-stu-id="a6485-114">actions</span></span>                     | <span data-ttu-id="a6485-115">[informationProtectionAction](informationprotectionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="a6485-115">[informationProtectionAction](informationprotectionaction.md) collection</span></span> | <span data-ttu-id="a6485-116">使用应用程序标记文档应采取的特定操作的集合。</span><span class="sxs-lookup"><span data-stu-id="a6485-116">The collection of specific actions that should be taken by the consuming application to label the document.</span></span> <span data-ttu-id="a6485-117">有关完整列表，请参阅[informationProtectionAction](informationprotectionaction.md) 。</span><span class="sxs-lookup"><span data-stu-id="a6485-117">See  [informationProtectionAction](informationprotectionaction.md) for the full list.</span></span> |
| <span data-ttu-id="a6485-118">label</span><span class="sxs-lookup"><span data-stu-id="a6485-118">label</span></span>                       | [<span data-ttu-id="a6485-119">labelDetails</span><span class="sxs-lookup"><span data-stu-id="a6485-119">labelDetails</span></span>](labeldetails.md)                                          | <span data-ttu-id="a6485-120">描述要应用的标签的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="a6485-120">Object that describes the details of the label to apply.</span></span>                                                                                                                                          |
| <span data-ttu-id="a6485-121">responsibleSensitiveTypeIds</span><span class="sxs-lookup"><span data-stu-id="a6485-121">responsibleSensitiveTypeIds</span></span> | <span data-ttu-id="a6485-122">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="a6485-122">Guid collection</span></span>                                                          | <span data-ttu-id="a6485-123">如果标签是自动分类的结果，请提供将导致返回的标签的敏感信息类型 Guid 的列表。</span><span class="sxs-lookup"><span data-stu-id="a6485-123">If the label was the result of an automatic classification, supply the list of sensitive info type GUIDs that resulted in the returned label.</span></span>                                         
## <a name="json-representation"></a><span data-ttu-id="a6485-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6485-124">JSON representation</span></span>

<span data-ttu-id="a6485-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6485-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applyLabelAction",
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
  "description": "applyLabelAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->