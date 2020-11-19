---
title: groupPolicyConfiguration 资源类型
description: 组策略配置实体包含一个或多个组策略定义的配置值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e4fce57585c0dee4f73719870da7d07a2d710cd5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267192"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="ee484-103">groupPolicyConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee484-103">groupPolicyConfiguration resource type</span></span>

<span data-ttu-id="ee484-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee484-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee484-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ee484-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee484-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ee484-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee484-107">组策略配置实体包含一个或多个组策略定义的配置值。</span><span class="sxs-lookup"><span data-stu-id="ee484-107">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="ee484-108">方法</span><span class="sxs-lookup"><span data-stu-id="ee484-108">Methods</span></span>
|<span data-ttu-id="ee484-109">方法</span><span class="sxs-lookup"><span data-stu-id="ee484-109">Method</span></span>|<span data-ttu-id="ee484-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ee484-110">Return Type</span></span>|<span data-ttu-id="ee484-111">说明</span><span class="sxs-lookup"><span data-stu-id="ee484-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ee484-112">列出 groupPolicyConfigurations</span><span class="sxs-lookup"><span data-stu-id="ee484-112">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="ee484-113">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ee484-113">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="ee484-114">列出 [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ee484-114">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="ee484-115">获取 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee484-115">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="ee484-116">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee484-116">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="ee484-117">读取 [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ee484-117">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ee484-118">创建 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee484-118">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="ee484-119">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee484-119">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="ee484-120">创建新的 [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ee484-120">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ee484-121">删除 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee484-121">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="ee484-122">无</span><span class="sxs-lookup"><span data-stu-id="ee484-122">None</span></span>|<span data-ttu-id="ee484-123">删除 [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="ee484-123">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="ee484-124">更新 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee484-124">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="ee484-125">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee484-125">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="ee484-126">更新 [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ee484-126">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ee484-127">分配操作</span><span class="sxs-lookup"><span data-stu-id="ee484-127">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="ee484-128">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ee484-128">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ee484-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ee484-129">Not yet documented</span></span>|
|[<span data-ttu-id="ee484-130">updateDefinitionValues 操作</span><span class="sxs-lookup"><span data-stu-id="ee484-130">updateDefinitionValues action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-updatedefinitionvalues.md)|<span data-ttu-id="ee484-131">无</span><span class="sxs-lookup"><span data-stu-id="ee484-131">None</span></span>|<span data-ttu-id="ee484-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ee484-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ee484-133">属性</span><span class="sxs-lookup"><span data-stu-id="ee484-133">Properties</span></span>
|<span data-ttu-id="ee484-134">属性</span><span class="sxs-lookup"><span data-stu-id="ee484-134">Property</span></span>|<span data-ttu-id="ee484-135">类型</span><span class="sxs-lookup"><span data-stu-id="ee484-135">Type</span></span>|<span data-ttu-id="ee484-136">说明</span><span class="sxs-lookup"><span data-stu-id="ee484-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee484-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee484-137">createdDateTime</span></span>|<span data-ttu-id="ee484-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee484-138">DateTimeOffset</span></span>|<span data-ttu-id="ee484-139">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ee484-139">The date and time the object was created.</span></span>|
|<span data-ttu-id="ee484-140">displayName</span><span class="sxs-lookup"><span data-stu-id="ee484-140">displayName</span></span>|<span data-ttu-id="ee484-141">字符串</span><span class="sxs-lookup"><span data-stu-id="ee484-141">String</span></span>|<span data-ttu-id="ee484-142">用户提供的资源对象的名称。</span><span class="sxs-lookup"><span data-stu-id="ee484-142">User provided name for the resource object.</span></span>|
|<span data-ttu-id="ee484-143">description</span><span class="sxs-lookup"><span data-stu-id="ee484-143">description</span></span>|<span data-ttu-id="ee484-144">字符串</span><span class="sxs-lookup"><span data-stu-id="ee484-144">String</span></span>|<span data-ttu-id="ee484-145">用户提供的资源对象的说明。</span><span class="sxs-lookup"><span data-stu-id="ee484-145">User provided description for the resource object.</span></span>|
|<span data-ttu-id="ee484-146">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ee484-146">roleScopeTagIds</span></span>|<span data-ttu-id="ee484-147">String 集合</span><span class="sxs-lookup"><span data-stu-id="ee484-147">String collection</span></span>|<span data-ttu-id="ee484-148">配置的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="ee484-148">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="ee484-149">id</span><span class="sxs-lookup"><span data-stu-id="ee484-149">id</span></span>|<span data-ttu-id="ee484-150">字符串</span><span class="sxs-lookup"><span data-stu-id="ee484-150">String</span></span>|<span data-ttu-id="ee484-151">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ee484-151">Key of the entity.</span></span>|
|<span data-ttu-id="ee484-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee484-152">lastModifiedDateTime</span></span>|<span data-ttu-id="ee484-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee484-153">DateTimeOffset</span></span>|<span data-ttu-id="ee484-154">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ee484-154">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee484-155">关系</span><span class="sxs-lookup"><span data-stu-id="ee484-155">Relationships</span></span>
|<span data-ttu-id="ee484-156">关系</span><span class="sxs-lookup"><span data-stu-id="ee484-156">Relationship</span></span>|<span data-ttu-id="ee484-157">类型</span><span class="sxs-lookup"><span data-stu-id="ee484-157">Type</span></span>|<span data-ttu-id="ee484-158">说明</span><span class="sxs-lookup"><span data-stu-id="ee484-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee484-159">definitionValues</span><span class="sxs-lookup"><span data-stu-id="ee484-159">definitionValues</span></span>|<span data-ttu-id="ee484-160">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ee484-160">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="ee484-161">配置的启用或禁用组策略定义值的列表。</span><span class="sxs-lookup"><span data-stu-id="ee484-161">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="ee484-162">assignments</span><span class="sxs-lookup"><span data-stu-id="ee484-162">assignments</span></span>|<span data-ttu-id="ee484-163">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ee484-163">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ee484-164">配置的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="ee484-164">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee484-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee484-165">JSON Representation</span></span>
<span data-ttu-id="ee484-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee484-166">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




