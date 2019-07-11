---
title: synchronizationRule 资源类型
description: 定义同步引擎的同步执行方式, 包括要同步的对象和在哪个方向上, 源目录中的对象应与目标目录中的对象匹配, 以及属性应在将其从源目录同步到目标目录时进行转换。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 83bb8751a60197b8afd9132618ba994c33f370c8
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620708"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="c9607-103">synchronizationRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9607-103">synchronizationRule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9607-104">定义同步引擎的同步执行方式, 包括要同步的对象和在哪个方向上, 源目录中的对象应与目标目录中的对象匹配, 以及属性应在将其从源目录同步到目标目录时进行转换。</span><span class="sxs-lookup"><span data-stu-id="c9607-104">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="c9607-105">**注意:** 同步规则将一个方向的同步定义为将源目录中的同步到目标目录。</span><span class="sxs-lookup"><span data-stu-id="c9607-105">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="c9607-106">源和目标目录定义为规则属性的一部分。</span><span class="sxs-lookup"><span data-stu-id="c9607-106">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="c9607-107">同步规则将作为[同步架构](synchronization-synchronizationschema.md)的一部分进行更新。</span><span class="sxs-lookup"><span data-stu-id="c9607-107">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c9607-108">属性</span><span class="sxs-lookup"><span data-stu-id="c9607-108">Properties</span></span>

| <span data-ttu-id="c9607-109">属性</span><span class="sxs-lookup"><span data-stu-id="c9607-109">Property</span></span>      | <span data-ttu-id="c9607-110">类型</span><span class="sxs-lookup"><span data-stu-id="c9607-110">Type</span></span>      | <span data-ttu-id="c9607-111">说明</span><span class="sxs-lookup"><span data-stu-id="c9607-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="c9607-112">变为</span><span class="sxs-lookup"><span data-stu-id="c9607-112">editable</span></span>       |<span data-ttu-id="c9607-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9607-113">Boolean</span></span>    |<span data-ttu-id="c9607-114">`true`如果可以对同步规则进行自定义, 则为  ;`false`如果此规则为只读, 则不应更改。</span><span class="sxs-lookup"><span data-stu-id="c9607-114">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="c9607-115">id</span><span class="sxs-lookup"><span data-stu-id="c9607-115">id</span></span>             |<span data-ttu-id="c9607-116">String</span><span class="sxs-lookup"><span data-stu-id="c9607-116">String</span></span>     |<span data-ttu-id="c9607-117">同步规则标识符。</span><span class="sxs-lookup"><span data-stu-id="c9607-117">Synchronization rule identifier.</span></span> <span data-ttu-id="c9607-118">必须是同步引擎可识别的标识符之一。</span><span class="sxs-lookup"><span data-stu-id="c9607-118">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="c9607-119">在 API 返回的同步模板中可以找到受支持的规则标识符。</span><span class="sxs-lookup"><span data-stu-id="c9607-119">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="c9607-120">metadata</span><span class="sxs-lookup"><span data-stu-id="c9607-120">metadata</span></span>       |<span data-ttu-id="c9607-121">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="c9607-121">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="c9607-122">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c9607-122">Additional extension properties.</span></span> <span data-ttu-id="c9607-123">除非支持团队明确指示, 否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="c9607-123">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="c9607-124">name</span><span class="sxs-lookup"><span data-stu-id="c9607-124">name</span></span>           |<span data-ttu-id="c9607-125">String</span><span class="sxs-lookup"><span data-stu-id="c9607-125">String</span></span>     |<span data-ttu-id="c9607-126">可读的同步规则名称。</span><span class="sxs-lookup"><span data-stu-id="c9607-126">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="c9607-127">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="c9607-127">Not nullable.</span></span>|
|<span data-ttu-id="c9607-128">objectMappings</span><span class="sxs-lookup"><span data-stu-id="c9607-128">objectMappings</span></span> |<span data-ttu-id="c9607-129">[objectMapping](synchronization-objectmapping.md)集合</span><span class="sxs-lookup"><span data-stu-id="c9607-129">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="c9607-130">该规则支持的对象映射的集合。</span><span class="sxs-lookup"><span data-stu-id="c9607-130">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="c9607-131">通知同步引擎应同步哪些对象。</span><span class="sxs-lookup"><span data-stu-id="c9607-131">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="c9607-132">priority</span><span class="sxs-lookup"><span data-stu-id="c9607-132">priority</span></span>       |<span data-ttu-id="c9607-133">整数</span><span class="sxs-lookup"><span data-stu-id="c9607-133">Integer</span></span>    |<span data-ttu-id="c9607-134">相对于[synchronizationSchema](synchronization-synchronizationschema.md)中其他规则的优先级。</span><span class="sxs-lookup"><span data-stu-id="c9607-134">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="c9607-135">将首先处理具有最低优先级编号的规则。</span><span class="sxs-lookup"><span data-stu-id="c9607-135">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="c9607-136">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="c9607-136">sourceDirectoryName</span></span>       |<span data-ttu-id="c9607-137">String</span><span class="sxs-lookup"><span data-stu-id="c9607-137">String</span></span>    |<span data-ttu-id="c9607-138">源目录的名称。</span><span class="sxs-lookup"><span data-stu-id="c9607-138">Name of the source directory.</span></span> <span data-ttu-id="c9607-139">必须与[synchronizationSchema](synchronization-synchronizationschema.md)中的一个目录定义相匹配。</span><span class="sxs-lookup"><span data-stu-id="c9607-139">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="c9607-140">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="c9607-140">targetDirectoryName</span></span>       |<span data-ttu-id="c9607-141">String</span><span class="sxs-lookup"><span data-stu-id="c9607-141">String</span></span>    |<span data-ttu-id="c9607-142">目标目录的名称。</span><span class="sxs-lookup"><span data-stu-id="c9607-142">Name of the target directory.</span></span> <span data-ttu-id="c9607-143">必须与[synchronizationSchema](synchronization-synchronizationschema.md)中的一个目录定义相匹配。</span><span class="sxs-lookup"><span data-stu-id="c9607-143">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9607-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9607-144">JSON representation</span></span>

<span data-ttu-id="c9607-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9607-145">The following is a JSON representation of the resource.</span></span>

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
