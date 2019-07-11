---
title: synchronizationSchema 资源类型
description: 定义将同步的对象以及同步的对象。 同步架构包含特定同步作业的大部分安装信息。 通常情况下, 您将自定义一些属性映射, 或添加作用域筛选器以仅同步满足特定条件的对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7d4302cec5fe568f322e5a8d1b86bc4681b50f7c
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620680"
---
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="22a43-105">synchronizationSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="22a43-105">synchronizationSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22a43-106">定义将同步的对象以及同步的对象。</span><span class="sxs-lookup"><span data-stu-id="22a43-106">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="22a43-107">同步架构包含特定同步作业的大部分安装信息。</span><span class="sxs-lookup"><span data-stu-id="22a43-107">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="22a43-108">通常情况下, 您将自定义一些[属性映射](synchronization-attributemapping.md), 或添加[作用域筛选器](synchronization-filter.md)以仅同步满足特定条件的对象。</span><span class="sxs-lookup"><span data-stu-id="22a43-108">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="22a43-109">以下各节介绍了同步架构的高级组件。</span><span class="sxs-lookup"><span data-stu-id="22a43-109">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="22a43-110">目录定义</span><span class="sxs-lookup"><span data-stu-id="22a43-110">Directory definitions</span></span>

<span data-ttu-id="22a43-111">[目录定义](synchronization-directorydefinition.md)提供有关目录及其对象的同步引擎信息。</span><span class="sxs-lookup"><span data-stu-id="22a43-111">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="22a43-112">例如, 目录定义告知同步引擎: Azure AD 目录包含名为**user**和**group**的对象, 这些对象支持哪些属性以及这些属性的类型。</span><span class="sxs-lookup"><span data-stu-id="22a43-112">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="22a43-113">为了在同步规则/对象映射中使用特定对象和属性, 必须将其定义为目录定义的一部分。</span><span class="sxs-lookup"><span data-stu-id="22a43-113">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="22a43-114">同步规则</span><span class="sxs-lookup"><span data-stu-id="22a43-114">Synchronization rules</span></span>

<span data-ttu-id="22a43-115">[同步规则](synchronization-synchronizationrule.md)是同步设置的核心。</span><span class="sxs-lookup"><span data-stu-id="22a43-115">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="22a43-116">它们定义同步引擎应如何执行同步, 包括应同步的对象、源目录中的对象与目标目录中的对象的匹配方式以及属性应如何在将其从源目录同步到目标目录时进行转换。</span><span class="sxs-lookup"><span data-stu-id="22a43-116">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span> 

## <a name="object-mappings"></a><span data-ttu-id="22a43-117">对象映射</span><span class="sxs-lookup"><span data-stu-id="22a43-117">Object mappings</span></span>

<span data-ttu-id="22a43-118">[对象映射](synchronization-objectmapping.md)是同步规则的主要部分。</span><span class="sxs-lookup"><span data-stu-id="22a43-118">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="22a43-119">每个对象映射定义应如何将给定对象从源同步到目标目录。</span><span class="sxs-lookup"><span data-stu-id="22a43-119">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="22a43-120">特别是, 映射定义源目录中的对象应如何与目标目录中的对象匹配, 应使用什么 (如果有) 作用域筛选器来决定是否设置对象, 以及应如何转换对象属性将其从源目录同步到目标目录。</span><span class="sxs-lookup"><span data-stu-id="22a43-120">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="22a43-121">方法</span><span class="sxs-lookup"><span data-stu-id="22a43-121">Methods</span></span>

