---
title: synchronizationSchema 资源类型
description: 定义将同步的对象以及同步的对象。 同步架构包含特定同步作业的大部分安装信息。 通常情况下，您将自定义一些属性映射，或添加作用域筛选器以仅同步满足特定条件的对象。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3a50a53c7d76d281f4a42e976bacc0803377379d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520035"
---
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="52b15-105">synchronizationSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="52b15-105">synchronizationSchema resource type</span></span>

<span data-ttu-id="52b15-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="52b15-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52b15-107">定义将同步的对象以及同步的对象。</span><span class="sxs-lookup"><span data-stu-id="52b15-107">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="52b15-108">同步架构包含特定同步作业的大部分安装信息。</span><span class="sxs-lookup"><span data-stu-id="52b15-108">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="52b15-109">通常情况下，您将自定义一些[属性映射](synchronization-attributemapping.md)，或添加[作用域筛选器](synchronization-filter.md)以仅同步满足特定条件的对象。</span><span class="sxs-lookup"><span data-stu-id="52b15-109">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="52b15-110">以下各节介绍了同步架构的高级组件。</span><span class="sxs-lookup"><span data-stu-id="52b15-110">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="52b15-111">目录定义</span><span class="sxs-lookup"><span data-stu-id="52b15-111">Directory definitions</span></span>

<span data-ttu-id="52b15-112">[目录定义](synchronization-directorydefinition.md)提供有关目录及其对象的同步引擎信息。</span><span class="sxs-lookup"><span data-stu-id="52b15-112">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="52b15-113">例如，目录定义告知同步引擎： Azure AD 目录包含名为**user**和**group**的对象，这些对象支持哪些属性以及这些属性的类型。</span><span class="sxs-lookup"><span data-stu-id="52b15-113">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="52b15-114">为了在同步规则/对象映射中使用特定对象和属性，必须将其定义为目录定义的一部分。</span><span class="sxs-lookup"><span data-stu-id="52b15-114">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="52b15-115">同步规则</span><span class="sxs-lookup"><span data-stu-id="52b15-115">Synchronization rules</span></span>

<span data-ttu-id="52b15-116">[同步规则](synchronization-synchronizationrule.md)是同步设置的核心。</span><span class="sxs-lookup"><span data-stu-id="52b15-116">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="52b15-117">它们定义同步引擎应如何执行同步，包括应同步的对象、源目录中的对象与目标目录中的对象的匹配方式以及属性应如何在将其从源目录同步到目标目录时进行转换。</span><span class="sxs-lookup"><span data-stu-id="52b15-117">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span> 

## <a name="object-mappings"></a><span data-ttu-id="52b15-118">对象映射</span><span class="sxs-lookup"><span data-stu-id="52b15-118">Object mappings</span></span>

<span data-ttu-id="52b15-119">[对象映射](synchronization-objectmapping.md)是同步规则的主要部分。</span><span class="sxs-lookup"><span data-stu-id="52b15-119">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="52b15-120">每个对象映射定义应如何将给定对象从源同步到目标目录。</span><span class="sxs-lookup"><span data-stu-id="52b15-120">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="52b15-121">特别是，映射定义源目录中的对象应如何与目标目录中的对象匹配，应使用什么（如果有）作用域筛选器来决定是否设置对象，以及应如何转换对象属性将其从源目录同步到目标目录。</span><span class="sxs-lookup"><span data-stu-id="52b15-121">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="52b15-122">方法</span><span class="sxs-lookup"><span data-stu-id="52b15-122">Methods</span></span>

