---
title: deviceEnrollmentLimitConfiguration 资源类型
description: 限制用户可以注册的设备数量的设备注册配置
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20bfb7eb49aeadb3ebd6fae4bad8fbf8c848e960
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196516"
---
# <a name="deviceenrollmentlimitconfiguration-resource-type"></a><span data-ttu-id="76230-103">deviceEnrollmentLimitConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="76230-103">deviceEnrollmentLimitConfiguration resource type</span></span>

> <span data-ttu-id="76230-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="76230-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76230-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76230-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76230-106">限制用户可以注册的设备数量的设备注册配置</span><span class="sxs-lookup"><span data-stu-id="76230-106">Device Enrollment Configuration that restricts the number of devices a user can enroll</span></span>


<span data-ttu-id="76230-107">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76230-107">Inherits from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="76230-108">方法</span><span class="sxs-lookup"><span data-stu-id="76230-108">Methods</span></span>
|<span data-ttu-id="76230-109">方法</span><span class="sxs-lookup"><span data-stu-id="76230-109">Method</span></span>|<span data-ttu-id="76230-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="76230-110">Return Type</span></span>|<span data-ttu-id="76230-111">说明</span><span class="sxs-lookup"><span data-stu-id="76230-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="76230-112">列出 deviceEnrollmentLimitConfigurations</span><span class="sxs-lookup"><span data-stu-id="76230-112">List deviceEnrollmentLimitConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-list.md)|<span data-ttu-id="76230-113">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="76230-113">[deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) collection</span></span>|<span data-ttu-id="76230-114">列出 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="76230-114">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="76230-115">获取 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="76230-115">Get deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-get.md)|[<span data-ttu-id="76230-116">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="76230-116">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="76230-117">读取 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="76230-117">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="76230-118">创建 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="76230-118">Create deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-create.md)|[<span data-ttu-id="76230-119">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="76230-119">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="76230-120">创建新的 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="76230-120">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|
|[<span data-ttu-id="76230-121">删除 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="76230-121">Delete deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-delete.md)|<span data-ttu-id="76230-122">无</span><span class="sxs-lookup"><span data-stu-id="76230-122">None</span></span>|<span data-ttu-id="76230-123">删除 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="76230-123">Deletes a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>|
|[<span data-ttu-id="76230-124">更新 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="76230-124">Update deviceEnrollmentLimitConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentlimitconfiguration-update.md)|[<span data-ttu-id="76230-125">deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="76230-125">deviceEnrollmentLimitConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)|<span data-ttu-id="76230-126">更新 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="76230-126">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="76230-127">属性</span><span class="sxs-lookup"><span data-stu-id="76230-127">Properties</span></span>
|<span data-ttu-id="76230-128">属性</span><span class="sxs-lookup"><span data-stu-id="76230-128">Property</span></span>|<span data-ttu-id="76230-129">类型</span><span class="sxs-lookup"><span data-stu-id="76230-129">Type</span></span>|<span data-ttu-id="76230-130">说明</span><span class="sxs-lookup"><span data-stu-id="76230-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76230-131">id</span><span class="sxs-lookup"><span data-stu-id="76230-131">id</span></span>|<span data-ttu-id="76230-132">字符串</span><span class="sxs-lookup"><span data-stu-id="76230-132">String</span></span>|<span data-ttu-id="76230-133">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="76230-133">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="76230-134">displayName</span><span class="sxs-lookup"><span data-stu-id="76230-134">displayName</span></span>|<span data-ttu-id="76230-135">String</span><span class="sxs-lookup"><span data-stu-id="76230-135">String</span></span>|<span data-ttu-id="76230-136">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="76230-136">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="76230-137">说明</span><span class="sxs-lookup"><span data-stu-id="76230-137">description</span></span>|<span data-ttu-id="76230-138">String</span><span class="sxs-lookup"><span data-stu-id="76230-138">String</span></span>|<span data-ttu-id="76230-139">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="76230-139">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="76230-140">priority</span><span class="sxs-lookup"><span data-stu-id="76230-140">priority</span></span>|<span data-ttu-id="76230-141">Int32</span><span class="sxs-lookup"><span data-stu-id="76230-141">Int32</span></span>|<span data-ttu-id="76230-142">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="76230-142">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="76230-143">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="76230-143">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="76230-144">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76230-144">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="76230-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76230-145">createdDateTime</span></span>|<span data-ttu-id="76230-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76230-146">DateTimeOffset</span></span>|<span data-ttu-id="76230-147">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="76230-147">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="76230-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76230-148">lastModifiedDateTime</span></span>|<span data-ttu-id="76230-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76230-149">DateTimeOffset</span></span>|<span data-ttu-id="76230-150">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="76230-150">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="76230-151">version</span><span class="sxs-lookup"><span data-stu-id="76230-151">version</span></span>|<span data-ttu-id="76230-152">Int32</span><span class="sxs-lookup"><span data-stu-id="76230-152">Int32</span></span>|<span data-ttu-id="76230-153">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="76230-153">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="76230-154">limit</span><span class="sxs-lookup"><span data-stu-id="76230-154">limit</span></span>|<span data-ttu-id="76230-155">Int32</span><span class="sxs-lookup"><span data-stu-id="76230-155">Int32</span></span>|<span data-ttu-id="76230-156">用户可注册的最大设备数</span><span class="sxs-lookup"><span data-stu-id="76230-156">The maximum number of devices that a user can enroll</span></span>|

## <a name="relationships"></a><span data-ttu-id="76230-157">关系</span><span class="sxs-lookup"><span data-stu-id="76230-157">Relationships</span></span>
|<span data-ttu-id="76230-158">关系</span><span class="sxs-lookup"><span data-stu-id="76230-158">Relationship</span></span>|<span data-ttu-id="76230-159">类型</span><span class="sxs-lookup"><span data-stu-id="76230-159">Type</span></span>|<span data-ttu-id="76230-160">说明</span><span class="sxs-lookup"><span data-stu-id="76230-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76230-161">assignments</span><span class="sxs-lookup"><span data-stu-id="76230-161">assignments</span></span>|<span data-ttu-id="76230-162">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="76230-162">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="76230-163">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备配置文件组的组分配列表</span><span class="sxs-lookup"><span data-stu-id="76230-163">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="76230-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76230-164">JSON Representation</span></span>
<span data-ttu-id="76230-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76230-165">Here is a JSON representation of the resource.</span></span>
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



