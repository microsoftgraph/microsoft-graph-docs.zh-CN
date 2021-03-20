---
title: applyLabelAction 资源类型
description: 表示应用或更新标签时应该采取的一组操作。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e53a2796c7cd4f0b8c0a415ca4bc38ffefeb609e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945737"
---
# <a name="applylabelaction-resource-type"></a><span data-ttu-id="4aa9a-103">applyLabelAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="4aa9a-103">applyLabelAction resource type</span></span>

<span data-ttu-id="4aa9a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4aa9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4aa9a-105">表示应用或更新标签时应该采取的一组操作。</span><span class="sxs-lookup"><span data-stu-id="4aa9a-105">Represents a set of actions that should be taken to apply or update a label.</span></span> <span data-ttu-id="4aa9a-106">当标签评估操作的结果是应应用标签时，将返回 **applyLabelAction。**</span><span class="sxs-lookup"><span data-stu-id="4aa9a-106">**applyLabelAction** is returned when the result of a label evaluation operation is that a label should be applied.</span></span> <span data-ttu-id="4aa9a-107">属性 `actions` 包含[一个 informationProtectionAction](informationProtectionaction.md)集合，该集合描述要应用标签的完整操作集，包括删除旧元数据、内容标记和保护。</span><span class="sxs-lookup"><span data-stu-id="4aa9a-107">The `actions` property contains an [informationProtectionAction](informationProtectionaction.md) collection that described the full set of actions to *apply* the label, including removal of old metadata, content marking, and protection.</span></span>

## <a name="properties"></a><span data-ttu-id="4aa9a-108">属性</span><span class="sxs-lookup"><span data-stu-id="4aa9a-108">Properties</span></span>

| <span data-ttu-id="4aa9a-109">属性</span><span class="sxs-lookup"><span data-stu-id="4aa9a-109">Property</span></span>                    | <span data-ttu-id="4aa9a-110">类型</span><span class="sxs-lookup"><span data-stu-id="4aa9a-110">Type</span></span>                                                                     | <span data-ttu-id="4aa9a-111">说明</span><span class="sxs-lookup"><span data-stu-id="4aa9a-111">Description</span></span>                                                                                                                                                                                       |
| :-------------------------- | :----------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="4aa9a-112">actionSource</span><span class="sxs-lookup"><span data-stu-id="4aa9a-112">actionSource</span></span>                | <span data-ttu-id="4aa9a-113">String</span><span class="sxs-lookup"><span data-stu-id="4aa9a-113">String</span></span>                                                                   | <span data-ttu-id="4aa9a-114">可能的值是：`manual`、`automatic`、`recommended`、`default`。</span><span class="sxs-lookup"><span data-stu-id="4aa9a-114">Possible values are: `manual`, `automatic`, `recommended`, `default`.</span></span>                                                                                                                             |
| <span data-ttu-id="4aa9a-115">actions</span><span class="sxs-lookup"><span data-stu-id="4aa9a-115">actions</span></span>                     | <span data-ttu-id="4aa9a-116">[informationProtectionAction](informationprotectionaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4aa9a-116">[informationProtectionAction](informationprotectionaction.md) collection</span></span> | <span data-ttu-id="4aa9a-117">使用应用程序为文档添加标签时应执行的特定操作的集合。</span><span class="sxs-lookup"><span data-stu-id="4aa9a-117">The collection of specific actions that should be taken by the consuming application to label the document.</span></span> <span data-ttu-id="4aa9a-118">有关[完整列表，请参阅 informationProtectionAction。](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="4aa9a-118">See  [informationProtectionAction](informationprotectionaction.md) for the full list.</span></span> |
| <span data-ttu-id="4aa9a-119">label</span><span class="sxs-lookup"><span data-stu-id="4aa9a-119">label</span></span>                       | [<span data-ttu-id="4aa9a-120">labelDetails</span><span class="sxs-lookup"><span data-stu-id="4aa9a-120">labelDetails</span></span>](labeldetails.md)                                          | <span data-ttu-id="4aa9a-121">描述要应用的标签的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="4aa9a-121">Object that describes the details of the label to apply.</span></span>                                                                                                                                          |
| <span data-ttu-id="4aa9a-122">responsibleSensitiveTypeIds</span><span class="sxs-lookup"><span data-stu-id="4aa9a-122">responsibleSensitiveTypeIds</span></span> | <span data-ttu-id="4aa9a-123">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="4aa9a-123">Guid collection</span></span>                                                          | <span data-ttu-id="4aa9a-124">如果标签是自动分类的结果，则提供导致返回标签的敏感信息类型 GUID 列表。</span><span class="sxs-lookup"><span data-stu-id="4aa9a-124">If the label was the result of an automatic classification, supply the list of sensitive info type GUIDs that resulted in the returned label.</span></span>                                         
## <a name="json-representation"></a><span data-ttu-id="4aa9a-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4aa9a-125">JSON representation</span></span>

<span data-ttu-id="4aa9a-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4aa9a-126">The following is a JSON representation of the resource.</span></span>

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

