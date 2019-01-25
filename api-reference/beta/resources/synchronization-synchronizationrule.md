---
title: synchronizationRule 资源类型
description: 定义同步引擎，包括要同步的对象和方向，应如何执行同步如何从源目录对象应匹配目标目录中的对象以及如何属性应转换他们正在同步时从源到目标目录。
localization_priority: Normal
ms.openlocfilehash: deaf27ec46268eebe289e502bdf3b62a659cf1fb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517923"
---
# <a name="synchronizationrule-resource-type"></a><span data-ttu-id="c9868-103">synchronizationRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9868-103">synchronizationRule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9868-104">定义同步引擎，包括要同步的对象和方向，应如何执行同步如何从源目录对象应匹配目标目录中的对象以及如何属性应转换他们正在同步时从源到目标目录。</span><span class="sxs-lookup"><span data-stu-id="c9868-104">Defines how the synchronization should be performed for the synchronization engine, including which objects to synchronize and in which direction, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

><span data-ttu-id="c9868-105">**注意：** 同步规则定义一个方向-从到目标目录源目录同步。</span><span class="sxs-lookup"><span data-stu-id="c9868-105">**Note:** Synchronization rules define synchronization in one direction - from the source directory to the target directory.</span></span> <span data-ttu-id="c9868-106">规则属性的一部分定义的源和目标目录。</span><span class="sxs-lookup"><span data-stu-id="c9868-106">The source and target directories are defined as part of the rule properties.</span></span>

