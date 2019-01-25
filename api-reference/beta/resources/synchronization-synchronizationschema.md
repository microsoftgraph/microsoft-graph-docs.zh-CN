---
title: synchronizationSchema 资源类型
description: 定义对象将同步和同步方式。 同步架构包含特定同步作业的设置信息的大部分。 通常情况下，您将自定义某些属性的映射，或添加范围筛选器同步只有满足特定条件的对象。
localization_priority: Normal
ms.openlocfilehash: e7bb91ef473a04552c4c5f33ffc9d54eb86a9b7a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515928"
---
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="1dbc7-105">synchronizationSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="1dbc7-105">synchronizationSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dbc7-106">定义对象将同步和同步方式。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-106">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="1dbc7-107">同步架构包含特定同步作业的设置信息的大部分。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-107">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="1dbc7-108">通常情况下，您将自定义某些[属性映射](synchronization-attributemapping.md)，或添加[范围筛选器](synchronization-filter.md)以同步只有满足特定条件的对象。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-108">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="1dbc7-109">以下各节介绍了同步架构的高级组件。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-109">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="1dbc7-110">目录定义</span><span class="sxs-lookup"><span data-stu-id="1dbc7-110">Directory definitions</span></span>

<span data-ttu-id="1dbc7-111">[目录定义](synchronization-directorydefinition.md)提供有关目录和其对象的同步引擎信息。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-111">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="1dbc7-112">例如，目录定义告知同步引擎 Azure AD 目录具有名为**用户**和**组**，这些对象，并为这些属性的类型支持哪些属性的对象。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-112">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="1dbc7-113">为了在同步规则/对象映射中使用的特定对象和属性，他们必须定义为目录定义的一部分。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-113">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="1dbc7-114">同步规则</span><span class="sxs-lookup"><span data-stu-id="1dbc7-114">Synchronization rules</span></span>

<span data-ttu-id="1dbc7-115">[同步规则](synchronization-synchronizationrule.md)是同步安装程序的核心。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-115">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="1dbc7-116">它们为同步引擎定义应如何执行的同步、 包括哪些对象应保持同步，从源目录对象与目标目录中的对象的匹配方式，并且应属性的方式转换他们正在同步时从源到目标目录。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-116">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span> 

## <a name="object-mappings"></a><span data-ttu-id="1dbc7-117">对象映射</span><span class="sxs-lookup"><span data-stu-id="1dbc7-117">Object mappings</span></span>

<span data-ttu-id="1dbc7-118">[对象映射](synchronization-objectmapping.md)是同步规则的主要部分。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-118">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="1dbc7-119">每个对象映射定义如何给定的对象应同步从源到目标目录。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-119">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="1dbc7-120">具体而言，映射定义源目录中的对象与目标目录中某个对象的匹配方式什么 （如果有） 范围筛选器应使用决定是否设置一个对象，以及应如何转换对象属性他们正在同步时从源到目标目录。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-120">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="1dbc7-121">方法</span><span class="sxs-lookup"><span data-stu-id="1dbc7-121">Methods</span></span>

