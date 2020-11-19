---
title: deviceComanagementAuthorityConfiguration 资源类型
description: Windows 10 Co-Management 证书颁发机构页面配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c287911666880bf0d6e45dc348c36a33198aee93
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49337009"
---
# <a name="devicecomanagementauthorityconfiguration-resource-type"></a><span data-ttu-id="ea386-103">deviceComanagementAuthorityConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea386-103">deviceComanagementAuthorityConfiguration resource type</span></span>

<span data-ttu-id="ea386-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea386-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea386-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ea386-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea386-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea386-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea386-107">Windows 10 Co-Management 证书颁发机构页面配置</span><span class="sxs-lookup"><span data-stu-id="ea386-107">Windows 10 Co-Management Authority Page Configuration</span></span>


<span data-ttu-id="ea386-108">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea386-108">Inherits from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ea386-109">Methods</span><span class="sxs-lookup"><span data-stu-id="ea386-109">Methods</span></span>
|<span data-ttu-id="ea386-110">方法</span><span class="sxs-lookup"><span data-stu-id="ea386-110">Method</span></span>|<span data-ttu-id="ea386-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="ea386-111">Return Type</span></span>|<span data-ttu-id="ea386-112">Description</span><span class="sxs-lookup"><span data-stu-id="ea386-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ea386-113">列出 deviceComanagementAuthorityConfigurations</span><span class="sxs-lookup"><span data-stu-id="ea386-113">List deviceComanagementAuthorityConfigurations</span></span>](../api/intune-onboarding-devicecomanagementauthorityconfiguration-list.md)|<span data-ttu-id="ea386-114">[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ea386-114">[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) collection</span></span>|<span data-ttu-id="ea386-115">列出 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ea386-115">List properties and relationships of the [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="ea386-116">获取 deviceComanagementAuthorityConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea386-116">Get deviceComanagementAuthorityConfiguration</span></span>](../api/intune-onboarding-devicecomanagementauthorityconfiguration-get.md)|[<span data-ttu-id="ea386-117">deviceComanagementAuthorityConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea386-117">deviceComanagementAuthorityConfiguration</span></span>](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|<span data-ttu-id="ea386-118">读取 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ea386-118">Read properties and relationships of the [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ea386-119">创建 deviceComanagementAuthorityConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea386-119">Create deviceComanagementAuthorityConfiguration</span></span>](../api/intune-onboarding-devicecomanagementauthorityconfiguration-create.md)|[<span data-ttu-id="ea386-120">deviceComanagementAuthorityConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea386-120">deviceComanagementAuthorityConfiguration</span></span>](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|<span data-ttu-id="ea386-121">创建新的 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ea386-121">Create a new [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ea386-122">删除 deviceComanagementAuthorityConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea386-122">Delete deviceComanagementAuthorityConfiguration</span></span>](../api/intune-onboarding-devicecomanagementauthorityconfiguration-delete.md)|<span data-ttu-id="ea386-123">无</span><span class="sxs-lookup"><span data-stu-id="ea386-123">None</span></span>|<span data-ttu-id="ea386-124">删除 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="ea386-124">Deletes a [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md).</span></span>|
|[<span data-ttu-id="ea386-125">更新 deviceComanagementAuthorityConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea386-125">Update deviceComanagementAuthorityConfiguration</span></span>](../api/intune-onboarding-devicecomanagementauthorityconfiguration-update.md)|[<span data-ttu-id="ea386-126">deviceComanagementAuthorityConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea386-126">deviceComanagementAuthorityConfiguration</span></span>](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|<span data-ttu-id="ea386-127">更新 [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ea386-127">Update the properties of a [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea386-128">属性</span><span class="sxs-lookup"><span data-stu-id="ea386-128">Properties</span></span>
|<span data-ttu-id="ea386-129">属性</span><span class="sxs-lookup"><span data-stu-id="ea386-129">Property</span></span>|<span data-ttu-id="ea386-130">类型</span><span class="sxs-lookup"><span data-stu-id="ea386-130">Type</span></span>|<span data-ttu-id="ea386-131">说明</span><span class="sxs-lookup"><span data-stu-id="ea386-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea386-132">id</span><span class="sxs-lookup"><span data-stu-id="ea386-132">id</span></span>|<span data-ttu-id="ea386-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ea386-133">String</span></span>|<span data-ttu-id="ea386-134">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的帐户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="ea386-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ea386-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ea386-135">displayName</span></span>|<span data-ttu-id="ea386-136">字符串</span><span class="sxs-lookup"><span data-stu-id="ea386-136">String</span></span>|<span data-ttu-id="ea386-137">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的显示名称</span><span class="sxs-lookup"><span data-stu-id="ea386-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ea386-138">description</span><span class="sxs-lookup"><span data-stu-id="ea386-138">description</span></span>|<span data-ttu-id="ea386-139">字符串</span><span class="sxs-lookup"><span data-stu-id="ea386-139">String</span></span>|<span data-ttu-id="ea386-140">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的说明</span><span class="sxs-lookup"><span data-stu-id="ea386-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ea386-141">priority</span><span class="sxs-lookup"><span data-stu-id="ea386-141">priority</span></span>|<span data-ttu-id="ea386-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ea386-142">Int32</span></span>|<span data-ttu-id="ea386-143">当用户存在于分配有注册配置的多个组中时，将使用优先级。</span><span class="sxs-lookup"><span data-stu-id="ea386-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="ea386-144">用户仅限于具有最低优先级值的配置。</span><span class="sxs-lookup"><span data-stu-id="ea386-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="ea386-145">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea386-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ea386-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea386-146">createdDateTime</span></span>|<span data-ttu-id="ea386-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea386-147">DateTimeOffset</span></span>|<span data-ttu-id="ea386-148">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 格式的创建日期时间</span><span class="sxs-lookup"><span data-stu-id="ea386-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ea386-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea386-149">lastModifiedDateTime</span></span>|<span data-ttu-id="ea386-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea386-150">DateTimeOffset</span></span>|<span data-ttu-id="ea386-151">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备注册配置的 UTC 的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="ea386-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ea386-152">version</span><span class="sxs-lookup"><span data-stu-id="ea386-152">version</span></span>|<span data-ttu-id="ea386-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ea386-153">Int32</span></span>|<span data-ttu-id="ea386-154">继承自[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)的设备注册配置的版本</span><span class="sxs-lookup"><span data-stu-id="ea386-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ea386-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ea386-155">roleScopeTagIds</span></span>|<span data-ttu-id="ea386-156">String 集合</span><span class="sxs-lookup"><span data-stu-id="ea386-156">String collection</span></span>|<span data-ttu-id="ea386-157">注册限制的可选角色范围标记。</span><span class="sxs-lookup"><span data-stu-id="ea386-157">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="ea386-158">继承自 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea386-158">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ea386-159">managedDeviceAuthority</span><span class="sxs-lookup"><span data-stu-id="ea386-159">managedDeviceAuthority</span></span>|<span data-ttu-id="ea386-160">Int32</span><span class="sxs-lookup"><span data-stu-id="ea386-160">Int32</span></span>|<span data-ttu-id="ea386-161">CoManagement 颁发机构配置 ManagedDeviceAuthority</span><span class="sxs-lookup"><span data-stu-id="ea386-161">CoManagement Authority configuration ManagedDeviceAuthority</span></span>|
|<span data-ttu-id="ea386-162">installConfigurationManagerAgent</span><span class="sxs-lookup"><span data-stu-id="ea386-162">installConfigurationManagerAgent</span></span>|<span data-ttu-id="ea386-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea386-163">Boolean</span></span>|<span data-ttu-id="ea386-164">CoManagement 颁发机构配置 InstallConfigurationManagerAgent</span><span class="sxs-lookup"><span data-stu-id="ea386-164">CoManagement Authority configuration InstallConfigurationManagerAgent</span></span>|
|<span data-ttu-id="ea386-165">configurationManagerAgentCommandLineArgument</span><span class="sxs-lookup"><span data-stu-id="ea386-165">configurationManagerAgentCommandLineArgument</span></span>|<span data-ttu-id="ea386-166">字符串</span><span class="sxs-lookup"><span data-stu-id="ea386-166">String</span></span>|<span data-ttu-id="ea386-167">CoManagement 颁发机构配置 ConfigurationManagerAgentCommandLineArgument</span><span class="sxs-lookup"><span data-stu-id="ea386-167">CoManagement Authority configuration ConfigurationManagerAgentCommandLineArgument</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea386-168">关系</span><span class="sxs-lookup"><span data-stu-id="ea386-168">Relationships</span></span>
|<span data-ttu-id="ea386-169">关系</span><span class="sxs-lookup"><span data-stu-id="ea386-169">Relationship</span></span>|<span data-ttu-id="ea386-170">类型</span><span class="sxs-lookup"><span data-stu-id="ea386-170">Type</span></span>|<span data-ttu-id="ea386-171">Description</span><span class="sxs-lookup"><span data-stu-id="ea386-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea386-172">assignments</span><span class="sxs-lookup"><span data-stu-id="ea386-172">assignments</span></span>|<span data-ttu-id="ea386-173">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ea386-173">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ea386-174">从[DeviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)继承的设备配置文件组的组分配列表</span><span class="sxs-lookup"><span data-stu-id="ea386-174">The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea386-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea386-175">JSON Representation</span></span>
<span data-ttu-id="ea386-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea386-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComanagementAuthorityConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComanagementAuthorityConfiguration",
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
  "managedDeviceAuthority": 1024,
  "installConfigurationManagerAgent": true,
  "configurationManagerAgentCommandLineArgument": "String"
}
```




