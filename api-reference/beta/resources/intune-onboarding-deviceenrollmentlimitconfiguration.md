---
title: deviceEnrollmentLimitConfiguration 资源类型
description: 限制用户可以注册的设备数量的设备注册配置
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 956bb4593bd6efc9a08e1ae2ee077c8770cf0615
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43418919"
---
# <a name="deviceenrollmentlimitconfiguration-resource-type"></a><span data-ttu-id="b63d4-103">deviceEnrollmentLimitConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="b63d4-103">deviceEnrollmentLimitConfiguration resource type</span></span>

<span data-ttu-id="b63d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b63d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b63d4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b63d4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b63d4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b63d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b63d4-107">限制用户可以注册的设备数量的设备注册配置</span><span class="sxs-lookup"><span data-stu-id="b63d4-107">Device Enrollment Configuration that restricts the number of devices a user can enroll</span></span>


<span data-ttu-id="b63d4-108">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b63d4-108">Inherits from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b63d4-109">方法</span><span class="sxs-lookup"><span data-stu-id="b63d4-109">Methods</span></span>
|<span data-ttu-id="b63d4-110">方法</span><span class="sxs-lookup"><span data-stu-id="b63d4-110">Method</span></span>|<span data-ttu-id="b63d4-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b63d4-111">Return Type</span></span>|<span data-ttu-id="b63d4-112">说明</span><span class="sxs-lookup"><span data-stu-id="b63d4-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b63d4-113">列出 deviceEnrollmentLimitConfigurations</span><span class="sxs-lookup"><span data-stu-id="b63d4-113">List deviceEnrollmentLimitConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-list.md)|<span data-ttu-id="b63d4-114">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b63d4-114">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) collection</span></span>|<span data-ttu-id="b63d4-115">列出 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b63d4-115">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="b63d4-116">获取 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="b63d4-116">Get deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-get.md)|[<span data-ttu-id="b63d4-117">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="b63d4-117">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="b63d4-118">读取 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b63d4-118">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b63d4-119">创建 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="b63d4-119">Create deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-create.md)|[<span data-ttu-id="b63d4-120">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="b63d4-120">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="b63d4-121">创建新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b63d4-121">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b63d4-122">删除 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="b63d4-122">Delete deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-delete.md)|<span data-ttu-id="b63d4-123">无</span><span class="sxs-lookup"><span data-stu-id="b63d4-123">None</span></span>|<span data-ttu-id="b63d4-124">删除 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="b63d4-124">Deletes a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>|
|[<span data-ttu-id="b63d4-125">更新 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="b63d4-125">Update deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-update.md)|[<span data-ttu-id="b63d4-126">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="b63d4-126">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="b63d4-127">更新 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b63d4-127">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b63d4-128">属性</span><span class="sxs-lookup"><span data-stu-id="b63d4-128">Properties</span></span>
|<span data-ttu-id="b63d4-129">属性</span><span class="sxs-lookup"><span data-stu-id="b63d4-129">Property</span></span>|<span data-ttu-id="b63d4-130">类型</span><span class="sxs-lookup"><span data-stu-id="b63d4-130">Type</span></span>|<span data-ttu-id="b63d4-131">说明</span><span class="sxs-lookup"><span data-stu-id="b63d4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b63d4-132">id</span><span class="sxs-lookup"><span data-stu-id="b63d4-132">id</span></span>|<span data-ttu-id="b63d4-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b63d4-133">String</span></span>|<span data-ttu-id="b63d4-134">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="b63d4-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b63d4-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b63d4-135">displayName</span></span>|<span data-ttu-id="b63d4-136">String</span><span class="sxs-lookup"><span data-stu-id="b63d4-136">String</span></span>|<span data-ttu-id="b63d4-137">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="b63d4-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b63d4-138">description</span><span class="sxs-lookup"><span data-stu-id="b63d4-138">description</span></span>|<span data-ttu-id="b63d4-139">String</span><span class="sxs-lookup"><span data-stu-id="b63d4-139">String</span></span>|<span data-ttu-id="b63d4-140">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="b63d4-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b63d4-141">priority</span><span class="sxs-lookup"><span data-stu-id="b63d4-141">priority</span></span>|<span data-ttu-id="b63d4-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b63d4-142">Int32</span></span>|<span data-ttu-id="b63d4-143">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="b63d4-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="b63d4-144">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="b63d4-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="b63d4-145">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b63d4-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b63d4-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b63d4-146">createdDateTime</span></span>|<span data-ttu-id="b63d4-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b63d4-147">DateTimeOffset</span></span>|<span data-ttu-id="b63d4-148">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="b63d4-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b63d4-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b63d4-149">lastModifiedDateTime</span></span>|<span data-ttu-id="b63d4-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b63d4-150">DateTimeOffset</span></span>|<span data-ttu-id="b63d4-151">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="b63d4-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b63d4-152">version</span><span class="sxs-lookup"><span data-stu-id="b63d4-152">version</span></span>|<span data-ttu-id="b63d4-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b63d4-153">Int32</span></span>|<span data-ttu-id="b63d4-154">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="b63d4-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b63d4-155">limit</span><span class="sxs-lookup"><span data-stu-id="b63d4-155">limit</span></span>|<span data-ttu-id="b63d4-156">Int32</span><span class="sxs-lookup"><span data-stu-id="b63d4-156">Int32</span></span>|<span data-ttu-id="b63d4-157">用户可注册的最大设备数</span><span class="sxs-lookup"><span data-stu-id="b63d4-157">The maximum number of devices that a user can enroll</span></span>|

## <a name="relationships"></a><span data-ttu-id="b63d4-158">关系</span><span class="sxs-lookup"><span data-stu-id="b63d4-158">Relationships</span></span>
|<span data-ttu-id="b63d4-159">关系</span><span class="sxs-lookup"><span data-stu-id="b63d4-159">Relationship</span></span>|<span data-ttu-id="b63d4-160">类型</span><span class="sxs-lookup"><span data-stu-id="b63d4-160">Type</span></span>|<span data-ttu-id="b63d4-161">说明</span><span class="sxs-lookup"><span data-stu-id="b63d4-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b63d4-162">assignments</span><span class="sxs-lookup"><span data-stu-id="b63d4-162">assignments</span></span>|<span data-ttu-id="b63d4-163">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b63d4-163">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b63d4-164">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备配置文件组的组分配列表</span><span class="sxs-lookup"><span data-stu-id="b63d4-164">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b63d4-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b63d4-165">JSON Representation</span></span>
<span data-ttu-id="b63d4-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b63d4-166">Here is a JSON representation of the resource.</span></span>
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



