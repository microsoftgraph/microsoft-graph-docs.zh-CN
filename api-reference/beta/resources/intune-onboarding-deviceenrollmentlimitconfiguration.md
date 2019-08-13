---
title: deviceEnrollmentLimitConfiguration 资源类型
description: 限制用户可以注册的设备数量的设备注册配置
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f4b77ecaeeb23182be2fe867c73675a294528048
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374349"
---
# <a name="deviceenrollmentlimitconfiguration-resource-type"></a><span data-ttu-id="6409e-103">deviceEnrollmentLimitConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="6409e-103">deviceEnrollmentLimitConfiguration resource type</span></span>

> <span data-ttu-id="6409e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6409e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6409e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6409e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6409e-106">限制用户可以注册的设备数量的设备注册配置</span><span class="sxs-lookup"><span data-stu-id="6409e-106">Device Enrollment Configuration that restricts the number of devices a user can enroll</span></span>


<span data-ttu-id="6409e-107">继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6409e-107">Inherits from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6409e-108">方法</span><span class="sxs-lookup"><span data-stu-id="6409e-108">Methods</span></span>
|<span data-ttu-id="6409e-109">方法</span><span class="sxs-lookup"><span data-stu-id="6409e-109">Method</span></span>|<span data-ttu-id="6409e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6409e-110">Return Type</span></span>|<span data-ttu-id="6409e-111">说明</span><span class="sxs-lookup"><span data-stu-id="6409e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6409e-112">列出 deviceEnrollmentLimitConfigurations</span><span class="sxs-lookup"><span data-stu-id="6409e-112">List deviceEnrollmentLimitConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-list.md)|<span data-ttu-id="6409e-113">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6409e-113">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) collection</span></span>|<span data-ttu-id="6409e-114">列出 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6409e-114">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="6409e-115">获取 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="6409e-115">Get deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-get.md)|[<span data-ttu-id="6409e-116">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="6409e-116">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="6409e-117">读取 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6409e-117">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="6409e-118">创建 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="6409e-118">Create deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-create.md)|[<span data-ttu-id="6409e-119">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="6409e-119">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="6409e-120">创建新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6409e-120">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="6409e-121">删除 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="6409e-121">Delete deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-delete.md)|<span data-ttu-id="6409e-122">无</span><span class="sxs-lookup"><span data-stu-id="6409e-122">None</span></span>|<span data-ttu-id="6409e-123">删除 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="6409e-123">Deletes a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>|
|[<span data-ttu-id="6409e-124">更新 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="6409e-124">Update deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-update.md)|[<span data-ttu-id="6409e-125">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="6409e-125">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="6409e-126">更新 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6409e-126">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6409e-127">属性</span><span class="sxs-lookup"><span data-stu-id="6409e-127">Properties</span></span>
|<span data-ttu-id="6409e-128">属性</span><span class="sxs-lookup"><span data-stu-id="6409e-128">Property</span></span>|<span data-ttu-id="6409e-129">类型</span><span class="sxs-lookup"><span data-stu-id="6409e-129">Type</span></span>|<span data-ttu-id="6409e-130">说明</span><span class="sxs-lookup"><span data-stu-id="6409e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6409e-131">id</span><span class="sxs-lookup"><span data-stu-id="6409e-131">id</span></span>|<span data-ttu-id="6409e-132">字符串</span><span class="sxs-lookup"><span data-stu-id="6409e-132">String</span></span>|<span data-ttu-id="6409e-133">继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="6409e-133">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6409e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6409e-134">displayName</span></span>|<span data-ttu-id="6409e-135">String</span><span class="sxs-lookup"><span data-stu-id="6409e-135">String</span></span>|<span data-ttu-id="6409e-136">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="6409e-136">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6409e-137">说明</span><span class="sxs-lookup"><span data-stu-id="6409e-137">description</span></span>|<span data-ttu-id="6409e-138">String</span><span class="sxs-lookup"><span data-stu-id="6409e-138">String</span></span>|<span data-ttu-id="6409e-139">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="6409e-139">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6409e-140">priority</span><span class="sxs-lookup"><span data-stu-id="6409e-140">priority</span></span>|<span data-ttu-id="6409e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6409e-141">Int32</span></span>|<span data-ttu-id="6409e-142">当用户存在于分配有注册配置的多个组中时, 将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="6409e-142">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="6409e-143">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="6409e-143">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="6409e-144">继承自 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6409e-144">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6409e-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6409e-145">createdDateTime</span></span>|<span data-ttu-id="6409e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6409e-146">DateTimeOffset</span></span>|<span data-ttu-id="6409e-147">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="6409e-147">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6409e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6409e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6409e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6409e-149">DateTimeOffset</span></span>|<span data-ttu-id="6409e-150">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="6409e-150">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6409e-151">version</span><span class="sxs-lookup"><span data-stu-id="6409e-151">version</span></span>|<span data-ttu-id="6409e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6409e-152">Int32</span></span>|<span data-ttu-id="6409e-153">继承自[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="6409e-153">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="6409e-154">limit</span><span class="sxs-lookup"><span data-stu-id="6409e-154">limit</span></span>|<span data-ttu-id="6409e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="6409e-155">Int32</span></span>|<span data-ttu-id="6409e-156">用户可注册的最大设备数</span><span class="sxs-lookup"><span data-stu-id="6409e-156">The maximum number of devices that a user can enroll</span></span>|

## <a name="relationships"></a><span data-ttu-id="6409e-157">关系</span><span class="sxs-lookup"><span data-stu-id="6409e-157">Relationships</span></span>
|<span data-ttu-id="6409e-158">关系</span><span class="sxs-lookup"><span data-stu-id="6409e-158">Relationship</span></span>|<span data-ttu-id="6409e-159">类型</span><span class="sxs-lookup"><span data-stu-id="6409e-159">Type</span></span>|<span data-ttu-id="6409e-160">说明</span><span class="sxs-lookup"><span data-stu-id="6409e-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6409e-161">assignments</span><span class="sxs-lookup"><span data-stu-id="6409e-161">assignments</span></span>|<span data-ttu-id="6409e-162">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6409e-162">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="6409e-163">从[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)继承的设备配置文件组的组分配列表</span><span class="sxs-lookup"><span data-stu-id="6409e-163">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6409e-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6409e-164">JSON Representation</span></span>
<span data-ttu-id="6409e-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6409e-165">Here is a JSON representation of the resource.</span></span>
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