| <span data-ttu-id="52b15-123">方法</span><span class="sxs-lookup"><span data-stu-id="52b15-123">Method</span></span>        | <span data-ttu-id="52b15-124">返回类型</span><span class="sxs-lookup"><span data-stu-id="52b15-124">Return Type</span></span>               | <span data-ttu-id="52b15-125">说明</span><span class="sxs-lookup"><span data-stu-id="52b15-125">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="52b15-126">获取架构</span><span class="sxs-lookup"><span data-stu-id="52b15-126">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="52b15-127">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="52b15-127">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="52b15-128">读取**synchronizationSchema**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="52b15-128">Read properties and relationships of the **synchronizationSchema** object.</span></span>|
|[<span data-ttu-id="52b15-129">更新架构</span><span class="sxs-lookup"><span data-stu-id="52b15-129">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="52b15-130">无</span><span class="sxs-lookup"><span data-stu-id="52b15-130">None</span></span>   |<span data-ttu-id="52b15-131">更新同步架构。</span><span class="sxs-lookup"><span data-stu-id="52b15-131">Update the synchronization schema.</span></span> |
|[<span data-ttu-id="52b15-132">删除架构</span><span class="sxs-lookup"><span data-stu-id="52b15-132">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)    |<span data-ttu-id="52b15-133">无</span><span class="sxs-lookup"><span data-stu-id="52b15-133">None</span></span>   |<span data-ttu-id="52b15-134">删除自定义架构，将架构重置为默认配置。</span><span class="sxs-lookup"><span data-stu-id="52b15-134">Delete the customized schema, resetting the schema to the default configuration.</span></span> |
|[<span data-ttu-id="52b15-135">列表筛选器运算符</span><span class="sxs-lookup"><span data-stu-id="52b15-135">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)    |<span data-ttu-id="52b15-136">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="52b15-136">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) colection</span></span>   |<span data-ttu-id="52b15-137">列出作用域筛选器支持的所有运算符。</span><span class="sxs-lookup"><span data-stu-id="52b15-137">List all operators supported in the scoping filters.</span></span> |
|[<span data-ttu-id="52b15-138">列表属性映射函数</span><span class="sxs-lookup"><span data-stu-id="52b15-138">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)    |<span data-ttu-id="52b15-139">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="52b15-139">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>   |<span data-ttu-id="52b15-140">列出属性映射表达式中支持的所有函数。</span><span class="sxs-lookup"><span data-stu-id="52b15-140">List all functions supported in the attribute mapping expressions.</span></span> |
|[<span data-ttu-id="52b15-141">分析属性映射表达式</span><span class="sxs-lookup"><span data-stu-id="52b15-141">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md)|[<span data-ttu-id="52b15-142">parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="52b15-142">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)|<span data-ttu-id="52b15-143">将字符串表达式分析为 [attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="52b15-143">Parse a string expression into an [attributeMappingSource</span></span>|<span data-ttu-id="52b15-144">(../resources/synchronization_attributemappingsource）对象。</span><span class="sxs-lookup"><span data-stu-id="52b15-144">(../resources/synchronization_attributemappingsource.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="52b15-145">属性</span><span class="sxs-lookup"><span data-stu-id="52b15-145">Properties</span></span>

| <span data-ttu-id="52b15-146">属性</span><span class="sxs-lookup"><span data-stu-id="52b15-146">Property</span></span>      | <span data-ttu-id="52b15-147">类型</span><span class="sxs-lookup"><span data-stu-id="52b15-147">Type</span></span>      | <span data-ttu-id="52b15-148">说明</span><span class="sxs-lookup"><span data-stu-id="52b15-148">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="52b15-149">目录名</span><span class="sxs-lookup"><span data-stu-id="52b15-149">directories</span></span>            |<span data-ttu-id="52b15-150">[directoryDefinition](synchronization-directorydefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="52b15-150">[directoryDefinition](synchronization-directorydefinition.md) collection</span></span>   |<span data-ttu-id="52b15-151">描述作为[synchronizationJob](synchronization-synchronizationjob.md)或[synchronizationTemplate](synchronization-synchronizationtemplate.md)一部分的目录和对象。</span><span class="sxs-lookup"><span data-stu-id="52b15-151">Describes directories and objects that are part of the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="52b15-152">synchronizationRules</span><span class="sxs-lookup"><span data-stu-id="52b15-152">synchronizationRules</span></span>   |<span data-ttu-id="52b15-153">[synchronizationRule](synchronization-synchronizationrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="52b15-153">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="52b15-154">为[synchronizationJob](synchronization-synchronizationjob.md)或[synchronizationTemplate](synchronization-synchronizationtemplate.md)配置的同步规则的集合。</span><span class="sxs-lookup"><span data-stu-id="52b15-154">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md),</span></span> |
|<span data-ttu-id="52b15-155">version</span><span class="sxs-lookup"><span data-stu-id="52b15-155">version</span></span>                |<span data-ttu-id="52b15-156">String</span><span class="sxs-lookup"><span data-stu-id="52b15-156">String</span></span>                             |<span data-ttu-id="52b15-157">架构的版本，随每个架构更改自动更新。</span><span class="sxs-lookup"><span data-stu-id="52b15-157">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="52b15-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52b15-158">JSON representation</span></span>

<span data-ttu-id="52b15-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52b15-159">The following is a JSON representation of the resource.</span></span>

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
