---
title: groupPolicyConfiguration 资源类型
description: 组策略配置实体包含一个或多个组策略定义的配置值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d910bf8bdef34c60ca6bb66e1ce87ca9cf1d51ab
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941175"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="2f9d8-103">groupPolicyConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f9d8-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="2f9d8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f9d8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f9d8-106">组策略配置实体包含一个或多个组策略定义的配置值。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-106">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="2f9d8-107">方法</span><span class="sxs-lookup"><span data-stu-id="2f9d8-107">Methods</span></span>
|<span data-ttu-id="2f9d8-108">方法</span><span class="sxs-lookup"><span data-stu-id="2f9d8-108">Method</span></span>|<span data-ttu-id="2f9d8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2f9d8-109">Return Type</span></span>|<span data-ttu-id="2f9d8-110">说明</span><span class="sxs-lookup"><span data-stu-id="2f9d8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2f9d8-111">列出 groupPolicyConfigurations</span><span class="sxs-lookup"><span data-stu-id="2f9d8-111">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="2f9d8-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="2f9d8-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="2f9d8-113">列出[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-113">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="2f9d8-114">获取 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f9d8-114">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="2f9d8-115">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f9d8-115">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="2f9d8-116">读取[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-116">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="2f9d8-117">创建 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f9d8-117">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="2f9d8-118">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f9d8-118">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="2f9d8-119">创建新的[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-119">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="2f9d8-120">删除 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f9d8-120">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="2f9d8-121">无</span><span class="sxs-lookup"><span data-stu-id="2f9d8-121">None</span></span>|<span data-ttu-id="2f9d8-122">删除[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-122">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="2f9d8-123">更新 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f9d8-123">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="2f9d8-124">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f9d8-124">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="2f9d8-125">更新[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-125">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="2f9d8-126">分配操作</span><span class="sxs-lookup"><span data-stu-id="2f9d8-126">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="2f9d8-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="2f9d8-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2f9d8-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2f9d8-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2f9d8-129">属性</span><span class="sxs-lookup"><span data-stu-id="2f9d8-129">Properties</span></span>
|<span data-ttu-id="2f9d8-130">属性</span><span class="sxs-lookup"><span data-stu-id="2f9d8-130">Property</span></span>|<span data-ttu-id="2f9d8-131">类型</span><span class="sxs-lookup"><span data-stu-id="2f9d8-131">Type</span></span>|<span data-ttu-id="2f9d8-132">说明</span><span class="sxs-lookup"><span data-stu-id="2f9d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f9d8-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f9d8-133">createdDateTime</span></span>|<span data-ttu-id="2f9d8-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f9d8-134">DateTimeOffset</span></span>|<span data-ttu-id="2f9d8-135">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="2f9d8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2f9d8-136">displayName</span></span>|<span data-ttu-id="2f9d8-137">String</span><span class="sxs-lookup"><span data-stu-id="2f9d8-137">String</span></span>|<span data-ttu-id="2f9d8-138">用户提供的资源对象的名称。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="2f9d8-139">说明</span><span class="sxs-lookup"><span data-stu-id="2f9d8-139">description</span></span>|<span data-ttu-id="2f9d8-140">String</span><span class="sxs-lookup"><span data-stu-id="2f9d8-140">String</span></span>|<span data-ttu-id="2f9d8-141">用户提供的资源对象的说明。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="2f9d8-142">id</span><span class="sxs-lookup"><span data-stu-id="2f9d8-142">id</span></span>|<span data-ttu-id="2f9d8-143">字符串</span><span class="sxs-lookup"><span data-stu-id="2f9d8-143">String</span></span>|<span data-ttu-id="2f9d8-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-144">Key of the entity.</span></span>|
|<span data-ttu-id="2f9d8-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f9d8-145">lastModifiedDateTime</span></span>|<span data-ttu-id="2f9d8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f9d8-146">DateTimeOffset</span></span>|<span data-ttu-id="2f9d8-147">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f9d8-148">关系</span><span class="sxs-lookup"><span data-stu-id="2f9d8-148">Relationships</span></span>
|<span data-ttu-id="2f9d8-149">关系</span><span class="sxs-lookup"><span data-stu-id="2f9d8-149">Relationship</span></span>|<span data-ttu-id="2f9d8-150">类型</span><span class="sxs-lookup"><span data-stu-id="2f9d8-150">Type</span></span>|<span data-ttu-id="2f9d8-151">说明</span><span class="sxs-lookup"><span data-stu-id="2f9d8-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f9d8-152">definitionValues</span><span class="sxs-lookup"><span data-stu-id="2f9d8-152">definitionValues</span></span>|<span data-ttu-id="2f9d8-153">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="2f9d8-153">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="2f9d8-154">配置的启用或禁用组策略定义值的列表。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-154">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="2f9d8-155">assignments</span><span class="sxs-lookup"><span data-stu-id="2f9d8-155">assignments</span></span>|<span data-ttu-id="2f9d8-156">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="2f9d8-156">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2f9d8-157">配置的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-157">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f9d8-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f9d8-158">JSON Representation</span></span>
<span data-ttu-id="2f9d8-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f9d8-159">Here is a JSON representation of the resource.</span></span>
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
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




