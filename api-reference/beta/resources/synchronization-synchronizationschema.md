---
title: synchronizationSchema 资源类型
description: 定义要同步的对象及其同步的方式。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: b16e892c44cb69fb5039418a4a246e8b6f32ae9f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131591"
---
# <a name="synchronizationschema-resource-type"></a><span data-ttu-id="9598c-103">synchronizationSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="9598c-103">synchronizationSchema resource type</span></span>

<span data-ttu-id="9598c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9598c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9598c-105">定义要同步的对象及其同步的方式。</span><span class="sxs-lookup"><span data-stu-id="9598c-105">Defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="9598c-106">同步架构包含特定同步作业的多数设置信息。</span><span class="sxs-lookup"><span data-stu-id="9598c-106">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="9598c-107">通常，您将自定义某些[属性](synchronization-attributemapping.md)映射，或添加范围筛选器以仅同步满足[](synchronization-filter.md)特定条件的对象。</span><span class="sxs-lookup"><span data-stu-id="9598c-107">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="9598c-108">以下各节介绍同步架构的高级别组件。</span><span class="sxs-lookup"><span data-stu-id="9598c-108">The following sections describe the high-level components of the synchronization schema.</span></span>

## <a name="directory-definitions"></a><span data-ttu-id="9598c-109">目录定义</span><span class="sxs-lookup"><span data-stu-id="9598c-109">Directory definitions</span></span>

<span data-ttu-id="9598c-110">[目录定义](synchronization-directorydefinition.md) 提供有关目录及其对象的同步引擎信息。</span><span class="sxs-lookup"><span data-stu-id="9598c-110">[Directory definitions](synchronization-directorydefinition.md) provide the synchronization engine information about directories and their objects.</span></span> <span data-ttu-id="9598c-111">例如，目录定义告知同步引擎，Azure AD 目录具有名为 user 和 **group** 的对象、这些对象支持哪些属性以及这些属性的类型。</span><span class="sxs-lookup"><span data-stu-id="9598c-111">For example, the directory definition tells the synchronization engine that an Azure AD directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="9598c-112">为了使特定对象和属性用于同步规则/对象映射，它们必须定义为目录定义的一部分。</span><span class="sxs-lookup"><span data-stu-id="9598c-112">In order for a particular object and attribute to be used in synchronization rules/object mappings, they have to be defined as part of the directory definition.</span></span>

## <a name="synchronization-rules"></a><span data-ttu-id="9598c-113">同步规则</span><span class="sxs-lookup"><span data-stu-id="9598c-113">Synchronization rules</span></span>

<span data-ttu-id="9598c-114">[同步](synchronization-synchronizationrule.md) 规则是同步设置的核心。</span><span class="sxs-lookup"><span data-stu-id="9598c-114">[Synchronization rules](synchronization-synchronizationrule.md) are the core of the synchronization setup.</span></span> <span data-ttu-id="9598c-115">它们为同步引擎定义如何执行同步，包括应同步哪些对象、源目录中的对象应该如何与目标目录中的对象匹配，以及属性在从源目录同步到目标目录时如何转换。</span><span class="sxs-lookup"><span data-stu-id="9598c-115">They define for the synchronization engine how the synchronization should be performed, including what objects should be synchronized, how objects from the source directory should be matched with objects in the target directory, and how attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="object-mappings"></a><span data-ttu-id="9598c-116">对象映射</span><span class="sxs-lookup"><span data-stu-id="9598c-116">Object mappings</span></span>

<span data-ttu-id="9598c-117">[对象映射](synchronization-objectmapping.md) 是同步规则的主要部分。</span><span class="sxs-lookup"><span data-stu-id="9598c-117">[Object mappings](synchronization-objectmapping.md) are the main part of the synchronization rule.</span></span> <span data-ttu-id="9598c-118">每个对象映射都定义给定对象如何从源目录同步到目标目录。</span><span class="sxs-lookup"><span data-stu-id="9598c-118">Each object mapping defines how a given object should be synchronized from the source to the target directory.</span></span> <span data-ttu-id="9598c-119">具体而言，该映射定义源目录中的对象如何与目标目录中的对象匹配，使用什么 (（如果有) 范围筛选器）决定是否设置对象，以及当对象属性从源目录同步到目标目录时，如何转换它们。</span><span class="sxs-lookup"><span data-stu-id="9598c-119">In particular, the mapping defines how an object in the source directory should be matched with an object in the target directory, what (if any) scoping filters should be used to decide whether to provision an object, and how object attributes should be transformed when they're synchronized from the source to the target directory.</span></span>

