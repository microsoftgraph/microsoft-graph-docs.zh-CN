---
title: synchronizationRule 资源类型
description: 定义同步引擎应如何执行同步。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 86a5f39612b6fdbeb123a74372520115e0357fb0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023812"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="be627-103">synchronizationRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="be627-103">synchronizationRule resource type</span></span>

<span data-ttu-id="be627-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be627-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be627-105">定义同步引擎的同步执行方式，包括要同步的对象和方向、源目录中的对象与目标目录中的对象的匹配方式以及在从源同步到目标目录时应如何转换属性。</span><span class="sxs-lookup"><span data-stu-id="be627-105">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="be627-106">**注意：** 同步规则将一个方向的同步定义为将源目录中的同步到目标目录。</span><span class="sxs-lookup"><span data-stu-id="be627-106">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="be627-107">源和目标目录定义为规则属性的一部分。</span><span class="sxs-lookup"><span data-stu-id="be627-107">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="be627-108">同步规则将作为 [同步架构](synchronization-synchronizationschema.md)的一部分进行更新。</span><span class="sxs-lookup"><span data-stu-id="be627-108">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="be627-109">属性</span><span class="sxs-lookup"><span data-stu-id="be627-109">Properties</span></span>

| <span data-ttu-id="be627-110">属性</span><span class="sxs-lookup"><span data-stu-id="be627-110">Property</span></span>      | <span data-ttu-id="be627-111">类型</span><span class="sxs-lookup"><span data-stu-id="be627-111">Type</span></span>      | <span data-ttu-id="be627-112">说明</span><span class="sxs-lookup"><span data-stu-id="be627-112">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="be627-113">变为</span><span class="sxs-lookup"><span data-stu-id="be627-113">editable</span></span>       |<span data-ttu-id="be627-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="be627-114">Boolean</span></span>    |<span data-ttu-id="be627-115">`true` 如果可以对同步规则进行自定义，则为  ; `false` 如果此规则为只读，则不应更改。</span><span class="sxs-lookup"><span data-stu-id="be627-115">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="be627-116">id</span><span class="sxs-lookup"><span data-stu-id="be627-116">id</span></span>             |<span data-ttu-id="be627-117">String</span><span class="sxs-lookup"><span data-stu-id="be627-117">String</span></span>     |<span data-ttu-id="be627-118">同步规则标识符。</span><span class="sxs-lookup"><span data-stu-id="be627-118">Synchronization rule identifier.</span></span> <span data-ttu-id="be627-119">必须是同步引擎可识别的标识符之一。</span><span class="sxs-lookup"><span data-stu-id="be627-119">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="be627-120">在 API 返回的同步模板中可以找到受支持的规则标识符。</span><span class="sxs-lookup"><span data-stu-id="be627-120">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="be627-121">metadata</span><span class="sxs-lookup"><span data-stu-id="be627-121">metadata</span></span>       |<span data-ttu-id="be627-122">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be627-122">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="be627-123">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="be627-123">Additional extension properties.</span></span> <span data-ttu-id="be627-124">除非支持团队明确指示，否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="be627-124">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="be627-125">name</span><span class="sxs-lookup"><span data-stu-id="be627-125">name</span></span>           |<span data-ttu-id="be627-126">String</span><span class="sxs-lookup"><span data-stu-id="be627-126">String</span></span>     |<span data-ttu-id="be627-127">可读的同步规则名称。</span><span class="sxs-lookup"><span data-stu-id="be627-127">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="be627-128">不可为空。</span><span class="sxs-lookup"><span data-stu-id="be627-128">Not nullable.</span></span>|
|<span data-ttu-id="be627-129">objectMappings</span><span class="sxs-lookup"><span data-stu-id="be627-129">objectMappings</span></span> |<span data-ttu-id="be627-130">[objectMapping](synchronization-objectmapping.md) 集合</span><span class="sxs-lookup"><span data-stu-id="be627-130">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="be627-131">该规则支持的对象映射的集合。</span><span class="sxs-lookup"><span data-stu-id="be627-131">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="be627-132">通知同步引擎应同步哪些对象。</span><span class="sxs-lookup"><span data-stu-id="be627-132">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="be627-133">priority</span><span class="sxs-lookup"><span data-stu-id="be627-133">priority</span></span>       |<span data-ttu-id="be627-134">整数</span><span class="sxs-lookup"><span data-stu-id="be627-134">Integer</span></span>    |<span data-ttu-id="be627-135">相对于 [synchronizationSchema](synchronization-synchronizationschema.md)中其他规则的优先级。</span><span class="sxs-lookup"><span data-stu-id="be627-135">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="be627-136">将首先处理具有最低优先级编号的规则。</span><span class="sxs-lookup"><span data-stu-id="be627-136">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="be627-137">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="be627-137">sourceDirectoryName</span></span>       |<span data-ttu-id="be627-138">String</span><span class="sxs-lookup"><span data-stu-id="be627-138">String</span></span>    |<span data-ttu-id="be627-139">源目录的名称。</span><span class="sxs-lookup"><span data-stu-id="be627-139">Name of the source directory.</span></span> <span data-ttu-id="be627-140">必须与 [synchronizationSchema](synchronization-synchronizationschema.md)中的一个目录定义相匹配。</span><span class="sxs-lookup"><span data-stu-id="be627-140">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="be627-141">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="be627-141">targetDirectoryName</span></span>       |<span data-ttu-id="be627-142">String</span><span class="sxs-lookup"><span data-stu-id="be627-142">String</span></span>    |<span data-ttu-id="be627-143">目标目录的名称。</span><span class="sxs-lookup"><span data-stu-id="be627-143">Name of the target directory.</span></span> <span data-ttu-id="be627-144">必须与 [synchronizationSchema](synchronization-synchronizationschema.md)中的一个目录定义相匹配。</span><span class="sxs-lookup"><span data-stu-id="be627-144">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be627-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be627-145">JSON representation</span></span>

<span data-ttu-id="be627-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be627-146">The following is a JSON representation of the resource.</span></span>

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


