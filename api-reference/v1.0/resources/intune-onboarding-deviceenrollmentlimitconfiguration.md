---
title: deviceEnrollmentLimitConfiguration 资源类型
description: 设备注册 限制用户可以注册的设备数量的配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 25e4951e48d5c97d6a07a63dc87b6d38a77b4c77
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751620"
---
# <a name="deviceenrollmentlimitconfiguration-resource-type"></a><span data-ttu-id="622aa-103">deviceEnrollmentLimitConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="622aa-103">deviceEnrollmentLimitConfiguration resource type</span></span>

<span data-ttu-id="622aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="622aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="622aa-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="622aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="622aa-106">设备注册 限制用户可以注册的设备数量的配置</span><span class="sxs-lookup"><span data-stu-id="622aa-106">Device Enrollment Configuration that restricts the number of devices a user can enroll</span></span>


<span data-ttu-id="622aa-107">继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="622aa-107">Inherits from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="622aa-108">Methods</span><span class="sxs-lookup"><span data-stu-id="622aa-108">Methods</span></span>
|<span data-ttu-id="622aa-109">方法</span><span class="sxs-lookup"><span data-stu-id="622aa-109">Method</span></span>|<span data-ttu-id="622aa-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="622aa-110">Return Type</span></span>|<span data-ttu-id="622aa-111">Description</span><span class="sxs-lookup"><span data-stu-id="622aa-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="622aa-112">列出 deviceEnrollmentLimitConfigurations</span><span class="sxs-lookup"><span data-stu-id="622aa-112">List deviceEnrollmentLimitConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-list.md)|<span data-ttu-id="622aa-113">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="622aa-113">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) collection</span></span>|<span data-ttu-id="622aa-114">列出 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="622aa-114">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="622aa-115">获取 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="622aa-115">Get deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-get.md)|[<span data-ttu-id="622aa-116">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="622aa-116">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="622aa-117">读取 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="622aa-117">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="622aa-118">创建 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="622aa-118">Create deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-create.md)|[<span data-ttu-id="622aa-119">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="622aa-119">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="622aa-120">创建新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="622aa-120">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="622aa-121">删除 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="622aa-121">Delete deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-delete.md)|<span data-ttu-id="622aa-122">无</span><span class="sxs-lookup"><span data-stu-id="622aa-122">None</span></span>|<span data-ttu-id="622aa-123">删除 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="622aa-123">Deletes a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>|
|[<span data-ttu-id="622aa-124">更新 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="622aa-124">Update deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-update.md)|[<span data-ttu-id="622aa-125">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="622aa-125">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="622aa-126">更新 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="622aa-126">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="622aa-127">属性</span><span class="sxs-lookup"><span data-stu-id="622aa-127">Properties</span></span>
|<span data-ttu-id="622aa-128">属性</span><span class="sxs-lookup"><span data-stu-id="622aa-128">Property</span></span>|<span data-ttu-id="622aa-129">类型</span><span class="sxs-lookup"><span data-stu-id="622aa-129">Type</span></span>|<span data-ttu-id="622aa-130">说明</span><span class="sxs-lookup"><span data-stu-id="622aa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="622aa-131">id</span><span class="sxs-lookup"><span data-stu-id="622aa-131">id</span></span>|<span data-ttu-id="622aa-132">String</span><span class="sxs-lookup"><span data-stu-id="622aa-132">String</span></span>|<span data-ttu-id="622aa-133">帐户的唯一标识符 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="622aa-133">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="622aa-134">displayName</span><span class="sxs-lookup"><span data-stu-id="622aa-134">displayName</span></span>|<span data-ttu-id="622aa-135">String</span><span class="sxs-lookup"><span data-stu-id="622aa-135">String</span></span>|<span data-ttu-id="622aa-136">设备显示名称的配置类型 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="622aa-136">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="622aa-137">说明</span><span class="sxs-lookup"><span data-stu-id="622aa-137">description</span></span>|<span data-ttu-id="622aa-138">String</span><span class="sxs-lookup"><span data-stu-id="622aa-138">String</span></span>|<span data-ttu-id="622aa-139">设备注册配置的说明 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="622aa-139">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="622aa-140">priority</span><span class="sxs-lookup"><span data-stu-id="622aa-140">priority</span></span>|<span data-ttu-id="622aa-141">Int32</span><span class="sxs-lookup"><span data-stu-id="622aa-141">Int32</span></span>|<span data-ttu-id="622aa-142">如果用户位于分配了注册配置的多个组中，则使用优先级。</span><span class="sxs-lookup"><span data-stu-id="622aa-142">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="622aa-143">用户仅受优先级值最低的配置使用。</span><span class="sxs-lookup"><span data-stu-id="622aa-143">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="622aa-144">继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="622aa-144">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="622aa-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="622aa-145">createdDateTime</span></span>|<span data-ttu-id="622aa-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="622aa-146">DateTimeOffset</span></span>|<span data-ttu-id="622aa-147">设备注册配置的创建日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="622aa-147">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="622aa-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="622aa-148">lastModifiedDateTime</span></span>|<span data-ttu-id="622aa-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="622aa-149">DateTimeOffset</span></span>|<span data-ttu-id="622aa-150">设备注册配置的上次修改日期时间（UTC）继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="622aa-150">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="622aa-151">version</span><span class="sxs-lookup"><span data-stu-id="622aa-151">version</span></span>|<span data-ttu-id="622aa-152">Int32</span><span class="sxs-lookup"><span data-stu-id="622aa-152">Int32</span></span>|<span data-ttu-id="622aa-153">设备注册配置的版本 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="622aa-153">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="622aa-154">limit</span><span class="sxs-lookup"><span data-stu-id="622aa-154">limit</span></span>|<span data-ttu-id="622aa-155">Int32</span><span class="sxs-lookup"><span data-stu-id="622aa-155">Int32</span></span>|<span data-ttu-id="622aa-156">用户可以注册的最大设备数</span><span class="sxs-lookup"><span data-stu-id="622aa-156">The maximum number of devices that a user can enroll</span></span>|

## <a name="relationships"></a><span data-ttu-id="622aa-157">关系</span><span class="sxs-lookup"><span data-stu-id="622aa-157">Relationships</span></span>
|<span data-ttu-id="622aa-158">关系</span><span class="sxs-lookup"><span data-stu-id="622aa-158">Relationship</span></span>|<span data-ttu-id="622aa-159">类型</span><span class="sxs-lookup"><span data-stu-id="622aa-159">Type</span></span>|<span data-ttu-id="622aa-160">Description</span><span class="sxs-lookup"><span data-stu-id="622aa-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="622aa-161">assignments</span><span class="sxs-lookup"><span data-stu-id="622aa-161">assignments</span></span>|<span data-ttu-id="622aa-162">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="622aa-162">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="622aa-163">设备配置文件的组分配列表 继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="622aa-163">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="622aa-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="622aa-164">JSON Representation</span></span>
<span data-ttu-id="622aa-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="622aa-165">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentLimitConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "limit": 1024
}
```




