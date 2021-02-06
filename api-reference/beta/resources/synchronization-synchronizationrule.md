---
title: synchronizationRule 资源类型
description: 定义如何对同步引擎执行同步。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 94697fede9ab9055b1a477cfd94edea88f207331
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135994"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="3fc94-103">synchronizationRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="3fc94-103">synchronizationRule resource type</span></span>

<span data-ttu-id="3fc94-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fc94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fc94-105">定义应为同步引擎执行同步的方式，包括要同步的对象以及方向、源目录中的对象如何与目标目录中的对象匹配，以及属性从源目录同步到目标目录时如何转换属性。</span><span class="sxs-lookup"><span data-stu-id="3fc94-105">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="3fc94-106">**注意：** 同步规则在一个方向定义同步 - 从源目录到目标目录。</span><span class="sxs-lookup"><span data-stu-id="3fc94-106">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="3fc94-107">源目录和目标目录定义为规则属性的一部分。</span><span class="sxs-lookup"><span data-stu-id="3fc94-107">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="3fc94-108">同步规则作为同步架构的一 [部分进行更新](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="3fc94-108">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3fc94-109">属性</span><span class="sxs-lookup"><span data-stu-id="3fc94-109">Properties</span></span>

| <span data-ttu-id="3fc94-110">属性</span><span class="sxs-lookup"><span data-stu-id="3fc94-110">Property</span></span>      | <span data-ttu-id="3fc94-111">类型</span><span class="sxs-lookup"><span data-stu-id="3fc94-111">Type</span></span>      | <span data-ttu-id="3fc94-112">说明</span><span class="sxs-lookup"><span data-stu-id="3fc94-112">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="3fc94-113">可编辑</span><span class="sxs-lookup"><span data-stu-id="3fc94-113">editable</span></span>       |<span data-ttu-id="3fc94-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fc94-114">Boolean</span></span>    |<span data-ttu-id="3fc94-115">`true` 同步规则是否可自定义; `false` 如果此规则是只读的且不应更改。</span><span class="sxs-lookup"><span data-stu-id="3fc94-115">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="3fc94-116">id</span><span class="sxs-lookup"><span data-stu-id="3fc94-116">id</span></span>             |<span data-ttu-id="3fc94-117">字符串</span><span class="sxs-lookup"><span data-stu-id="3fc94-117">String</span></span>     |<span data-ttu-id="3fc94-118">同步规则标识符。</span><span class="sxs-lookup"><span data-stu-id="3fc94-118">Synchronization rule identifier.</span></span> <span data-ttu-id="3fc94-119">必须是同步引擎识别的标识符之一。</span><span class="sxs-lookup"><span data-stu-id="3fc94-119">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="3fc94-120">可以在 API 返回的同步模板中找到受支持的规则标识符。</span><span class="sxs-lookup"><span data-stu-id="3fc94-120">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="3fc94-121">metadata</span><span class="sxs-lookup"><span data-stu-id="3fc94-121">metadata</span></span>       |<span data-ttu-id="3fc94-122">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3fc94-122">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="3fc94-123">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3fc94-123">Additional extension properties.</span></span> <span data-ttu-id="3fc94-124">除非支持团队明确指示，否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="3fc94-124">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="3fc94-125">name</span><span class="sxs-lookup"><span data-stu-id="3fc94-125">name</span></span>           |<span data-ttu-id="3fc94-126">字符串</span><span class="sxs-lookup"><span data-stu-id="3fc94-126">String</span></span>     |<span data-ttu-id="3fc94-127">同步规则的可读名称。</span><span class="sxs-lookup"><span data-stu-id="3fc94-127">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="3fc94-128">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="3fc94-128">Not nullable.</span></span>|
|<span data-ttu-id="3fc94-129">objectMappings</span><span class="sxs-lookup"><span data-stu-id="3fc94-129">objectMappings</span></span> |<span data-ttu-id="3fc94-130">[objectMapping](synchronization-objectmapping.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3fc94-130">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="3fc94-131">规则支持的对象映射的集合。</span><span class="sxs-lookup"><span data-stu-id="3fc94-131">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="3fc94-132">告知同步引擎应同步哪些对象。</span><span class="sxs-lookup"><span data-stu-id="3fc94-132">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="3fc94-133">priority</span><span class="sxs-lookup"><span data-stu-id="3fc94-133">priority</span></span>       |<span data-ttu-id="3fc94-134">整数</span><span class="sxs-lookup"><span data-stu-id="3fc94-134">Integer</span></span>    |<span data-ttu-id="3fc94-135">相对于 [synchronizationSchema](synchronization-synchronizationschema.md)中其他规则的优先级。</span><span class="sxs-lookup"><span data-stu-id="3fc94-135">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="3fc94-136">优先级最低的规则将首先进行处理。</span><span class="sxs-lookup"><span data-stu-id="3fc94-136">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="3fc94-137">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="3fc94-137">sourceDirectoryName</span></span>       |<span data-ttu-id="3fc94-138">字符串</span><span class="sxs-lookup"><span data-stu-id="3fc94-138">String</span></span>    |<span data-ttu-id="3fc94-139">源目录的名称。</span><span class="sxs-lookup"><span data-stu-id="3fc94-139">Name of the source directory.</span></span> <span data-ttu-id="3fc94-140">必须与 synchronizationSchema 中的目录定义 [之一匹配](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="3fc94-140">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="3fc94-141">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="3fc94-141">targetDirectoryName</span></span>       |<span data-ttu-id="3fc94-142">字符串</span><span class="sxs-lookup"><span data-stu-id="3fc94-142">String</span></span>    |<span data-ttu-id="3fc94-143">目标目录的名称。</span><span class="sxs-lookup"><span data-stu-id="3fc94-143">Name of the target directory.</span></span> <span data-ttu-id="3fc94-144">必须与 synchronizationSchema 中的目录定义 [之一匹配](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="3fc94-144">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3fc94-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3fc94-145">JSON representation</span></span>

<span data-ttu-id="3fc94-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3fc94-146">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationRule"
}-->

```json
{
  "editable": true,
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objectMappings": [{"@odata.type": "microsoft.graph.objectMapping"}],
  "priority": 1024,
  "sourceDirectoryName": "String",
  "targetDirectoryName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


