---
title: attributeMapping 资源类型
description: 定义如何在同步过程中传递给定目标属性的值。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1f2884a4fc9f4e3091f1e7523c615d9ed132abc6
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621388"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="57205-103">attributeMapping 资源类型</span><span class="sxs-lookup"><span data-stu-id="57205-103">attributeMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57205-104">定义如何在同步过程中传递给定目标属性的值。</span><span class="sxs-lookup"><span data-stu-id="57205-104">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="57205-105">属性</span><span class="sxs-lookup"><span data-stu-id="57205-105">Properties</span></span>

| <span data-ttu-id="57205-106">属性</span><span class="sxs-lookup"><span data-stu-id="57205-106">Property</span></span>                  | <span data-ttu-id="57205-107">类型</span><span class="sxs-lookup"><span data-stu-id="57205-107">Type</span></span>                      | <span data-ttu-id="57205-108">说明</span><span class="sxs-lookup"><span data-stu-id="57205-108">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="57205-109">默认</span><span class="sxs-lookup"><span data-stu-id="57205-109">defaultValue</span></span>               | <span data-ttu-id="57205-110">String</span><span class="sxs-lookup"><span data-stu-id="57205-110">String</span></span>                    |<span data-ttu-id="57205-111">要在对`null`**源**属性进行求值的情况下使用的默认值。</span><span class="sxs-lookup"><span data-stu-id="57205-111">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="57205-112">可选。</span><span class="sxs-lookup"><span data-stu-id="57205-112">Optional.</span></span>|
|<span data-ttu-id="57205-113">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="57205-113">exportMissingReferences</span></span>    |<span data-ttu-id="57205-114">String</span><span class="sxs-lookup"><span data-stu-id="57205-114">String</span></span>                     |<span data-ttu-id="57205-115">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="57205-115">For internal use only.</span></span>|
|<span data-ttu-id="57205-116">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="57205-116">flowBehavior</span></span>               |<span data-ttu-id="57205-117">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="57205-117">attributeFlowBehavior</span></span>      |<span data-ttu-id="57205-118">定义何时应将此属性导出到目标目录。</span><span class="sxs-lookup"><span data-stu-id="57205-118">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="57205-119">可能的值为`FlowWhenChanged` : `FlowAlways`和。</span><span class="sxs-lookup"><span data-stu-id="57205-119">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="57205-120">默认值为 `FlowWhenChanged`。</span><span class="sxs-lookup"><span data-stu-id="57205-120">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="57205-121">flowType</span><span class="sxs-lookup"><span data-stu-id="57205-121">flowType</span></span>                   |<span data-ttu-id="57205-122">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="57205-122">attributeFlowType</span></span>          |<span data-ttu-id="57205-123">定义应何时在目标目录中更新此属性。</span><span class="sxs-lookup"><span data-stu-id="57205-123">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="57205-124">可能的值为`Always` : (默认值`ObjectAddOnly` ), (仅在创建新对象时`MultiValueAddOnly` ) (仅当更改将新值添加到多值属性时)。</span><span class="sxs-lookup"><span data-stu-id="57205-124">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="57205-125">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="57205-125">matchingPriority</span></span>           |<span data-ttu-id="57205-126">Int32</span><span class="sxs-lookup"><span data-stu-id="57205-126">Int32</span></span>                      |<span data-ttu-id="57205-127">如果高于 0, 则此属性将用于执行源目录和目标目录之间的对象的初始匹配。</span><span class="sxs-lookup"><span data-stu-id="57205-127">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="57205-128">同步引擎将尝试使用具有最小匹配优先级值的属性来查找匹配的对象。</span><span class="sxs-lookup"><span data-stu-id="57205-128">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="57205-129">如果未找到, 则将使用具有下一个匹配的优先级的属性, 在找到匹配项或不留下更多匹配属性的情况下, 将使用该属性。</span><span class="sxs-lookup"><span data-stu-id="57205-129">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="57205-130">应仅将应具有唯一值的属性 (如电子邮件) 用作匹配属性。</span><span class="sxs-lookup"><span data-stu-id="57205-130">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="57205-131">source</span><span class="sxs-lookup"><span data-stu-id="57205-131">source</span></span>                     |[<span data-ttu-id="57205-132">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="57205-132">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="57205-133">定义应如何从源对象提取 (或转换) 值。</span><span class="sxs-lookup"><span data-stu-id="57205-133">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="57205-134">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="57205-134">targetAttributeName</span></span>        |<span data-ttu-id="57205-135">String</span><span class="sxs-lookup"><span data-stu-id="57205-135">String</span></span>                     |<span data-ttu-id="57205-136">目标对象上的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="57205-136">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="57205-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57205-137">JSON representation</span></span>

<span data-ttu-id="57205-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57205-138">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
