---
title: attributeMapping 资源类型
description: 定义同步过程中流给定的目标属性的值应如何。
ms.openlocfilehash: e4fd8ba0aece448f358d51373dfca0157759a23e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044844"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="b1a0c-103">attributeMapping 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1a0c-103">attributeMapping resource type</span></span>

> <span data-ttu-id="b1a0c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1a0c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1a0c-106">定义同步过程中流给定的目标属性的值应如何。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-106">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="b1a0c-107">属性</span><span class="sxs-lookup"><span data-stu-id="b1a0c-107">Properties</span></span>

| <span data-ttu-id="b1a0c-108">属性</span><span class="sxs-lookup"><span data-stu-id="b1a0c-108">Property</span></span>                  | <span data-ttu-id="b1a0c-109">类型</span><span class="sxs-lookup"><span data-stu-id="b1a0c-109">Type</span></span>                      | <span data-ttu-id="b1a0c-110">说明</span><span class="sxs-lookup"><span data-stu-id="b1a0c-110">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="b1a0c-111">defaultValue</span><span class="sxs-lookup"><span data-stu-id="b1a0c-111">defaultValue</span></span>               | <span data-ttu-id="b1a0c-112">字符串</span><span class="sxs-lookup"><span data-stu-id="b1a0c-112">String</span></span>                    |<span data-ttu-id="b1a0c-113">默认值用于以防**source**属性计算结果为`null`。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-113">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="b1a0c-114">可选。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-114">Optional.</span></span>|
|<span data-ttu-id="b1a0c-115">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="b1a0c-115">exportMissingReferences</span></span>    |<span data-ttu-id="b1a0c-116">字符串</span><span class="sxs-lookup"><span data-stu-id="b1a0c-116">String</span></span>                     |<span data-ttu-id="b1a0c-117">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-117">For internal use only.</span></span>|
|<span data-ttu-id="b1a0c-118">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="b1a0c-118">flowBehavior</span></span>               |<span data-ttu-id="b1a0c-119">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="b1a0c-119">attributeFlowBehavior</span></span>      |<span data-ttu-id="b1a0c-120">定义此属性时应可导出到目标目录。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-120">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="b1a0c-121">可能的值为：`FlowWhenChanged`和`FlowAlways`。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-121">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="b1a0c-122">默认值为 `FlowWhenChanged`。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-122">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="b1a0c-123">flowType</span><span class="sxs-lookup"><span data-stu-id="b1a0c-123">flowType</span></span>                   |<span data-ttu-id="b1a0c-124">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="b1a0c-124">attributeFlowType</span></span>          |<span data-ttu-id="b1a0c-125">定义此属性时应更新目标目录中。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-125">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="b1a0c-126">可能的值为： `Always` （默认）， `ObjectAddOnly` （仅当创建新对象）， `MultiValueAddOnly` （仅当更改正在添加新值到多值属性）。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-126">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="b1a0c-127">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="b1a0c-127">matchingPriority</span></span>           |<span data-ttu-id="b1a0c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b1a0c-128">Int32</span></span>                      |<span data-ttu-id="b1a0c-129">如果大于 0，则此属性将用于执行源和目标目录之间的对象的初始匹配。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-129">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="b1a0c-130">同步引擎将尝试查找匹配对象属性使用的第一次匹配优先级最低值。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-130">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="b1a0c-131">如果找不到下, 一匹配 priority 属性将使用，依此类推直到找到匹配项，或没有匹配属性会保留。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-131">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="b1a0c-132">仅对于预计具有唯一的值，如电子邮件、 属性应用作匹配的属性。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-132">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="b1a0c-133">源</span><span class="sxs-lookup"><span data-stu-id="b1a0c-133">source</span></span>                     |[<span data-ttu-id="b1a0c-134">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="b1a0c-134">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="b1a0c-135">定义如何值应为源对象中提取 （或转换）。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-135">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="b1a0c-136">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="b1a0c-136">targetAttributeName</span></span>        |<span data-ttu-id="b1a0c-137">字符串</span><span class="sxs-lookup"><span data-stu-id="b1a0c-137">String</span></span>                     |<span data-ttu-id="b1a0c-138">对目标对象的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-138">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b1a0c-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1a0c-139">JSON representation</span></span>

<span data-ttu-id="b1a0c-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1a0c-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMapping"
}-->

```json
{
  "defaultValue": "String",
  "exportMissingReferences": true,
  "flowBehavior": "String",
  "flowType": "String",
  "matchingPriority": 1024,
  "source": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "targetAttributeName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->