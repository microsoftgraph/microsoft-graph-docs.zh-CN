---
title: synchronizationRule 资源类型
description: 定义同步引擎，包括要同步的对象和方向，应如何执行同步如何从源目录对象应匹配目标目录中的对象以及如何属性应转换他们正在同步时从源到目标目录。
ms.openlocfilehash: c860228637a6cc3ad9137851408379bd7f779c75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043410"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="43983-103">synchronizationRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="43983-103">synchronizationRule resource type</span></span>

> <span data-ttu-id="43983-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="43983-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43983-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="43983-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="43983-106">定义同步引擎，包括要同步的对象和方向，应如何执行同步如何从源目录对象应匹配目标目录中的对象以及如何属性应转换他们正在同步时从源到目标目录。</span><span class="sxs-lookup"><span data-stu-id="43983-106">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="43983-107">**注意：** 同步规则定义一个方向-从到目标目录源目录同步。</span><span class="sxs-lookup"><span data-stu-id="43983-107">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="43983-108">规则属性的一部分定义的源和目标目录。</span><span class="sxs-lookup"><span data-stu-id="43983-108">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="43983-109">同步规则更新[同步架构](synchronization-synchronizationschema.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="43983-109">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="43983-110">属性</span><span class="sxs-lookup"><span data-stu-id="43983-110">Properties</span></span>

| <span data-ttu-id="43983-111">属性</span><span class="sxs-lookup"><span data-stu-id="43983-111">Property</span></span>      | <span data-ttu-id="43983-112">类型</span><span class="sxs-lookup"><span data-stu-id="43983-112">Type</span></span>      | <span data-ttu-id="43983-113">说明</span><span class="sxs-lookup"><span data-stu-id="43983-113">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="43983-114">可编辑</span><span class="sxs-lookup"><span data-stu-id="43983-114">editable</span></span>       |<span data-ttu-id="43983-115">布尔</span><span class="sxs-lookup"><span data-stu-id="43983-115">Boolean</span></span>    |<span data-ttu-id="43983-116">`true`如果可以自定义同步规则;，`false`如果此规则是只读的并且不应被更改。</span><span class="sxs-lookup"><span data-stu-id="43983-116">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="43983-117">id</span><span class="sxs-lookup"><span data-stu-id="43983-117">id</span></span>             |<span data-ttu-id="43983-118">字符串</span><span class="sxs-lookup"><span data-stu-id="43983-118">String</span></span>     |<span data-ttu-id="43983-119">同步规则标识符。</span><span class="sxs-lookup"><span data-stu-id="43983-119">Synchronization rule identifier.</span></span> <span data-ttu-id="43983-120">必须是同步引擎识别的标识符。</span><span class="sxs-lookup"><span data-stu-id="43983-120">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="43983-121">支持标识符可以找到 API 返回的同步模板中的规则。</span><span class="sxs-lookup"><span data-stu-id="43983-121">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="43983-122">元数据</span><span class="sxs-lookup"><span data-stu-id="43983-122">metadata</span></span>       |<span data-ttu-id="43983-123">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="43983-123">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="43983-124">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="43983-124">Additional extension properties.</span></span> <span data-ttu-id="43983-125">除非明确由支持团队，不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="43983-125">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="43983-126">name</span><span class="sxs-lookup"><span data-stu-id="43983-126">name</span></span>           |<span data-ttu-id="43983-127">字符串</span><span class="sxs-lookup"><span data-stu-id="43983-127">String</span></span>     |<span data-ttu-id="43983-128">可读同步规则的名称。</span><span class="sxs-lookup"><span data-stu-id="43983-128">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="43983-129">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="43983-129">Not nullable.</span></span>|
|<span data-ttu-id="43983-130">objectMappings</span><span class="sxs-lookup"><span data-stu-id="43983-130">objectMappings</span></span> |<span data-ttu-id="43983-131">[objectMapping](synchronization-objectmapping.md)集合</span><span class="sxs-lookup"><span data-stu-id="43983-131">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="43983-132">规则支持的对象映射的集合。</span><span class="sxs-lookup"><span data-stu-id="43983-132">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="43983-133">指示同步引擎应同步的对象。</span><span class="sxs-lookup"><span data-stu-id="43983-133">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="43983-134">priority</span><span class="sxs-lookup"><span data-stu-id="43983-134">priority</span></span>       |<span data-ttu-id="43983-135">整数</span><span class="sxs-lookup"><span data-stu-id="43983-135">Integer</span></span>    |<span data-ttu-id="43983-136">相对于[synchronizationSchema](synchronization-synchronizationschema.md)中其他规则的优先级。</span><span class="sxs-lookup"><span data-stu-id="43983-136">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="43983-137">将首先处理与最低优先级编号的规则。</span><span class="sxs-lookup"><span data-stu-id="43983-137">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="43983-138">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="43983-138">sourceDirectoryName</span></span>       |<span data-ttu-id="43983-139">字符串</span><span class="sxs-lookup"><span data-stu-id="43983-139">String</span></span>    |<span data-ttu-id="43983-140">源目录的名称。</span><span class="sxs-lookup"><span data-stu-id="43983-140">Name of the source directory.</span></span> <span data-ttu-id="43983-141">必须匹配[synchronizationSchema](synchronization-synchronizationschema.md)中的目录定义之一。</span><span class="sxs-lookup"><span data-stu-id="43983-141">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="43983-142">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="43983-142">targetDirectoryName</span></span>       |<span data-ttu-id="43983-143">字符串</span><span class="sxs-lookup"><span data-stu-id="43983-143">String</span></span>    |<span data-ttu-id="43983-144">目标目录的名称。</span><span class="sxs-lookup"><span data-stu-id="43983-144">Name of the target directory.</span></span> <span data-ttu-id="43983-145">必须匹配[synchronizationSchema](synchronization-synchronizationschema.md)中的目录定义之一。</span><span class="sxs-lookup"><span data-stu-id="43983-145">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43983-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43983-146">JSON representation</span></span>

<span data-ttu-id="43983-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43983-147">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->