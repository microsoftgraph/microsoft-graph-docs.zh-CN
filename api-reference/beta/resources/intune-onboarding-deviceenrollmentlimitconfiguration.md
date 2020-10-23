---
title: deviceEnrollmentLimitConfiguration 资源类型
description: 限制用户可以注册的设备数量的设备注册配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5f5dcc20e7f7ddfc26b670b276843379686f8316
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697271"
---
# <a name="deviceenrollmentlimitconfiguration-resource-type"></a><span data-ttu-id="f2961-103">deviceEnrollmentLimitConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2961-103">deviceEnrollmentLimitConfiguration resource type</span></span>

<span data-ttu-id="f2961-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2961-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2961-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f2961-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2961-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f2961-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2961-107">限制用户可以注册的设备数量的设备注册配置</span><span class="sxs-lookup"><span data-stu-id="f2961-107">Device Enrollment Configuration that restricts the number of devices a user can enroll</span></span>


<span data-ttu-id="f2961-108">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2961-108">Inherits from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="f2961-109">Methods</span><span class="sxs-lookup"><span data-stu-id="f2961-109">Methods</span></span>
|<span data-ttu-id="f2961-110">方法</span><span class="sxs-lookup"><span data-stu-id="f2961-110">Method</span></span>|<span data-ttu-id="f2961-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="f2961-111">Return Type</span></span>|<span data-ttu-id="f2961-112">说明</span><span class="sxs-lookup"><span data-stu-id="f2961-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f2961-113">列出 deviceEnrollmentLimitConfigurations</span><span class="sxs-lookup"><span data-stu-id="f2961-113">List deviceEnrollmentLimitConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-list.md)|<span data-ttu-id="f2961-114">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2961-114">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) collection</span></span>|<span data-ttu-id="f2961-115">列出 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f2961-115">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="f2961-116">获取 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2961-116">Get deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-get.md)|[<span data-ttu-id="f2961-117">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2961-117">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="f2961-118">读取 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f2961-118">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="f2961-119">创建 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2961-119">Create deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-create.md)|[<span data-ttu-id="f2961-120">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2961-120">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="f2961-121">创建新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2961-121">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="f2961-122">删除 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2961-122">Delete deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-delete.md)|<span data-ttu-id="f2961-123">无</span><span class="sxs-lookup"><span data-stu-id="f2961-123">None</span></span>|<span data-ttu-id="f2961-124">删除 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="f2961-124">Deletes a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>|
|[<span data-ttu-id="f2961-125">更新 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2961-125">Update deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-update.md)|[<span data-ttu-id="f2961-126">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2961-126">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="f2961-127">更新 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f2961-127">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2961-128">属性</span><span class="sxs-lookup"><span data-stu-id="f2961-128">Properties</span></span>
|<span data-ttu-id="f2961-129">属性</span><span class="sxs-lookup"><span data-stu-id="f2961-129">Property</span></span>|<span data-ttu-id="f2961-130">类型</span><span class="sxs-lookup"><span data-stu-id="f2961-130">Type</span></span>|<span data-ttu-id="f2961-131">说明</span><span class="sxs-lookup"><span data-stu-id="f2961-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2961-132">id</span><span class="sxs-lookup"><span data-stu-id="f2961-132">id</span></span>|<span data-ttu-id="f2961-133">String</span><span class="sxs-lookup"><span data-stu-id="f2961-133">String</span></span>|<span data-ttu-id="f2961-134">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="f2961-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f2961-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f2961-135">displayName</span></span>|<span data-ttu-id="f2961-136">String</span><span class="sxs-lookup"><span data-stu-id="f2961-136">String</span></span>|<span data-ttu-id="f2961-137">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="f2961-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f2961-138">说明</span><span class="sxs-lookup"><span data-stu-id="f2961-138">description</span></span>|<span data-ttu-id="f2961-139">String</span><span class="sxs-lookup"><span data-stu-id="f2961-139">String</span></span>|<span data-ttu-id="f2961-140">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="f2961-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f2961-141">priority</span><span class="sxs-lookup"><span data-stu-id="f2961-141">priority</span></span>|<span data-ttu-id="f2961-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f2961-142">Int32</span></span>|<span data-ttu-id="f2961-143">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="f2961-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="f2961-144">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="f2961-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="f2961-145">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2961-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f2961-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2961-146">createdDateTime</span></span>|<span data-ttu-id="f2961-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2961-147">DateTimeOffset</span></span>|<span data-ttu-id="f2961-148">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="f2961-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f2961-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2961-149">lastModifiedDateTime</span></span>|<span data-ttu-id="f2961-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2961-150">DateTimeOffset</span></span>|<span data-ttu-id="f2961-151">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="f2961-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f2961-152">version</span><span class="sxs-lookup"><span data-stu-id="f2961-152">version</span></span>|<span data-ttu-id="f2961-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f2961-153">Int32</span></span>|<span data-ttu-id="f2961-154">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="f2961-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f2961-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f2961-155">roleScopeTagIds</span></span>|<span data-ttu-id="f2961-156">String collection</span><span class="sxs-lookup"><span data-stu-id="f2961-156">String collection</span></span>|<span data-ttu-id="f2961-157">注册限制的可选角色范围标记。</span><span class="sxs-lookup"><span data-stu-id="f2961-157">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="f2961-158">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2961-158">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="f2961-159">limit</span><span class="sxs-lookup"><span data-stu-id="f2961-159">limit</span></span>|<span data-ttu-id="f2961-160">Int32</span><span class="sxs-lookup"><span data-stu-id="f2961-160">Int32</span></span>|<span data-ttu-id="f2961-161">用户可注册的最大设备数</span><span class="sxs-lookup"><span data-stu-id="f2961-161">The maximum number of devices that a user can enroll</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2961-162">关系</span><span class="sxs-lookup"><span data-stu-id="f2961-162">Relationships</span></span>
|<span data-ttu-id="f2961-163">关系</span><span class="sxs-lookup"><span data-stu-id="f2961-163">Relationship</span></span>|<span data-ttu-id="f2961-164">类型</span><span class="sxs-lookup"><span data-stu-id="f2961-164">Type</span></span>|<span data-ttu-id="f2961-165">说明</span><span class="sxs-lookup"><span data-stu-id="f2961-165">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2961-166">assignments</span><span class="sxs-lookup"><span data-stu-id="f2961-166">assignments</span></span>|<span data-ttu-id="f2961-167">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2961-167">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f2961-168">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备配置文件组的组分配列表</span><span class="sxs-lookup"><span data-stu-id="f2961-168">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2961-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2961-169">JSON Representation</span></span>
<span data-ttu-id="f2961-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2961-170">Here is a JSON representation of the resource.</span></span>
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
  "roleScopeTagIds": [
    "String"
  ],
  "limit": 1024
}
```