| <span data-ttu-id="1dbc7-122">方法</span><span class="sxs-lookup"><span data-stu-id="1dbc7-122">Method</span></span>        | <span data-ttu-id="1dbc7-123">返回类型</span><span class="sxs-lookup"><span data-stu-id="1dbc7-123">Return Type</span></span>               | <span data-ttu-id="1dbc7-124">说明</span><span class="sxs-lookup"><span data-stu-id="1dbc7-124">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="1dbc7-125">获取架构</span><span class="sxs-lookup"><span data-stu-id="1dbc7-125">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="1dbc7-126">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="1dbc7-126">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="1dbc7-127">读取属性和**synchronizationSchema**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-127">Read properties and relationships of the **synchronizationSchema** object.</span></span>|
|[<span data-ttu-id="1dbc7-128">更新架构</span><span class="sxs-lookup"><span data-stu-id="1dbc7-128">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="1dbc7-129">无</span><span class="sxs-lookup"><span data-stu-id="1dbc7-129">None</span></span>   |<span data-ttu-id="1dbc7-130">更新同步架构。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-130">Update the synchronization schema.</span></span> |
|[<span data-ttu-id="1dbc7-131">删除架构</span><span class="sxs-lookup"><span data-stu-id="1dbc7-131">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)    |<span data-ttu-id="1dbc7-132">无</span><span class="sxs-lookup"><span data-stu-id="1dbc7-132">None</span></span>   |<span data-ttu-id="1dbc7-133">删除自定义的架构，重置为默认配置的架构。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-133">Delete the customized schema, resetting the schema to the default configuration.</span></span> |
|[<span data-ttu-id="1dbc7-134">列表筛选器运算符</span><span class="sxs-lookup"><span data-stu-id="1dbc7-134">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)    |<span data-ttu-id="1dbc7-135">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="1dbc7-135">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) colection</span></span>   |<span data-ttu-id="1dbc7-136">列出所有支持的范围筛选器中的运算符。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-136">List all operators supported in the scoping filters.</span></span> |
|[<span data-ttu-id="1dbc7-137">List 属性映射函数</span><span class="sxs-lookup"><span data-stu-id="1dbc7-137">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)    |<span data-ttu-id="1dbc7-138">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="1dbc7-138">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>   |<span data-ttu-id="1dbc7-139">列出属性映射表达式中支持的所有功能。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-139">List all functions supported in the attribute mapping expressions.</span></span> |
|[<span data-ttu-id="1dbc7-140">分析属性映射表达式</span><span class="sxs-lookup"><span data-stu-id="1dbc7-140">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md)|[<span data-ttu-id="1dbc7-141">parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="1dbc7-141">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)|<span data-ttu-id="1dbc7-142">分析 [attributeMappingSource 字符串表达式</span><span class="sxs-lookup"><span data-stu-id="1dbc7-142">Parse a string expression into an [attributeMappingSource</span></span>|<span data-ttu-id="1dbc7-143">(../ resources/synchronization_attributemappingsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-143">(../resources/synchronization_attributemappingsource.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="1dbc7-144">属性</span><span class="sxs-lookup"><span data-stu-id="1dbc7-144">Properties</span></span>

| <span data-ttu-id="1dbc7-145">属性</span><span class="sxs-lookup"><span data-stu-id="1dbc7-145">Property</span></span>      | <span data-ttu-id="1dbc7-146">类型</span><span class="sxs-lookup"><span data-stu-id="1dbc7-146">Type</span></span>      | <span data-ttu-id="1dbc7-147">说明</span><span class="sxs-lookup"><span data-stu-id="1dbc7-147">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="1dbc7-148">directories</span><span class="sxs-lookup"><span data-stu-id="1dbc7-148">directories</span></span>            |<span data-ttu-id="1dbc7-149">[directoryDefinition](synchronization-directorydefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="1dbc7-149">[directoryDefinition](synchronization-directorydefinition.md) collection</span></span>   |<span data-ttu-id="1dbc7-150">描述目录和[synchronizationJob](synchronization-synchronizationjob.md)或[synchronizationTemplate](synchronization-synchronizationtemplate.md)的一部分的对象。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-150">Describes directories and objects that are part of the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="1dbc7-151">synchronizationRules</span><span class="sxs-lookup"><span data-stu-id="1dbc7-151">synchronizationRules</span></span>   |<span data-ttu-id="1dbc7-152">[synchronizationRule](synchronization-synchronizationrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="1dbc7-152">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="1dbc7-153">同步规则[synchronizationJob](synchronization-synchronizationjob.md)或[synchronizationTemplate](synchronization-synchronizationtemplate.md)，配置的集合</span><span class="sxs-lookup"><span data-stu-id="1dbc7-153">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span></span> |
|<span data-ttu-id="1dbc7-154">version</span><span class="sxs-lookup"><span data-stu-id="1dbc7-154">version</span></span>                |<span data-ttu-id="1dbc7-155">String</span><span class="sxs-lookup"><span data-stu-id="1dbc7-155">String</span></span>                             |<span data-ttu-id="1dbc7-156">架构，每次架构更改自动更新的版本。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-156">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1dbc7-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1dbc7-157">JSON representation</span></span>

<span data-ttu-id="1dbc7-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1dbc7-158">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