## <a name="methods"></a><span data-ttu-id="9598c-120">方法</span><span class="sxs-lookup"><span data-stu-id="9598c-120">Methods</span></span>

| <span data-ttu-id="9598c-121">方法</span><span class="sxs-lookup"><span data-stu-id="9598c-121">Method</span></span>                                                                                                | <span data-ttu-id="9598c-122">返回类型</span><span class="sxs-lookup"><span data-stu-id="9598c-122">Return Type</span></span>                                                                                                 | <span data-ttu-id="9598c-123">说明</span><span class="sxs-lookup"><span data-stu-id="9598c-123">Description</span></span>                                                                                                                |
|:------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------|
| [<span data-ttu-id="9598c-124">获取架构</span><span class="sxs-lookup"><span data-stu-id="9598c-124">Get schema</span></span>](../api/synchronization-synchronizationschema-get.md)                                     | [<span data-ttu-id="9598c-125">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="9598c-125">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)                                           | <span data-ttu-id="9598c-126">读取 **synchronizationSchema** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9598c-126">Read properties and relationships of the **synchronizationSchema** object.</span></span>                                                 |
| [<span data-ttu-id="9598c-127">更新架构</span><span class="sxs-lookup"><span data-stu-id="9598c-127">Update schema</span></span>](../api/synchronization-synchronizationschema-update.md)                               | <span data-ttu-id="9598c-128">无</span><span class="sxs-lookup"><span data-stu-id="9598c-128">None</span></span>                                                                                                        | <span data-ttu-id="9598c-129">更新同步架构。</span><span class="sxs-lookup"><span data-stu-id="9598c-129">Update the synchronization schema.</span></span>                                                                                         |
| [<span data-ttu-id="9598c-130">删除架构</span><span class="sxs-lookup"><span data-stu-id="9598c-130">Delete schema</span></span>](../api/synchronization-synchronizationschema-delete.md)                               | <span data-ttu-id="9598c-131">无</span><span class="sxs-lookup"><span data-stu-id="9598c-131">None</span></span>                                                                                                        | <span data-ttu-id="9598c-132">删除自定义架构，将架构重置为默认配置。</span><span class="sxs-lookup"><span data-stu-id="9598c-132">Delete the customized schema, resetting the schema to the default configuration.</span></span>                                           |
| [<span data-ttu-id="9598c-133">列出筛选器运算符</span><span class="sxs-lookup"><span data-stu-id="9598c-133">List filter operators</span></span>](../api/synchronization-synchronizationschema-filteroperators.md)              | <span data-ttu-id="9598c-134">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9598c-134">[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection</span></span>                      | <span data-ttu-id="9598c-135">列出范围筛选器中支持的所有运算符。</span><span class="sxs-lookup"><span data-stu-id="9598c-135">List all operators supported in the scoping filters.</span></span>                                                                       |
| [<span data-ttu-id="9598c-136">列表属性映射函数</span><span class="sxs-lookup"><span data-stu-id="9598c-136">List attribute mapping functions</span></span>](../api/synchronization-synchronizationschema-functions.md)         | <span data-ttu-id="9598c-137">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9598c-137">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span> | <span data-ttu-id="9598c-138">列出属性映射表达式中支持的所有函数。</span><span class="sxs-lookup"><span data-stu-id="9598c-138">List all functions supported in the attribute mapping expressions.</span></span>                                                         |
| [<span data-ttu-id="9598c-139">分析属性映射表达式</span><span class="sxs-lookup"><span data-stu-id="9598c-139">Parse attribute mapping expression</span></span>](../api/synchronization-synchronizationschema-parseexpression.md) | [<span data-ttu-id="9598c-140">parseExpressionResponse</span><span class="sxs-lookup"><span data-stu-id="9598c-140">parseExpressionResponse</span></span>](synchronization-parseexpressionresponse.md)                                       | <span data-ttu-id="9598c-141">将字符串表达式解析为 [attributeMappingSource](../resources/synchronization-attributemappingsource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9598c-141">Parse a string expression into an [attributeMappingSource](../resources/synchronization-attributemappingsource.md) object.</span></span> |


## <a name="properties"></a><span data-ttu-id="9598c-142">属性</span><span class="sxs-lookup"><span data-stu-id="9598c-142">Properties</span></span>

| <span data-ttu-id="9598c-143">属性</span><span class="sxs-lookup"><span data-stu-id="9598c-143">Property</span></span>      | <span data-ttu-id="9598c-144">类型</span><span class="sxs-lookup"><span data-stu-id="9598c-144">Type</span></span>      | <span data-ttu-id="9598c-145">说明</span><span class="sxs-lookup"><span data-stu-id="9598c-145">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="9598c-146">id</span><span class="sxs-lookup"><span data-stu-id="9598c-146">id</span></span>|<span data-ttu-id="9598c-147">字符串</span><span class="sxs-lookup"><span data-stu-id="9598c-147">String</span></span>|<span data-ttu-id="9598c-148">架构的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9598c-148">Unique identifier for the schema.</span></span>|
|<span data-ttu-id="9598c-149">synchronizationRules</span><span class="sxs-lookup"><span data-stu-id="9598c-149">synchronizationRules</span></span>   |<span data-ttu-id="9598c-150">[synchronizationRule](synchronization-synchronizationrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9598c-150">[synchronizationRule](synchronization-synchronizationrule.md) collection</span></span>   |<span data-ttu-id="9598c-151">为 [synchronizationJob](synchronization-synchronizationjob.md) 或 [synchronizationTemplate](synchronization-synchronizationtemplate.md)配置的同步规则的集合。</span><span class="sxs-lookup"><span data-stu-id="9598c-151">A collection of synchronization rules configured for the [synchronizationJob](synchronization-synchronizationjob.md) or [synchronizationTemplate](synchronization-synchronizationtemplate.md).</span></span> |
|<span data-ttu-id="9598c-152">version</span><span class="sxs-lookup"><span data-stu-id="9598c-152">version</span></span>                |<span data-ttu-id="9598c-153">String</span><span class="sxs-lookup"><span data-stu-id="9598c-153">String</span></span>                             |<span data-ttu-id="9598c-154">架构版本，随每个架构更改自动更新。</span><span class="sxs-lookup"><span data-stu-id="9598c-154">The version of the schema, updated automatically with every schema change.</span></span>|


## <a name="relationships"></a><span data-ttu-id="9598c-155">关系</span><span class="sxs-lookup"><span data-stu-id="9598c-155">Relationships</span></span>
|<span data-ttu-id="9598c-156">关系</span><span class="sxs-lookup"><span data-stu-id="9598c-156">Relationship</span></span>|<span data-ttu-id="9598c-157">类型</span><span class="sxs-lookup"><span data-stu-id="9598c-157">Type</span></span>|<span data-ttu-id="9598c-158">说明</span><span class="sxs-lookup"><span data-stu-id="9598c-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9598c-159">目录</span><span class="sxs-lookup"><span data-stu-id="9598c-159">directories</span></span>|<span data-ttu-id="9598c-160">[directoryDefinition](../resources/synchronization-directorydefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9598c-160">[directoryDefinition](../resources/synchronization-directorydefinition.md) collection</span></span>|<span data-ttu-id="9598c-161">包含目录及其所有对象的集合。</span><span class="sxs-lookup"><span data-stu-id="9598c-161">Contains the collection of directories and all of their objects.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9598c-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9598c-162">JSON representation</span></span>
<span data-ttu-id="9598c-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9598c-163">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationSchema",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationSchema",
  "id": "String (identifier)",
  "synchronizationRules": [
    {
      "@odata.type": "microsoft.graph.synchronizationRule"
    }
  ],
  "version": "String"
}
```


