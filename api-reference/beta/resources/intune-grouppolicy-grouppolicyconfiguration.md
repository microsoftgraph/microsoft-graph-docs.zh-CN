---
title: groupPolicyConfiguration 资源类型
description: 组策略配置实体包含一个或多个组策略定义的配置的的值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be3b43ab0e9e3f87f53ed0dae144f2b6f4dce7b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431395"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="d0fb0-103">groupPolicyConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0fb0-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="d0fb0-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d0fb0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0fb0-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0fb0-107">组策略配置实体包含一个或多个组策略定义的配置的的值。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-107">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="d0fb0-108">方法</span><span class="sxs-lookup"><span data-stu-id="d0fb0-108">Methods</span></span>
|<span data-ttu-id="d0fb0-109">方法</span><span class="sxs-lookup"><span data-stu-id="d0fb0-109">Method</span></span>|<span data-ttu-id="d0fb0-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d0fb0-110">Return Type</span></span>|<span data-ttu-id="d0fb0-111">说明</span><span class="sxs-lookup"><span data-stu-id="d0fb0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d0fb0-112">列表 groupPolicyConfigurations</span><span class="sxs-lookup"><span data-stu-id="d0fb0-112">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="d0fb0-113">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="d0fb0-113">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="d0fb0-114">列出属性和[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-114">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d0fb0-115">获取 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0fb0-115">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="d0fb0-116">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0fb0-116">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="d0fb0-117">读取属性和[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-117">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d0fb0-118">创建 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0fb0-118">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="d0fb0-119">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0fb0-119">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="d0fb0-120">创建新的[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-120">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d0fb0-121">删除 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0fb0-121">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="d0fb0-122">无</span><span class="sxs-lookup"><span data-stu-id="d0fb0-122">None</span></span>|<span data-ttu-id="d0fb0-123">删除[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-123">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="d0fb0-124">更新 groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0fb0-124">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="d0fb0-125">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0fb0-125">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="d0fb0-126">更新[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-126">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d0fb0-127">assign 操作</span><span class="sxs-lookup"><span data-stu-id="d0fb0-127">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="d0fb0-128">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="d0fb0-128">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d0fb0-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d0fb0-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d0fb0-130">属性</span><span class="sxs-lookup"><span data-stu-id="d0fb0-130">Properties</span></span>
|<span data-ttu-id="d0fb0-131">属性</span><span class="sxs-lookup"><span data-stu-id="d0fb0-131">Property</span></span>|<span data-ttu-id="d0fb0-132">类型</span><span class="sxs-lookup"><span data-stu-id="d0fb0-132">Type</span></span>|<span data-ttu-id="d0fb0-133">说明</span><span class="sxs-lookup"><span data-stu-id="d0fb0-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0fb0-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0fb0-134">createdDateTime</span></span>|<span data-ttu-id="d0fb0-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0fb0-135">DateTimeOffset</span></span>|<span data-ttu-id="d0fb0-136">日期和时间创建对象。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-136">The date and time the object was created.</span></span>|
|<span data-ttu-id="d0fb0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d0fb0-137">displayName</span></span>|<span data-ttu-id="d0fb0-138">String</span><span class="sxs-lookup"><span data-stu-id="d0fb0-138">String</span></span>|<span data-ttu-id="d0fb0-139">用户提供的资源对象的名称。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-139">User provided name for the resource object.</span></span>|
|<span data-ttu-id="d0fb0-140">说明</span><span class="sxs-lookup"><span data-stu-id="d0fb0-140">description</span></span>|<span data-ttu-id="d0fb0-141">String</span><span class="sxs-lookup"><span data-stu-id="d0fb0-141">String</span></span>|<span data-ttu-id="d0fb0-142">用户提供的资源对象的说明。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-142">User provided description for the resource object.</span></span>|
|<span data-ttu-id="d0fb0-143">id</span><span class="sxs-lookup"><span data-stu-id="d0fb0-143">id</span></span>|<span data-ttu-id="d0fb0-144">String</span><span class="sxs-lookup"><span data-stu-id="d0fb0-144">String</span></span>|<span data-ttu-id="d0fb0-145">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-145">Key of the entity.</span></span>|
|<span data-ttu-id="d0fb0-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0fb0-146">lastModifiedDateTime</span></span>|<span data-ttu-id="d0fb0-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0fb0-147">DateTimeOffset</span></span>|<span data-ttu-id="d0fb0-148">日期和实体上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-148">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0fb0-149">关系</span><span class="sxs-lookup"><span data-stu-id="d0fb0-149">Relationships</span></span>
|<span data-ttu-id="d0fb0-150">关系</span><span class="sxs-lookup"><span data-stu-id="d0fb0-150">Relationship</span></span>|<span data-ttu-id="d0fb0-151">类型</span><span class="sxs-lookup"><span data-stu-id="d0fb0-151">Type</span></span>|<span data-ttu-id="d0fb0-152">说明</span><span class="sxs-lookup"><span data-stu-id="d0fb0-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0fb0-153">definitionValues</span><span class="sxs-lookup"><span data-stu-id="d0fb0-153">definitionValues</span></span>|<span data-ttu-id="d0fb0-154">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="d0fb0-154">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="d0fb0-155">列表中的启用或禁用配置组策略定义值。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-155">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="d0fb0-156">assignments</span><span class="sxs-lookup"><span data-stu-id="d0fb0-156">assignments</span></span>|<span data-ttu-id="d0fb0-157">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="d0fb0-157">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d0fb0-158">为配置的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-158">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0fb0-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0fb0-159">JSON Representation</span></span>
<span data-ttu-id="d0fb0-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0fb0-160">Here is a JSON representation of the resource.</span></span>
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