| <span data-ttu-id="22a43-122">方法</span><span class="sxs-lookup"><span data-stu-id="22a43-122">Method</span></span>        | <span data-ttu-id="22a43-123">返回类型</span><span class="sxs-lookup"><span data-stu-id="22a43-123">Return Type</span></span>               | <span data-ttu-id="22a43-124">说明</span><span class="sxs-lookup"><span data-stu-id="22a43-124">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="22a43-125">获取架构</span><span class="sxs-lookup"><span data-stu-id="22a43-125">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="22a43-126">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="22a43-126">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="22a43-127">读取**synchronizationSchema**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="22a43-127">Read properties and relationships of the **synchronizationSchema** object.</span></span>|
|[<span data-ttu-id="22a43-128">更新架构</span><span class="sxs-lookup"><span data-stu-id="22a43-128">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="22a43-129">无</span><span class="sxs-lookup"><span data-stu-id="22a43-129">None</span></span>   |<span data-ttu-id="22a43-130">更新同步架构。</span><span class="sxs-lookup"><span data-stu-id="22a43-130">Update the synchronization schema.</span></span> |
|[<span data-ttu-id="22a43-131">删除架构</span><span class="sxs-lookup"><span data-stu-id="22a43-131">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)    |<span data-ttu-id="22a43-132">无</span><span class="sxs-lookup"><span data-stu-id="22a43-132">None</span></span>   |<span data-ttu-id="22a43-133">删除自定义架构, 将架构重置为默认配置。</span><span class="sxs-lookup"><span data-stu-id="22a43-133">Delete the customized schema, resetting the schema to the default configuration.</span></span> |
|[<span data-ttu-id="22a43-134">列表筛选器运算符</span><span class="sxs-lookup"><span data-stu-id="22a43-134">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)    |<span data-ttu-id="22a43-135">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="22a43-135">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) colection</span></span>   |<span data-ttu-id="22a43-136">列出作用域筛选器支持的所有运算符。</span><span class="sxs-lookup"><span data-stu-id="22a43-136">List all operators supported in the scoping filters.</span></span> |
|[<span data-ttu-id="22a43-137">列表属性映射函数</span><span class="sxs-lookup"><span data-stu-id="22a43-137">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)    |<span data-ttu-id="22a43-138">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="22a43-138">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>   |<span data-ttu-id="22a43-139">列出属性映射表达式中支持的所有函数。</span><span class="sxs-lookup"><span data-stu-id="22a43-139">List all functions supported in the attribute mapping expressions.</span></span> |
|[<span data-ttu-id="22a43-140">分析属性映射表达式</span><span class="sxs-lookup"><span data-stu-id="22a43-140">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md)|[<span data-ttu-id="22a43-141">parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="22a43-141">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)|<span data-ttu-id="22a43-142">将字符串表达式分析为 [attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="22a43-142">Parse a string expression into an [attributeMappingSource</span></span>|<span data-ttu-id="22a43-143">(../resources/synchronization_attributemappingsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="22a43-143">(../resources/synchronization_attributemappingsource.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="22a43-144">属性</span><span class="sxs-lookup"><span data-stu-id="22a43-144">Properties</span></span>

| <span data-ttu-id="22a43-145">属性</span><span class="sxs-lookup"><span data-stu-id="22a43-145">Property</span></span>      | <span data-ttu-id="22a43-146">类型</span><span class="sxs-lookup"><span data-stu-id="22a43-146">Type</span></span>      | <span data-ttu-id="22a43-147">说明</span><span class="sxs-lookup"><span data-stu-id="22a43-147">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="22a43-148">目录名</span><span class="sxs-lookup"><span data-stu-id="22a43-148">directories</span></span>            |<span data-ttu-id="22a43-149">[directoryDefinition](synchronization-directorydefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="22a43-149">[directoryDefinition](synchronization-directorydefinition.md) collection</span></span>   |<span data-ttu-id="22a43-150">描述作为[synchronizationJob](synchronization-synchronizationjob.md)或[synchronizationTemplate](synchronization-synchronizationtemplate.md)一部分的目录和对象。</span><span class="sxs-lookup"><span data-stu-id="22a43-150">Describes directories and objects that are part of the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="22a43-151">synchronizationRules</span><span class="sxs-lookup"><span data-stu-id="22a43-151">synchronizationRules</span></span>   |<span data-ttu-id="22a43-152">[synchronizationRule](synchronization-synchronizationrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="22a43-152">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="22a43-153">为[synchronizationJob](synchronization-synchronizationjob.md)或[synchronizationTemplate](synchronization-synchronizationtemplate.md)配置的同步规则的集合。</span><span class="sxs-lookup"><span data-stu-id="22a43-153">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span></span> |
|<span data-ttu-id="22a43-154">version</span><span class="sxs-lookup"><span data-stu-id="22a43-154">version</span></span>                |<span data-ttu-id="22a43-155">String</span><span class="sxs-lookup"><span data-stu-id="22a43-155">String</span></span>                             |<span data-ttu-id="22a43-156">架构的版本, 随每个架构更改自动更新。</span><span class="sxs-lookup"><span data-stu-id="22a43-156">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="22a43-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22a43-157">JSON representation</span></span>

<span data-ttu-id="22a43-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22a43-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchema"
}-->

```json
{
  "directories": [{"@odata.type": "microsoft.graph.directoryDefinition"}],
  "provisioningTaskIdentifier": "String (identifier)",
  "synchronizationRules": [{"@odata.type": "microsoft.graph.synchronizationRule"}],
  "version": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
