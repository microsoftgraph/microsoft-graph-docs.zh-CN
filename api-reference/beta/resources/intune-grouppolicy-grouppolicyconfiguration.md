---
title: groupPolicyConfiguration 资源类型
description: 组策略配置实体包含一个或多个组策略定义的配置值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c9ee783ffa3e037243a78cd49187511797e221de
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088068"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="3e2c6-103">groupPolicyConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e2c6-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="3e2c6-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e2c6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e2c6-106">组策略配置实体包含一个或多个组策略定义的配置值。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-106">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="3e2c6-107">方法</span><span class="sxs-lookup"><span data-stu-id="3e2c6-107">Methods</span></span>
|<span data-ttu-id="3e2c6-108">方法</span><span class="sxs-lookup"><span data-stu-id="3e2c6-108">Method</span></span>|<span data-ttu-id="3e2c6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3e2c6-109">Return Type</span></span>|<span data-ttu-id="3e2c6-110">说明</span><span class="sxs-lookup"><span data-stu-id="3e2c6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3e2c6-111">列出 groupPolicyConfigurations</span><span class="sxs-lookup"><span data-stu-id="3e2c6-111">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="3e2c6-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="3e2c6-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="3e2c6-113">列出[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-113">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="3e2c6-114">获取 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e2c6-114">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="3e2c6-115">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e2c6-115">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="3e2c6-116">读取[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-116">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="3e2c6-117">创建 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e2c6-117">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="3e2c6-118">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e2c6-118">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="3e2c6-119">创建新的[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-119">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="3e2c6-120">删除 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e2c6-120">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="3e2c6-121">无</span><span class="sxs-lookup"><span data-stu-id="3e2c6-121">None</span></span>|<span data-ttu-id="3e2c6-122">删除[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-122">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="3e2c6-123">更新 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e2c6-123">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="3e2c6-124">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e2c6-124">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="3e2c6-125">更新[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-125">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="3e2c6-126">分配操作</span><span class="sxs-lookup"><span data-stu-id="3e2c6-126">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="3e2c6-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="3e2c6-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3e2c6-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3e2c6-128">Not yet documented</span></span>|
|[<span data-ttu-id="3e2c6-129">updateDefinitionValues 操作</span><span class="sxs-lookup"><span data-stu-id="3e2c6-129">updateDefinitionValues action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-updatedefinitionvalues.md)|<span data-ttu-id="3e2c6-130">无</span><span class="sxs-lookup"><span data-stu-id="3e2c6-130">None</span></span>|<span data-ttu-id="3e2c6-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3e2c6-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3e2c6-132">属性</span><span class="sxs-lookup"><span data-stu-id="3e2c6-132">Properties</span></span>
|<span data-ttu-id="3e2c6-133">属性</span><span class="sxs-lookup"><span data-stu-id="3e2c6-133">Property</span></span>|<span data-ttu-id="3e2c6-134">类型</span><span class="sxs-lookup"><span data-stu-id="3e2c6-134">Type</span></span>|<span data-ttu-id="3e2c6-135">说明</span><span class="sxs-lookup"><span data-stu-id="3e2c6-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e2c6-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e2c6-136">createdDateTime</span></span>|<span data-ttu-id="3e2c6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e2c6-137">DateTimeOffset</span></span>|<span data-ttu-id="3e2c6-138">对象的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="3e2c6-139">displayName</span><span class="sxs-lookup"><span data-stu-id="3e2c6-139">displayName</span></span>|<span data-ttu-id="3e2c6-140">String</span><span class="sxs-lookup"><span data-stu-id="3e2c6-140">String</span></span>|<span data-ttu-id="3e2c6-141">用户提供的资源对象的名称。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-141">User provided name for the resource object.</span></span>|
|<span data-ttu-id="3e2c6-142">说明</span><span class="sxs-lookup"><span data-stu-id="3e2c6-142">description</span></span>|<span data-ttu-id="3e2c6-143">String</span><span class="sxs-lookup"><span data-stu-id="3e2c6-143">String</span></span>|<span data-ttu-id="3e2c6-144">用户提供的资源对象的说明。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-144">User provided description for the resource object.</span></span>|
|<span data-ttu-id="3e2c6-145">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3e2c6-145">roleScopeTagIds</span></span>|<span data-ttu-id="3e2c6-146">String collection</span><span class="sxs-lookup"><span data-stu-id="3e2c6-146">String collection</span></span>|<span data-ttu-id="3e2c6-147">配置的作用域标记列表。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-147">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="3e2c6-148">id</span><span class="sxs-lookup"><span data-stu-id="3e2c6-148">id</span></span>|<span data-ttu-id="3e2c6-149">字符串</span><span class="sxs-lookup"><span data-stu-id="3e2c6-149">String</span></span>|<span data-ttu-id="3e2c6-150">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-150">Key of the entity.</span></span>|
|<span data-ttu-id="3e2c6-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e2c6-151">lastModifiedDateTime</span></span>|<span data-ttu-id="3e2c6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e2c6-152">DateTimeOffset</span></span>|<span data-ttu-id="3e2c6-153">上次修改实体的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-153">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e2c6-154">关系</span><span class="sxs-lookup"><span data-stu-id="3e2c6-154">Relationships</span></span>
|<span data-ttu-id="3e2c6-155">关系</span><span class="sxs-lookup"><span data-stu-id="3e2c6-155">Relationship</span></span>|<span data-ttu-id="3e2c6-156">类型</span><span class="sxs-lookup"><span data-stu-id="3e2c6-156">Type</span></span>|<span data-ttu-id="3e2c6-157">描述</span><span class="sxs-lookup"><span data-stu-id="3e2c6-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e2c6-158">definitionValues</span><span class="sxs-lookup"><span data-stu-id="3e2c6-158">definitionValues</span></span>|<span data-ttu-id="3e2c6-159">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="3e2c6-159">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="3e2c6-160">配置的启用或禁用组策略定义值的列表。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-160">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="3e2c6-161">assignments</span><span class="sxs-lookup"><span data-stu-id="3e2c6-161">assignments</span></span>|<span data-ttu-id="3e2c6-162">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="3e2c6-162">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3e2c6-163">配置的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-163">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e2c6-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e2c6-164">JSON Representation</span></span>
<span data-ttu-id="3e2c6-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e2c6-165">Here is a JSON representation of the resource.</span></span>
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



