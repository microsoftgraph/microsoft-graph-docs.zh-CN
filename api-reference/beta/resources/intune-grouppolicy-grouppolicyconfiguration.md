---
title: groupPolicyConfiguration 资源类型
description: 组策略配置实体包含一个或多个组策略定义的配置值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 544b743ab690521fee48e3609e2c62582131d6ef
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994242"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="b0bb2-103">groupPolicyConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0bb2-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="b0bb2-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0bb2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0bb2-106">组策略配置实体包含一个或多个组策略定义的配置值。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-106">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="b0bb2-107">方法</span><span class="sxs-lookup"><span data-stu-id="b0bb2-107">Methods</span></span>
|<span data-ttu-id="b0bb2-108">方法</span><span class="sxs-lookup"><span data-stu-id="b0bb2-108">Method</span></span>|<span data-ttu-id="b0bb2-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b0bb2-109">Return Type</span></span>|<span data-ttu-id="b0bb2-110">说明</span><span class="sxs-lookup"><span data-stu-id="b0bb2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b0bb2-111">列出 groupPolicyConfigurations</span><span class="sxs-lookup"><span data-stu-id="b0bb2-111">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="b0bb2-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="b0bb2-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="b0bb2-113">列出[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-113">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="b0bb2-114">获取 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0bb2-114">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="b0bb2-115">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0bb2-115">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="b0bb2-116">读取[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-116">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b0bb2-117">创建 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0bb2-117">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="b0bb2-118">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0bb2-118">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="b0bb2-119">创建新的[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-119">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b0bb2-120">删除 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0bb2-120">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="b0bb2-121">无</span><span class="sxs-lookup"><span data-stu-id="b0bb2-121">None</span></span>|<span data-ttu-id="b0bb2-122">删除[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-122">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="b0bb2-123">更新 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0bb2-123">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="b0bb2-124">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0bb2-124">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="b0bb2-125">更新[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-125">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b0bb2-126">分配操作</span><span class="sxs-lookup"><span data-stu-id="b0bb2-126">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="b0bb2-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="b0bb2-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b0bb2-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b0bb2-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b0bb2-129">属性</span><span class="sxs-lookup"><span data-stu-id="b0bb2-129">Properties</span></span>
|<span data-ttu-id="b0bb2-130">属性</span><span class="sxs-lookup"><span data-stu-id="b0bb2-130">Property</span></span>|<span data-ttu-id="b0bb2-131">类型</span><span class="sxs-lookup"><span data-stu-id="b0bb2-131">Type</span></span>|<span data-ttu-id="b0bb2-132">说明</span><span class="sxs-lookup"><span data-stu-id="b0bb2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0bb2-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0bb2-133">createdDateTime</span></span>|<span data-ttu-id="b0bb2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0bb2-134">DateTimeOffset</span></span>|<span data-ttu-id="b0bb2-135">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="b0bb2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b0bb2-136">displayName</span></span>|<span data-ttu-id="b0bb2-137">String</span><span class="sxs-lookup"><span data-stu-id="b0bb2-137">String</span></span>|<span data-ttu-id="b0bb2-138">用户提供的资源对象的名称。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="b0bb2-139">说明</span><span class="sxs-lookup"><span data-stu-id="b0bb2-139">description</span></span>|<span data-ttu-id="b0bb2-140">String</span><span class="sxs-lookup"><span data-stu-id="b0bb2-140">String</span></span>|<span data-ttu-id="b0bb2-141">用户提供的资源对象的说明。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="b0bb2-142">id</span><span class="sxs-lookup"><span data-stu-id="b0bb2-142">id</span></span>|<span data-ttu-id="b0bb2-143">字符串</span><span class="sxs-lookup"><span data-stu-id="b0bb2-143">String</span></span>|<span data-ttu-id="b0bb2-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-144">Key of the entity.</span></span>|
|<span data-ttu-id="b0bb2-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0bb2-145">lastModifiedDateTime</span></span>|<span data-ttu-id="b0bb2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0bb2-146">DateTimeOffset</span></span>|<span data-ttu-id="b0bb2-147">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0bb2-148">关系</span><span class="sxs-lookup"><span data-stu-id="b0bb2-148">Relationships</span></span>
|<span data-ttu-id="b0bb2-149">关系</span><span class="sxs-lookup"><span data-stu-id="b0bb2-149">Relationship</span></span>|<span data-ttu-id="b0bb2-150">类型</span><span class="sxs-lookup"><span data-stu-id="b0bb2-150">Type</span></span>|<span data-ttu-id="b0bb2-151">说明</span><span class="sxs-lookup"><span data-stu-id="b0bb2-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0bb2-152">definitionValues</span><span class="sxs-lookup"><span data-stu-id="b0bb2-152">definitionValues</span></span>|<span data-ttu-id="b0bb2-153">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="b0bb2-153">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="b0bb2-154">配置的启用或禁用组策略定义值的列表。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-154">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="b0bb2-155">assignments</span><span class="sxs-lookup"><span data-stu-id="b0bb2-155">assignments</span></span>|<span data-ttu-id="b0bb2-156">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="b0bb2-156">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b0bb2-157">配置的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-157">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0bb2-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0bb2-158">JSON Representation</span></span>
<span data-ttu-id="b0bb2-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0bb2-159">Here is a JSON representation of the resource.</span></span>
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





