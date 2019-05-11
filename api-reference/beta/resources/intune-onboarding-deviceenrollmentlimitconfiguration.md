---
title: deviceEnrollmentLimitConfiguration 资源类型
description: 限制用户可以注册的设备数量的设备注册配置
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ea20766d7240b1d3087da84f753b8ad9fb441d2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940468"
---
# <a name="deviceenrollmentlimitconfiguration-resource-type"></a><span data-ttu-id="89c49-103">deviceEnrollmentLimitConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="89c49-103">deviceEnrollmentLimitConfiguration resource type</span></span>

> <span data-ttu-id="89c49-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="89c49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89c49-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89c49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89c49-106">限制用户可以注册的设备数量的设备注册配置</span><span class="sxs-lookup"><span data-stu-id="89c49-106">Device Enrollment Configuration that restricts the number of devices a user can enroll</span></span>


<span data-ttu-id="89c49-107">继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89c49-107">Inherits from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="89c49-108">方法</span><span class="sxs-lookup"><span data-stu-id="89c49-108">Methods</span></span>
|<span data-ttu-id="89c49-109">方法</span><span class="sxs-lookup"><span data-stu-id="89c49-109">Method</span></span>|<span data-ttu-id="89c49-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="89c49-110">Return Type</span></span>|<span data-ttu-id="89c49-111">说明</span><span class="sxs-lookup"><span data-stu-id="89c49-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="89c49-112">列出 deviceEnrollmentLimitConfigurations</span><span class="sxs-lookup"><span data-stu-id="89c49-112">List deviceEnrollmentLimitConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-list.md)|<span data-ttu-id="89c49-113">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89c49-113">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) collection</span></span>|<span data-ttu-id="89c49-114">列出 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="89c49-114">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="89c49-115">获取 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="89c49-115">Get deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-get.md)|[<span data-ttu-id="89c49-116">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="89c49-116">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="89c49-117">读取 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="89c49-117">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="89c49-118">创建 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="89c49-118">Create deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-create.md)|[<span data-ttu-id="89c49-119">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="89c49-119">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="89c49-120">创建新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89c49-120">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="89c49-121">删除 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="89c49-121">Delete deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-delete.md)|<span data-ttu-id="89c49-122">无</span><span class="sxs-lookup"><span data-stu-id="89c49-122">None</span></span>|<span data-ttu-id="89c49-123">删除 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="89c49-123">Deletes a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>|
|[<span data-ttu-id="89c49-124">更新 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="89c49-124">Update deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-update.md)|[<span data-ttu-id="89c49-125">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="89c49-125">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="89c49-126">更新 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="89c49-126">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="89c49-127">属性</span><span class="sxs-lookup"><span data-stu-id="89c49-127">Properties</span></span>
|<span data-ttu-id="89c49-128">属性</span><span class="sxs-lookup"><span data-stu-id="89c49-128">Property</span></span>|<span data-ttu-id="89c49-129">类型</span><span class="sxs-lookup"><span data-stu-id="89c49-129">Type</span></span>|<span data-ttu-id="89c49-130">说明</span><span class="sxs-lookup"><span data-stu-id="89c49-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89c49-131">id</span><span class="sxs-lookup"><span data-stu-id="89c49-131">id</span></span>|<span data-ttu-id="89c49-132">字符串</span><span class="sxs-lookup"><span data-stu-id="89c49-132">String</span></span>|<span data-ttu-id="89c49-133">继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="89c49-133">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="89c49-134">displayName</span><span class="sxs-lookup"><span data-stu-id="89c49-134">displayName</span></span>|<span data-ttu-id="89c49-135">String</span><span class="sxs-lookup"><span data-stu-id="89c49-135">String</span></span>|<span data-ttu-id="89c49-136">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="89c49-136">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="89c49-137">说明</span><span class="sxs-lookup"><span data-stu-id="89c49-137">description</span></span>|<span data-ttu-id="89c49-138">String</span><span class="sxs-lookup"><span data-stu-id="89c49-138">String</span></span>|<span data-ttu-id="89c49-139">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="89c49-139">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="89c49-140">priority</span><span class="sxs-lookup"><span data-stu-id="89c49-140">priority</span></span>|<span data-ttu-id="89c49-141">Int32</span><span class="sxs-lookup"><span data-stu-id="89c49-141">Int32</span></span>|<span data-ttu-id="89c49-142">当用户存在于分配有注册配置的多个组中时, 将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="89c49-142">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="89c49-143">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="89c49-143">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="89c49-144">继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89c49-144">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="89c49-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89c49-145">createdDateTime</span></span>|<span data-ttu-id="89c49-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89c49-146">DateTimeOffset</span></span>|<span data-ttu-id="89c49-147">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="89c49-147">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="89c49-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89c49-148">lastModifiedDateTime</span></span>|<span data-ttu-id="89c49-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89c49-149">DateTimeOffset</span></span>|<span data-ttu-id="89c49-150">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="89c49-150">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="89c49-151">version</span><span class="sxs-lookup"><span data-stu-id="89c49-151">version</span></span>|<span data-ttu-id="89c49-152">Int32</span><span class="sxs-lookup"><span data-stu-id="89c49-152">Int32</span></span>|<span data-ttu-id="89c49-153">继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="89c49-153">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="89c49-154">limit</span><span class="sxs-lookup"><span data-stu-id="89c49-154">limit</span></span>|<span data-ttu-id="89c49-155">Int32</span><span class="sxs-lookup"><span data-stu-id="89c49-155">Int32</span></span>|<span data-ttu-id="89c49-156">用户可注册的最大设备数</span><span class="sxs-lookup"><span data-stu-id="89c49-156">The maximum number of devices that a user can enroll</span></span>|

## <a name="relationships"></a><span data-ttu-id="89c49-157">关系</span><span class="sxs-lookup"><span data-stu-id="89c49-157">Relationships</span></span>
|<span data-ttu-id="89c49-158">关系</span><span class="sxs-lookup"><span data-stu-id="89c49-158">Relationship</span></span>|<span data-ttu-id="89c49-159">类型</span><span class="sxs-lookup"><span data-stu-id="89c49-159">Type</span></span>|<span data-ttu-id="89c49-160">说明</span><span class="sxs-lookup"><span data-stu-id="89c49-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89c49-161">assignments</span><span class="sxs-lookup"><span data-stu-id="89c49-161">assignments</span></span>|<span data-ttu-id="89c49-162">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89c49-162">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="89c49-163">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备配置文件组的组分配列表</span><span class="sxs-lookup"><span data-stu-id="89c49-163">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89c49-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89c49-164">JSON Representation</span></span>
<span data-ttu-id="89c49-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89c49-165">Here is a JSON representation of the resource.</span></span>
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