<span data-ttu-id="c9868-107">同步规则更新[同步架构](synchronization-synchronizationschema.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="c9868-107">Synchronization rules are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c9868-108">属性</span><span class="sxs-lookup"><span data-stu-id="c9868-108">Properties</span></span>

| <span data-ttu-id="c9868-109">属性</span><span class="sxs-lookup"><span data-stu-id="c9868-109">Property</span></span>      | <span data-ttu-id="c9868-110">类型</span><span class="sxs-lookup"><span data-stu-id="c9868-110">Type</span></span>      | <span data-ttu-id="c9868-111">说明</span><span class="sxs-lookup"><span data-stu-id="c9868-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="c9868-112">可编辑</span><span class="sxs-lookup"><span data-stu-id="c9868-112">editable</span></span>       |<span data-ttu-id="c9868-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9868-113">Boolean</span></span>    |<span data-ttu-id="c9868-114">`true`如果可以自定义同步规则;，`false`如果此规则是只读的并且不应被更改。</span><span class="sxs-lookup"><span data-stu-id="c9868-114">`true` if the synchronization rule can be customized; `false` if this rule is read-only and should not be changed.</span></span>|
|<span data-ttu-id="c9868-115">id</span><span class="sxs-lookup"><span data-stu-id="c9868-115">id</span></span>             |<span data-ttu-id="c9868-116">String</span><span class="sxs-lookup"><span data-stu-id="c9868-116">String</span></span>     |<span data-ttu-id="c9868-117">同步规则标识符。</span><span class="sxs-lookup"><span data-stu-id="c9868-117">Synchronization rule identifier.</span></span> <span data-ttu-id="c9868-118">必须是同步引擎识别的标识符。</span><span class="sxs-lookup"><span data-stu-id="c9868-118">Must be one of the identifiers recognized by the synchronization engine.</span></span> <span data-ttu-id="c9868-119">支持标识符可以找到 API 返回的同步模板中的规则。</span><span class="sxs-lookup"><span data-stu-id="c9868-119">Supported rule identifiers can be found in the synchronization template returned by the API.</span></span>|
|<span data-ttu-id="c9868-120">元数据</span><span class="sxs-lookup"><span data-stu-id="c9868-120">metadata</span></span>       |<span data-ttu-id="c9868-121">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="c9868-121">[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) collection</span></span> |<span data-ttu-id="c9868-122">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c9868-122">Additional extension properties.</span></span> <span data-ttu-id="c9868-123">除非明确由支持团队，不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="c9868-123">Unless instructed explicitly by the support team, metadata values should not be changed.</span></span>|
|<span data-ttu-id="c9868-124">name</span><span class="sxs-lookup"><span data-stu-id="c9868-124">name</span></span>           |<span data-ttu-id="c9868-125">String</span><span class="sxs-lookup"><span data-stu-id="c9868-125">String</span></span>     |<span data-ttu-id="c9868-126">可读同步规则的名称。</span><span class="sxs-lookup"><span data-stu-id="c9868-126">Human-readable name of the synchronization rule.</span></span> <span data-ttu-id="c9868-127">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="c9868-127">Not nullable.</span></span>|
|<span data-ttu-id="c9868-128">objectMappings</span><span class="sxs-lookup"><span data-stu-id="c9868-128">objectMappings</span></span> |<span data-ttu-id="c9868-129">[objectMapping](synchronization-objectmapping.md)集合</span><span class="sxs-lookup"><span data-stu-id="c9868-129">[objectMapping](synchronization-objectmapping.md) collection</span></span>    |<span data-ttu-id="c9868-130">规则支持的对象映射的集合。</span><span class="sxs-lookup"><span data-stu-id="c9868-130">Collection of object mappings supported by the rule.</span></span> <span data-ttu-id="c9868-131">指示同步引擎应同步的对象。</span><span class="sxs-lookup"><span data-stu-id="c9868-131">Tells the synchronization engine which objects should be synchronized.</span></span>|
|<span data-ttu-id="c9868-132">priority</span><span class="sxs-lookup"><span data-stu-id="c9868-132">priority</span></span>       |<span data-ttu-id="c9868-133">整数</span><span class="sxs-lookup"><span data-stu-id="c9868-133">Integer</span></span>    |<span data-ttu-id="c9868-134">相对于[synchronizationSchema](synchronization-synchronizationschema.md)中其他规则的优先级。</span><span class="sxs-lookup"><span data-stu-id="c9868-134">Priority relative to other rules in the [synchronizationSchema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="c9868-135">将首先处理与最低优先级编号的规则。</span><span class="sxs-lookup"><span data-stu-id="c9868-135">Rules with the lowest priority number will be processed first.</span></span>|
|<span data-ttu-id="c9868-136">sourceDirectoryName</span><span class="sxs-lookup"><span data-stu-id="c9868-136">sourceDirectoryName</span></span>       |<span data-ttu-id="c9868-137">String</span><span class="sxs-lookup"><span data-stu-id="c9868-137">String</span></span>    |<span data-ttu-id="c9868-138">源目录的名称。</span><span class="sxs-lookup"><span data-stu-id="c9868-138">Name of the source directory.</span></span> <span data-ttu-id="c9868-139">必须匹配[synchronizationSchema](synchronization-synchronizationschema.md)中的目录定义之一。</span><span class="sxs-lookup"><span data-stu-id="c9868-139">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|
|<span data-ttu-id="c9868-140">targetDirectoryName</span><span class="sxs-lookup"><span data-stu-id="c9868-140">targetDirectoryName</span></span>       |<span data-ttu-id="c9868-141">String</span><span class="sxs-lookup"><span data-stu-id="c9868-141">String</span></span>    |<span data-ttu-id="c9868-142">目标目录的名称。</span><span class="sxs-lookup"><span data-stu-id="c9868-142">Name of the target directory.</span></span> <span data-ttu-id="c9868-143">必须匹配[synchronizationSchema](synchronization-synchronizationschema.md)中的目录定义之一。</span><span class="sxs-lookup"><span data-stu-id="c9868-143">Must match one of the directory definitions in [synchronizationSchema](synchronization-synchronizationschema.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9868-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9868-144">JSON representation</span></span>

<span data-ttu-id="c9868-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9868-145">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationrule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
